<script lang="ts">
    import Title from "$lib/components/title.svelte";
    import Container from "$lib/components/Container.svelte";
    import ProjectsCard from "$lib/components/ProjectsCard.svelte";
</script>
<title>
    Projects
</title>

<Container class="flex flex-col gap-16 ">
<Title title="مشاريعي"/>

<ProjectsCard 
imageSrc="/img1.jpg"
title=" جالسة تنطبخ "
subtitle="انتظروها ترا رهيبه 😉">
</ProjectsCard>


</Container>