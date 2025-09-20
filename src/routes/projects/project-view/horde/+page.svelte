<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ['Unreal Engine', 'CI/CD', 'DevOps'];
	const workTags = ['Web Dev', 'React', 'TypeScript', 'ASP.NET Core', 'C#'];
</script>

<svelte:head>
	<title>Lucas C. | UE Horde</title>
</svelte:head>

<div class="mb-12">
	<h1 class="text-center text-6xl h1 font-bold mb-4">UE Horde</h1>
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
		<img class="w-full hidden sm:block" src="/screenshots/gauge.gif" alt="" />
		<img class="w-full sm:hidden" src="/screenshots/gauge_m.gif" alt="" />
	</figure>
	<p class="m-0 p-4 text-lg">
		While I cannot show much of Horde itself due to NDA, I can share some of my contributions to the
        project as a whole. If you wish to read more about Horde before continuing here, check out
        <a href="https://dev.epicgames.com/documentation/en-us/unreal-engine/horde-in-unreal-engine">the documentation</a>.
	</p>
</div>
<p>
	During the summer of 2025, I worked at Epic Games as an "Engine Programmer Intern" on the Horde team (a misleading title, I know). The average user
    interacts with Horde through the Horde Dashboard, a web application built with React and TypeScript. This is where I
    spent most of my time during the internship; however, I also got a good taste for server work.
</p>
<p>My primary contributions to Horde were the following:</p>
<ul>
	<li>
		Worked closely with stakeholders to identify their needs, and owned and developed a new build
        temperature gauge feature to indicate the stability of projects. This feature is depicted above.
        It's a simple interface with a lot of complexity under the hood, as it required a new server endpoint (ASP.NET Core)
        accompanied by a backend plugin system for per-project configuration and easy extension.
	</li>
	<li>
		Proactively led a cleanup effort to improve React and TypeScript code organization and documentation,
        standardize practices across the project, and streamline developer onboarding. This involved scanning
        the codebase for inconsistencies, drafting a proposal for improvements, and creating a Jira epic alongside
        tickets to document the work.
	</li>
</ul>

<p>As I cannot link to Horde, here's a bonus pic showcasing a tooltip!</p>
<img src="/screenshots/gauge.webp" alt="">
