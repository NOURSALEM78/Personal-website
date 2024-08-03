<script>
        import Button from "$lib/components/ui/button/button.svelte";
        import SocialMedia from "$lib/components/SocialMedia.svelte";
        
</script>
<title>
    Nour salem
</title>

<div class="flex justify-end pb-[35rem] lg:pb-0 ">
    <div class="bg-secondary relative w-full lg:w-[60vw] min-h-[40vh]
    lg:min-h-[calc(100vh-9.5rem)]  flex justify-center items-center pb-32 ">
        <div
        class="bg-[#e8e3e1] shadow-[0_35px_60px_-15px_rgba(0,0,0,0.6)] w-[22rem] absolute  
        lg:start-10 lg:-translate-x-[-103%]  flex flex-col items-center 
        justify-between pt-5 dark:text-secondary-foreground 
        translate-y-[95%] lg:translate-y-[10%] max-w-[85vw]">
        
        <img
        src="/sticker.webp" 
        alt="Nour salem" 
        class="rounded-full w-64"/>
            
            <div class="flex flex-col items-center gap-6 dark:text-secondary">
                <h1 class="font-bold text-4xl"> نور بنت سالم  </h1>
                <hr class="w-24 border-2 border-primary dark:border-secondary"/>
                <h2 class="text-2xl"> طالبة علم بيانات  </h2>
            </div>
            
            <div class="bg-secondary w-full flex justify-center p-2 mt-8">
            <SocialMedia/>
            </div>
        </div>
        <div class="max-w-[35rem] flex flex-col gap-9 justify-center mx-10">
            <h1 class="text-5xl font-bold">
                أهلا،
            </h1>
            <h4 class="text-3xl " >
                صفحة شخصية تضم كل انجازاتي
            </h4>
            <div class="flex gap-5 dark:text-secondary ">
                <Button href="/RESUME" variant="outline" class="w-40">
                    سيرتي الذاتية 
                </Button>
                <Button href="/PROJECTS" variant="outline" class="w-40">
                    مشاريعي
                </Button>
            </div>
            <div >
                <p >
                    طالبة علم بيانات في جامعه ام القرى، كلية الحاسبات.
                عضو في اللجنة التنظيمية بنادي الحاسبات، وعضو في مجتمع كبتار التقني التابع لجمعية عون التقنية. 
                </p>
            </div>
        </div>
    </div>
</div>
