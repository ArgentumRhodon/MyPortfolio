<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ['Time Management', 'When2meet Tool'];
	const workTags = ['Web Dev', 'Svelte', 'TypeScript', 'Full Stack'];
</script>

<svelte:head>
	<title>Lucas C. | ThenToMeet</title>
</svelte:head>

<div class="mb-12">
	<h1 class="text-center text-6xl h1 font-bold mb-4">ThenToMeet</h1>
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
	<figure class="w-full aspect-video m-0">
		<img src="/screenshots/then-to-meet.png" alt="" />
	</figure>
	<p class="m-0 p-4 text-lg">
		Tired of peeking through large When2meet events to find meeting times for sub-groups? No? I was,
		so I made ThenToMeet!
	</p>
</div>
<p>
	ThenToMeet is a web application for finding overlaps between specific members of any When2meet
	event. It was inspired by the inconvenience I and many of my peers and professors experienced with
	When2meet when setting up recurring team meetings for a medium-size project course with multiple
	subteams.
</p>
<p>
	Why not build an improved When2meet clone you ask? It seemed unnecessary; why build something with
	profile authentication and database queries when I can just parse a When2meet page with RegEx to
	populate my app?
</p>
<a href="https://www.thentomeet.com" class="btn variant-filled-primary w-full" target="_blank">
	<span><i class="fa-solid fa-link"></i></span>
	<span>ThenToMeet</span>
</a>
