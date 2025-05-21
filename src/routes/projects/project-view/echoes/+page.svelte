<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ['Community', 'Reflection', 'Connection'];
	const workTags = ['Web Dev', 'Svelte', 'JavaScript', 'Vertically Integrated Project'];
</script>

<svelte:head>
	<title>Lucas C. | echoes</title>
</svelte:head>

<div class="mb-12">
	<h1 class="text-center text-6xl h1 font-bold mb-4"><i>echoes</i></h1>
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
		<img src="/screenshots/echoes.png" alt="" />
	</figure>
	<p class="m-0 p-4 text-lg">
		<i>echoes</i> is a credit-bearing student-led, student-run project at Rochester Institute of Technology
		exploring how developing and playing games can cultivate shared understanding and foster meaningful
		connections.
	</p>
</div>
<p>
	During the fall of 2024 and spring of 2025, I led a small team of web developers for the
	<i>echoes</i> website. We built the website from the ground up using Svelte, JavaScript, and
	TailwindCSS. This website is a source of information about <i>echoes</i> as a project, as an RIT course,
	and as a community.
</p>
<p>My primary contributions:</p>
<ul>
	<li>
		Mentored two to three peers in the use of Svelte, JavaScript, and TailwindCSS to develop
		<a href="https://www.echoes-vip.org/">the <i>echoes</i> website.</a>
	</li>
	<li>
		Created custom GitHub actions for CI/CD, using Vercel's CLI to enable automatic development and
		production deployments despite using Vercel's free tier with a team repository.
	</li>
	<li>
		Developed simple data and content pipelines with Google Sheets and Google Apps Script, allowing
		for easy updates to team and project information.
	</li>
</ul>

<a href="https://www.echoes-vip.org/" class="btn variant-filled-primary w-full" target="_blank">
	<span><i class="fa-solid fa-link"></i></span>
	<span>The <i>echoes</i> Website</span>
</a>
