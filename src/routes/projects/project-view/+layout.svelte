<script lang="ts">
	import type { LayoutData } from './$types';

	export let data: LayoutData;
</script>

<div class="flex flex-col items-center">
	<a href="/projects" class="btn variant-outline-primary mb-12">
		<span>
			<i class="fa-solid fa-arrow-left"></i>
		</span>
		<span>Back To Projects</span>
	</a>

	<div class="prose dark:prose-invert max-w-[48rem]">
		<slot />
	</div>

	<a href="/projects" class="btn variant-outline-primary mt-12">
		<span>
			<i class="fa-solid fa-arrow-left"></i>
		</span>
		<span>Back To Projects</span>
	</a>
</div>
