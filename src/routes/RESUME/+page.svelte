<script>
import Themeswitch from "$lib/components/Themeswitch.svelte";
import Button from "$lib/components/ui/button/button.svelte";
</script>
<title>
    Resume
</title>

<div class="max-w-screen-sm px-7 mx-auto pt-16">
    <h1 class="mx-auto w-fit text-5xl font-bold flex items-center  ">
        <div class="bg-primary w-5 h-5 me-4"/>
        <span>Resume</span>
    </h1>
    <div class="pt-16 flex flex-col gap-10">
        <div class="flex justify-between items-center">
            <spsn class="font-bold text-2xl">Education</spsn>
            <Button>Downloud My CV</Button>
        </div>
        <div class="bg-secondary p-8 shadow-2xl flex justify-between gap-0 ]">
            <div class="flex  flex-col md:min-w-40 min-w-32 gap-1 ">
            <span class="text-primary font-bold">
            2023 - present
            </span>
            <span class="font-bold">
                Data Science
            </span>
            <spsn>
                Umm AL-Qura University
            </spsn>
            </div>
            <div>
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Aliquid distinctio quasi asperiores accusantium ipsam laboriosam pariatur! 
                    Maiores, labore at aspernatur quae fugiat debitis possimus. Labore,
                    ex! Nobis saepe recusandae sit?
                </p>  
            </div>
        </div>
    </div>
</div>