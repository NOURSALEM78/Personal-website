<script lang="ts">
export let date: string;
export let title: string;
export let company: string; 
</script>

<div class="bg-secondary p-6 shadow-2xl flex flex-col  justify-between gap-3 ]">
    <div class="flex  flex-col md:min-w-40 min-w-32 gap-4 ">
    <span class="text-primary font-bold">{date}</span>
    <span class="font-bold">{title}</span>
    <spsn>{company}</spsn>
    </div>
    <div>
        <slot/> 
    </div>
</div>