<script>
        import Button from "$lib/components/ui/button/button.svelte";
        import X from "$lib/icons/X.svelte";
        import Telegram from "$lib/icons/telegram.svelte";
        import Email from "$lib/icons/Email.svelte";
        import LinkedIn from "$lib/icons/linkedIn.svelte";
</script>
<title>
    Nour salem
</title>

<div class="flex justify-end ">
<div class="bg-secondary min-h-[calc(100vh-4.5rem)] w-[60vw] relative">
        <div
        class="bg-[#e8e3e1] shadow-2xl w-[22rem] absolute start-10 
        -translate-x-full translate-y-1/4 flex flex-col items-center justify-between pt-8 gap-3">
        
        <img
        src="/sticker.webp" 
        alt="Nour salem" 
        class="rounded-full w-64"/>
            
            <div class="flex flex-col items-center gap-5 mt-12">
                <h1 class="font-bold text-4xl"> Nour salem  </h1>
                <hr class="w-24 border-2 border-primary"/>
                <h2 class="text-2xl"> DS Student  </h2>

                <div class="bg-secondary w-full flex justify-center">
                    <Button 
                    variant="ghost" 
                    size="icon" 
                    href="https://x.com/78Nour_"> <X/> </Button>
                    <Button  
                    variant="ghost" 
                    size="icon" 
                    href="https://t.me/awi_78"> <Telegram/> </Button>
                
                    <Button  
                    variant="ghost" 
                    size="icon" 
                    href="http://linkedin.com/in/nour-salem-b652b7283"> <LinkedIn/> </Button>
                </div>
            </div>
        </div>
    </div>
</div>
