<script>
	import { resolve } from '$app/paths';
	import Container from './Container.svelte';
</script>

<footer>
	<Container>
		<div>
			<a href={resolve('/')}> Holding Space Collective </a>
		</div>
	</Container>
</footer>

<style>
	footer {
		align-items: center;
		background-color: var(--text);
		display: flex;
		justify-content: center;
		margin-top: auto;
		min-height: 4rem;
		width: 100%;
	}

	div {
		align-items: center;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

	a {
		text-decoration: none;
		color: #ffffff;
		font-family: PlexSerif, serif;
	}
</style>
