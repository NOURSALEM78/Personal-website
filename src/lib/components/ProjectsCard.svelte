<script lang="ts">
    export let title: string;
    export let subtitle: string; 
    export let imageSrc: string;
    </script>
    
    <div class="bg-secondary shadow-xl flex flex-col sm:flex-row gap-4 ">
        <div class="flex flex-col  gap-0 pt-8">
            <div class="flex  flex-col min-w-80 border-s-8 border-primary ps-8">
                <span class="font-bold text-primary text-xl">{title}</span>
                    <spsn>{subtitle}</spsn>
            </div>
                <div class="ps-8 pb-8">
                <slot/> 
            </div>
        </div>
        <img src={imageSrc} alt="صورة المشروع" class="w-auto sm:w-64 obj"/>
    </div>