<script lang="ts">
    import Themeswitch from "$lib/components/Themeswitch.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import {page} from "$app/stores";
    import { text } from "@sveltejs/kit";
    import * as Sheet from "$lib/components/ui/sheet";
const links = [
      {
        text: 'الصفحة الرئيسية',
        herf: '/'
      },
      {
        text: 'سيرتي الذاتية  ',
        herf: '/RESUME'
      },
      {
        text: 'مشاريعي',
        herf: '/PROJECTS'
      },
      {
        text: 'التواصل',
        herf: '/CONTACT'
      }

]
let isSheetOpen = false;
</script>

<header  class=" w-[100dvw] bg-secondary text-secondary-foreground py-7 px-5">
  <nav 
    class="max-w-screen-2xl flex justify-between items-center mx-auto">
    <a href="/" class="flex gap-2 items-center">
        <div class="header__logo-img-cont flex items-center" >
          <img src="/sticker2.webp" alt="Nour salem" class="h-10 w-10"/>
        </div>
        <div class="flex items-end gap-2">
        <span class="font-bold text-3xl"> نور بنت سالم </span>
        <span class="text-1xl uppercase hidden sm:flex"> / طالبة علم بيانات </span>
        
    </div>
  </a>

      <!--Large Screen-->
      <div class="uppercase hidden md:flex">
      {#each links  as link }
        <Button
        class=" {$page.url.pathname == '/' && 'text-primary'}"
      href={link.herf}
      variant="link">{link.text}</Button>
      { /each}
      <Themeswitch/>
      </div>



      
        <!--Small Screen-->
      <Sheet.Root  bind:open={isSheetOpen}>
        <Sheet.Trigger  class="flex md:hidden ">
          
          <Button  variant="ghost" size="icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em"
              viewBox="0 0 20 20"><path fill="currentColor" fill-rule="evenodd"
              d="M2 8a1 1 0 0 1 1-1h10.308a1 1 0 1 1 0 2H3a1 1 0 0 1-1-1m0-4a1 1 
              0 0 1 1-1h14a1 1 0 1 1 0 2H3a1 1 0 0 1-1-1m0 8a1 1 0 0 1 1-1h14a1 1
              0 1 1 0 2H3a1 1 0 0 1-1-1m0 4a1 1 0 0 1 1-1h10.308a1 1 0 1 1 0 2H3a1 1 0 0 1-1-1" 
              clip-rule="evenodd"/></svg>
          </Button>
        </Sheet.Trigger>
        <Sheet.Content side="left" class="flex flex-col" >
          <Themeswitch/>
          {#each links  as link }
          <Button
          class=" text-2xl {$page.url.pathname == '/' && 'text-primary'}"
        href={link.herf}
        variant="link" on:click={() => isSheetOpen = false}
            >
          {link.text}
          </Button>
        { /each}
        </Sheet.Content>
      </Sheet.Root>
</nav>
</header>


