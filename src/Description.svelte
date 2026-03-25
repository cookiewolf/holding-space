<script lang="ts">
	import type { Snippet } from 'svelte';

	let { id, children }: { id: string; children: Snippet } = $props();
</script>

<p {id}>
	{@render children?.()}
</p>

<style>
	p {
		font-size: smaller;
		font-style: italic;
	}
</style>
