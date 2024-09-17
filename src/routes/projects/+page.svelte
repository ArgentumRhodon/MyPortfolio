<script lang="ts">
	import ProjectCard from '$lib/components/ProjectCard.svelte';
</script>

<svelte:head>
	<title>Lucas C. | Projects</title>
</svelte:head>

<h1 class="text-center text-6xl h1 font-bold mb-12">My Work</h1>

<div class="grid md:grid-cols-2 place-items-center justify-center gap-8">
	<ProjectCard
		name="Bat Bots"
		href="/projects/project-view/bat-bots"
		src="/cardImages/bat-bots.png"
		gameTags={['Arcade', 'Retro Shooter', 'Couch Co-op']}
		workTags={['Unity C#', 'Art', 'Web Dev', 'Marketing']}
	/>
	<ProjectCard
		name="ThenToMeet"
		href="/projects/project-view/then-to-meet"
		src="/cardImages/then-to-meet.png"
		gameTags={['Time Management', 'When2meet Tool']}
		workTags={['Web Dev', 'Svelte', 'TypeScript', 'Full Stack']}
	/>
</div>
