<script>
    import Telegram from "$lib/icons/telegram.svelte";
import { Footer } from "./ui/sheet";
import SocialMedia from "$lib/components/SocialMedia.svelte"

</script> 
<footer class=" w-[100dvw] md:h-14 bg-secondary text-secondary-foreground md:py-1 py-4 px-10 ">
    <div class="max-w-screen-2xl flex flex-row-reverse md:flex-row justify-between items-center mx-auto ">
    <span class="self-end md:self-center">
    © {(new Date()).getFullYear()} 
    </span>
    <div class="flex flex-col md:flex-row md:gap-32 gap-4">
    <span class="flex gap-6 md:gap-0  md:flex-col items-center">
        <span class="font-bold">للاتصال</span>
        <a href="tel:0566217334">0566217334</a> 
    </span>
    <span class="flex gap-6 md:gap-0  md:flex-col items-center">
        <span class="font-bold">البريد </span>
        <a href="mailto:noursalm261@gmail.com">noursalm261@gmail.com</a> 
    </span>
        <span class="flex items-center md:justify-end  gap-4"><SocialMedia/></span>
        </div>
    </div>
</footer>