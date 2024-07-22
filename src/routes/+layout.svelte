<script lang="ts">
	import '../app.postcss';

	import { AppBar, Avatar, LightSwitch } from '@skeletonlabs/skeleton';
	import { page } from '$app/stores';

	$: routeId = $page.route.id;
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css"
		integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A=="
		crossorigin="anonymous"
		referrerpolicy="no-referrer"
	/>
</svelte:head>

<AppBar
	gridColumns="grid-cols-3"
	slotDefault="place-self-center"
	slotTrail="place-content-end"
	background="bg-transparent"
	class="mx-auto max-w-[80rem] hidden md:block"
>
	<svelte:fragment slot="lead">
		<a href="/" class="btn p-0">
			<Avatar
				width="w-12"
				src="/lucas_home.png"
				border="border-2 border-surface-300-600-token hover:!border-primary-500"
			/>
		</a>
	</svelte:fragment>
	<nav>
		<a
			href="/"
			class="btn btn-sm variant-outline-primary"
			class:variant-filled-primary={routeId === '/'}
		>
			Home
		</a>
		<a
			href="/projects"
			class="btn btn-sm variant-outline-primary"
			class:variant-filled-primary={routeId?.startsWith('/projects')}
		>
			Projects
		</a>
	</nav>
	<svelte:fragment slot="trail">
		<LightSwitch />
	</svelte:fragment>
</AppBar>
<AppBar
	gridColumns="grid-cols-1"
	slotDefault="flex justify-between items-center"
	background="bg-transparent"
	class="mx-auto max-w-[80rem] md:hidden"
>
	<nav>
		<a href="/" class="btn variant-outline-primary" class:variant-filled-primary={routeId === '/'}>
			Home
		</a>
		<a
			href="/projects"
			class="btn variant-outline-primary"
			class:variant-filled-primary={routeId?.startsWith('/projects')}
		>
			Projects
		</a>
	</nav>
	<LightSwitch />
</AppBar>

<div class="mx-auto max-w-[80rem] px-4 py-12">
	<slot />
</div>

<hr class="mb-8" />

<footer class="flex flex-col items-center p-8 pt-0 space-y-8">
	<div class="logo-cloud grid-cols-1 md:!grid-cols-3 gap-1 max-w-[80rem] w-full md:w-auto">
		<a class="logo-item p-4" href="https://github.com/ArgentumRhodon" target="_blank">
			<i class="fa-brands fa-github fa-xl"></i>
			<span>GitHub</span>
		</a>
		<a
			class="logo-item p-4"
			href="https://www.linkedin.com/in/lucas-corey-4a171421b/"
			target="_blank"
		>
			<i class="fa-brands fa-linkedin fa-xl"></i>
			<span>LinkedIn</span>
		</a>
		<a class="logo-item p-4" href="mailto:rit.lucascorey@gmail.com" target="_blank">
			<i class="fa-solid fa-envelope fa-xl"></i>
			<span>Email</span>
		</a>
	</div>
	<nav>
		<a
			href="/"
			class="btn btn-sm variant-outline-primary"
			class:variant-filled-primary={routeId === '/'}
		>
			Home
		</a>
		<a
			href="/projects"
			class="btn btn-sm variant-outline-primary"
			class:variant-filled-primary={routeId?.startsWith('/projects')}
		>
			Projects
		</a>
	</nav>
	<span class="text-sm opacity-75 text-primary-900-50-token">
		© Copyright 2024. All rights reserved.
	</span>
</footer>
