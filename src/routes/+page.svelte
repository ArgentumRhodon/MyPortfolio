<script>
	import { Avatar, filter } from '@skeletonlabs/skeleton';
</script>

<svelte:head>
	<title>Lucas C. | Home</title>
</svelte:head>

<header class="flex flex-col-reverse md:flex-row md:items-center justify-between gap-8">
	<div class="max-w-2xl space-y-8">
		<h1 class="h1 text-7xl">Hi, I'm Lucas.</h1>
		<p class="text-2xl opacity-75">
			I am a game and front-end web developer currently studying for my Master of Science in Game
			Design and Development at Rochester Institute of Technology.
		</p>
		<a href="/resume.pdf" download="corey_l_resume.pdf" class="btn variant-filled-primary">
			<i class="fa-solid fa-download"></i>
			<span>Download Resume</span>
		</a>
	</div>
	<Avatar class="w-32 md:min-w-[400px] shadow-2xl" src="/lucas_home.png" rounded="rounded-token" />
</header>

<main>
	<div class="grid grid-cols-1 md:grid-cols-3 gap-4 lg:gap-8 mt-12">
		<div class="card variant-outline-surface p-4 md:p-8 space-y-4">
			<i class="fa-solid fa-star text-3xl"></i>
			<h2 class="h3">Fun</h2>
			<p class="opacity-75">
				When developers have fun creating a product, it often reflects in the quality of what's
				produced. Work hard and work smart, but remember to leave room for fun.
			</p>
		</div>
		<div class="card variant-outline-surface p-4 md:p-8 space-y-4">
			<i class="fa-solid fa-comments text-3xl"></i>
			<h2 class="h3">Communication</h2>
			<p class="opacity-75">
				It's a tale as old as time, but communication is key. Whether it's feedback, a schedule
				notice, or a deadline issue, be prompt, clear, and honest.
			</p>
		</div>
		<div class="card variant-outline-surface p-4 md:p-8 space-y-4">
			<i class="fa-solid fa-pencil fa-2xl"></i>
			<h2 class="h3">Learning</h2>
			<p class="opacity-75">
				"If everything you try works, you aren't trying hard enough." - Gordon Moore
			</p>
			<p class="opacity-75">Never stop learning; the tech industry won't wait up.</p>
		</div>
	</div>

	<div class="flex items-center my-12">
		<hr class="flex-grow" />
		<h1 class="text-center text-4xl h1 mx-4">About Me</h1>
		<hr class="flex-grow" />
	</div>

	<section class="mx-auto md:text-xl space-y-8">
		<header class="flex flex-col lg:flex-row items-center justify-between gap-8">
			<Avatar
				class="w-auto max-w-[400px] shadow-2xl"
				src="/lucas_about.png"
				rounded="rounded-token"
			/>
			<div class="max-w-2xl space-y-8">
				<p class="opacity-75">
					At RIT, I've worked on software and design projects from quick, iterative prototyping to
					full-scale production and documentation. My experience has primarily been in small
					cross-functional teams following a scrum-like process while prioritizing agile
					methodologies.
				</p>
				<p class="opacity-75">
					Another passion of mine is front-end web development. Although I'm still experimenting and
					trying new things, I'm loving the flexibility and control that Svelte and Tailwind
					provide.
				</p>
				<p class="opacity-75">
					In a place where I'm warmed by the sun, cooled by the shade, and refreshed by the breeze,
					with a painted sky above and the mountains of home surrounding, I find my greatest peace.
				</p>
			</div>
		</header>
	</section>
</main>
