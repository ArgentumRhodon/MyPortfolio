<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ['Arcade', 'Retro Shooter', 'Couch Co-op'];
	const workTags = ['Unity C#', 'Art', 'Web Dev', 'Marketing'];
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
	For the summer of 2024, I am working full-time as a founding member of indie studio Yesteryear
	Games on <i>Bat Bots</i>, our love-letter to the classics targeted at older generations to play
	with their young relatives. Working on Bat Bots professionally has revealed the great difference
	between industry and academic-level work.
</p>
<p>
	My contributions to this game are widespread: from drafting the initial systems architecture to
	gameplay programming to producing background art and particle effects. I also took on the solo
	development of <a href="https://www.batbotsgame.com" target="_blank">the website</a> and
	<a href="https://store.steampowered.com/app/3099010/Bat_Bots/" target="_blank">Steam page</a>,
	which was aided by the frequent feedback of my teammates.
</p>
<p>
	As our production winds down and less technical and artistic work is needed, I have also performed
	as Yesteryear Games' marketing lead. Bat Bots releases on Steam Q3 2024!
</p>

<a
	href="https://linktr.ee/batbotsofficial"
	class="btn variant-filled-primary w-full"
	target="_blank"
>
	<span><i class="fa-solid fa-link"></i></span>
	<span>BatBots' Linktree</span>
</a>
