<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ['Arcade', 'Retro Shooter', 'Couch Co-op'];
	const workTags = ['Web Dev', 'Unity C#', 'Art'];
</script>

<svelte:head>
	<title>Lucas C. | Bat Bots</title>
</svelte:head>

<div class="mb-12">
	<h1 class="text-center text-6xl h1 font-bold mb-4">Bat Bots</h1>
	<ul class="flex flex-wrap gap-2 p-0 justify-center m-0">
		{#each gameTags as tag}
			<li class="badge variant-filled-primary">{tag}</li>
		{/each}
	</ul>
	<ul class="flex flex-wrap gap-2 p-0 justify-center m-0">
		{#each workTags as tag}
			<li class="badge variant-filled-secondary">{tag}</li>
		{/each}
	</ul>
</div>

<div class="card variant-filled-primary overflow-hidden">
	<iframe
		class="w-full aspect-video"
		src="https://www.youtube.com/embed/cDKbxhRROxo?si=ZnenMOA0XoSAhoPY"
		title="YouTube video player"
		frameborder="0"
		allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
		referrerpolicy="strict-origin-when-cross-origin"
		allowfullscreen
	></iframe>
	<p class="m-0 p-4 text-lg">
		Enjoy a modern take on timeless arcade action with <i>Bat Bots</i>, a nostalgic shooter inspired
		by the classics. Take down waves of robotic bats using precise aim and quick reflexes. Engage in
		solo play, challenge your friends and family, or work together to defend against the oncoming
		waves.
	</p>
</div>
<p>
	For the summer of 2024, I worked full-time as a founding member of indie studio Yesteryear Games
	on <i>Bat Bots</i>, our love-letter to the classics targeted at older generations to play with
	their young relatives. Working on Bat Bots professionally has revealed the great difference
	between industry and academic-level work.
</p>
<p>My primary contributions:</p>
<ul>
	<li>
		Used JavaScript, HTML, TailwindCSS, and Vercel to build and deploy
		<a href="https://www.batbotsgame.com">the website</a> for Bat Bots.
	</li>
	<li>
		Built the Steam page for Bat Bots. Used my art capabilities to make assets for the Steam page
		while our primary artist focused on the game itself.
	</li>
	<li>
		Created visual assets like background and particle effects for Bat Bots' customization systems.
	</li>
</ul>

<a
	href="https://linktr.ee/batbotsofficial"
	class="btn variant-filled-primary w-full"
	target="_blank"
>
	<span><i class="fa-solid fa-link"></i></span>
	<span>BatBots' Linktree</span>
</a>
