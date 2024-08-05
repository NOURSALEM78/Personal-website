<script lang="ts">
export let title: string;
</script>

<div class="bg-secondary p-6 shadow-2xl flex flex-col  justify-between gap-3 ]">
    <div class="flex  flex-col md:min-w-40 min-w-32 gap-4 ">
    <span class="font-bold text-2xl">{title}</span>
    </div>
    <div>
        <slot/> 
    </div>
</div>