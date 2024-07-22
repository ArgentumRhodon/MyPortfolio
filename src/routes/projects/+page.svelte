<script lang="ts">
	import ProjectCard from '$lib/components/ProjectCard.svelte';
</script>

<h1 class="text-center text-6xl h1 font-bold mb-12">My Work</h1>

<div class="flex justify-center gap-8">
	<ProjectCard
		name="Bat Bots"
		href="/projects/games/bat-bots"
		src="/cardImages/bat-bots.png"
		gameTags={['Arcade', 'Retro Shooter', 'Couch Co-op']}
		workTags={['Unity C#', 'Art', 'Web Dev', 'Marketing']}
	/>
</div>
