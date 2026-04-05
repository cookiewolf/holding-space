<script>
	let { children } = $props();
</script>

<div>
	{@render children?.()}
</div>

<style>
	div {
		margin: 0 auto;
		max-width: 1000px;
		padding: 0 var(--gutter-width);
		width: 100%;
	}
</style>
