<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import Container from '../Container.svelte';
	import NavBar from '../NavBar.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Holding Space</title>
</svelte:head>

<NavBar />
<Container>
	{@render children()}
</Container>

<style>
	:global(body) {
		font-family:
			system-ui,
			-apple-system,
			BlinkMacSystemFont,
			'Segoe UI',
			Roboto,
			Oxygen,
			Ubuntu,
			Cantarell,
			'Open Sans',
			'Helvetica Neue',
			sans-serif;
	}

	:global(*),
	:global(*)::before,
	:global(*)::after {
		box-sizing: border-box;
	}
</style>
