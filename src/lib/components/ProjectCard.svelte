<script lang="ts">
	export let name: string = 'Project';
	export let src: string = 'https://placehold.co/400?text=Cover Image';
	export let href: string = '/projects';
	export let gameTags: string[] = ['Tag 1', 'Tag 2', 'Tag 3', 'Tag 4'];
	export let workTags: string[] = ['Tag 1', 'Tag 2', 'Tag 3', 'Tag 4'];
</script>

<a {href} class="card card-hover variant-outline-surface group max-w-96 overflow-hidden">
	<div class="overflow-hidden">
		<img {src} alt="" class="group-hover:scale-110 transition-transform duration-150" />
	</div>
	<div class="p-4">
		<span class="block text-xl mb-2">{name}</span>
		<ul class="flex flex-wrap gap-2 mb-2">
			{#each gameTags as tag}
				<li class="badge variant-filled-primary">{tag}</li>
			{/each}
		</ul>
		<ul class="flex flex-wrap gap-2">
			{#each workTags as tag}
				<li class="badge variant-filled-secondary">{tag}</li>
			{/each}
		</ul>
	</div>
</a>
