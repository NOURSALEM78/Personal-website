<script>
    import Telegram from "$lib/icons/telegram.svelte";
import { Footer } from "./ui/sheet";
import SocialMedia from "$lib/components/SocialMedia.svelte"

</script>
<footer class=" w-[100dvw] bg-secondary text-secondary-foreground py-4 px-4 ">
    <div class="max-w-screen-2xl flex justify-between items-center mx-auto ">
    <span>
    © {(new Date()).getFullYear()} 
    </span>
    <span class="flex flex-col items-center">
        <span class="font-bold">call</span>
        <a href="tel:0566217334">0566217334</a> 
    </span>
    <span class="flex flex-col items-center">
        <span class="font-bold">call</span>
        <a href="mailto:noursalm261@gmail.com">noursalm261@gmail.com</a> 
    </span>
        <span class="flex items-end   "><SocialMedia/></span>
    </div>
</footer>