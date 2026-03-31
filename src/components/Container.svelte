<script>
	let { children } = $props();
</script>

<div>
	{@render children?.()}
</div>

<style>
	div {
		margin: 0 auto;
		max-width: 1200px;
		padding: var(--gutter-width);
		width: 100%;
	}
</style>
