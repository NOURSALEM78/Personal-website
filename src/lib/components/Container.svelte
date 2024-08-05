<script lang="ts">
    import {cn} from "$lib/utils";

    let className: string = "";

    export{ className as class}
</script>

<div class={cn("max-w-screen-sm px-6 mx-auto py-12",className)}>
    <slot/>
</div>
