<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children, narrow }: { children: Snippet; narrow?: boolean } = $props();
</script>

<div class={narrow ? 'narrow' : ''}>
	{@render children?.()}
</div>

<style>
	div {
		margin: 0 auto;
		max-width: 1000px;
		padding: 0 var(--gutter-width);
		width: 100%;
	}

	.narrow {
		max-width: 800px;
	}
</style>
