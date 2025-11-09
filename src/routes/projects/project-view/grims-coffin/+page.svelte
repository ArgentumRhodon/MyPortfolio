<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;

	const gameTags = ["Metroidvania", "Themes of Grief"];
	const workTags = ["Unity C#", "Game Dev", "Pixel Art", "Tech Art"];
</script>

<svelte:head>
	<title>Lucas C. | Grim's Coffin</title>
</svelte:head>

<div class="mb-12">
	<h1 class="text-center text-6xl h1 font-bold mb-4">Grim's Coffin</h1>
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
		<img src="/screenshots/grims-coffin.webp" alt="" />
	</figure>
	<p class="m-0 p-4 text-lg">
        <span class="font-bold">Elevator Pitch: </span>
		In Grim’s Coffin, you play as the Grim Reaper, who, after a shocking revelation, must 
        find lost spirits and cut down terrible foes while coming to terms with their true nature.
	</p>
</div>
<p>
    <span class="font-bold">Extended Description: </span>
    You control Grim, whose sole purpose in the Underworld is to shepherd spirits to the
    King of the Underworld through a realm known as The Drift. After making a shocking
    revelation, Grim’s world is turned upside down and he must deal with his own grief
    while trying to guide the spirits he is responsible for. As you navigate through The
    Drift, you’ll encounter various foes trying to devour lost spirits. Use your scythe
    to cut them down, protect the lost spirits, and gain powerful new abilities, as you
    seek to understand your true purpose in the Underworld.
</p>

<p>
    I worked on Grim's Coffin as part of a team of five core students and many
    external contributors during Fall 2024 and Spring 2025 at Rochester Institute of
    Technology as part of my graduate capstone project. I worked mainly as the team's
    artist, technical artist, and backup programmer.
</p>

<p>My primary contributions:</p>
<ul>
    <li>
        Created and implemented pixel art assets for characters, environments, and UI elements,
        establishing a cohesive visual style for the game. <span class="bg-yellow-200/65 text-black">Note: Not all assets featured in the game
        are owned by me or our external artists. Some assets (like enemies and bosses) were sourced from free and paid asset packs to
        fill gaps in our art production pipeline. Credits for these assets are found at the end of the game.</span>
    </li>
    <li>
        Managed an experienced external artist to help produce high-quality art assets. This involved
        providing expectations, feedback, ensuring timely delivery of assets, tracking hours, and
        coordinating payment.
    </li>
    <li>
        Worked with RIT professor David Sanchez to enlist the help of talented undergraduate students
        to create animated pixel art assets for the game. Not all assets produced were used,
        but every student was granted credit for their work.
    </li>
    <li>
        Assisted in programming gameplay mechanics and systems using Unity and C#,
        distributing workload and ensuring smooth development progress during stressful
        periods.
    </li>
</ul>

<a
	href="https://kevin-insinna.itch.io/grims-coffin"
	class="btn variant-filled-primary w-full"
	target="_blank"
>
	<span><i class="fa-solid fa-link"></i></span>
	<span>Grim's Coffin (Itch.io)</span>
</a>

<p>
    If you wish to see my independent research into procedural pixel-art cloth animations
    in Aseprite, which I worked on alongside Grim's Coffin as part of my capstone, here it is!
    Apologies for the poor audio quality.
</p>
<iframe
    class="w-full aspect-video"
    src="https://www.youtube.com/embed/byTH6StWDC4?si=-nJY6_x-fV9Q_fDo"
    title="YouTube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
></iframe>