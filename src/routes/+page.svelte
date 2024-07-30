<script>
        import Button from "$lib/components/ui/button/button.svelte";
        import SocialMedia from "$lib/components/SocialMedia.svelte";
</script>
<title>
    Nour salem
</title>

<div class="flex justify-end pb-[35rem] lg:pb-0">
    <div class="bg-secondary drark: w-full md:w-[60vw] min-h-[40vh] lg:min-h-[calc(100vh-9.5rem)] relative
flex justify-center pb-20">
        <div
        class="bg-[#e8e3e1] shadow-[0_35px_60px_-15px_rgba(0,0,0,0.6)] w-[22rem] absolute  
        lg:start-10 lg:-translate-x-full  flex flex-col items-center 
        justify-between pt-4 gap-3 dark:text-secondary-foreground 
        translate-y-[90%] lg:translate-y-1/4 max-w-[85vw]">
        
        <img
        src="/sticker.webp" 
        alt="Nour salem" 
        class="rounded-full w-64"/>
            
            <div class="flex flex-col items-center gap-6 dark:text-secondary">
                <h1 class="font-bold text-4xl"> Nour salem  </h1>
                <hr class="w-24 border-2 border-primary dark:border-secondary"/>
                <h2 class="text-2xl"> DS Student  </h2>
            </div>
            
            <div class="bg-secondary w-full flex justify-center p-2 mt-8">
            <SocialMedia/>
            </div>
        </div>
        <div class="max-w-[35rem] flex flex-col gap-9 justify-center mx-10">
            <h1 class="text-8xl font-extrabold">
                Hello
            </h1>
            <h4 class="text-4xl">
                here's who i am and wht i do
            </h4>
            <div class="flex gap-5">
                <Button href="/RESUME" variant="outline" class="w-40">
                    RESUME
                </Button>
                <Button href="/PROJECTS" variant="outline" class="w-40">
                    PROJECTS
                </Button>
            </div>
            <div>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                    Quasi dicta tempora itaque eligendi! In ullam architecto necessitatibus,
                    cumque officia earum odit commodi optio facilis eum illo fuga enim est nulla?
                </p>
            </div>
        </div>
    </div>
</div>
