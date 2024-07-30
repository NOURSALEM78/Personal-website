<script>
    import Themeswitch from "$lib/components/Themeswitch.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import {page} from "$app/stores";
    import { text } from "@sveltejs/kit";
    import * as Sheet from "$lib/components/ui/sheet";

const links = [
      {
        text: 'About me',
        herf: '/'
      },
      {
        text: 'Resume',
        herf: '/RESUME'
      },
      {
        text: 'Projects',
        herf: '/PROJECTS'
      },
      {
        text: 'Contact',
        herf: '/CONTACT'
      }

]
let isSheetOpen = false;
</script>

<header class=" w-[100dvw] bg-secondary 
    text-secondary-foreground py-4 px-4">
  <nav 
    class="max-w-screen-2xl flex justify-between items-center mx-auto">
    <a href=" /" class="flex gap-2 items-center">
        <div class="header__logo-img-cont flex items-center" >
          <img src="/sticker2.webp" alt="Nour salem" class="h-10 w-10"/>
        </div>
        <div class="flex items-end gap-2">
        <span class="font-bold text-3xl"> Nour salem </span>
        <span class="text-1xl uppercase hidden sm:flex"> / DS student </span>
        
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
      <Sheet.Root bind:open={isSheetOpen}>
        <Sheet.Trigger class="flex md:hidden">
          
          <Button  variant="ghost" size="icon">
            <svg class="w-10 h-auto"
            xmlns="http://www.w3.org/2000/svg" 
            viewBox="0 0 24 24"><g 
            fill="none" stroke="currentColor" 
            stroke-linecap="round" stroke-width="2"
            ><path stroke-dasharray="10" stroke-dashoffset="10" d="M7 9L4 12L7 15"
            ><animate fill="freeze" attributeName="stroke-dashoffset" 
            begin="0.6s" dur="0.2s" values="10;0"/></path><path
            stroke-dasharray="16" stroke-dashoffset="16" d="M19 5H5">
            <animate fill="freeze" attributeName="stroke-dashoffset" dur="0.2s" values="16;0"/>
          </path><path stroke-dasharray="12" stroke-dashoffset="12" d="M19 12H10">
            <animate fill="freeze" attributeName="stroke-dashoffset" begin="0.2s" dur="0.2s" values="12;0"/>
          </path><path stroke-dasharray="16" stroke-dashoffset="16" d="M19 19H5"
          ><animate fill="freeze" attributeName="stroke-dashoffset" begin="0.4s"
            dur="0.2s" values="16;0"/></path></g></svg>
          </Button>
        </Sheet.Trigger>
        <Sheet.Content class="flex flex-col">
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


