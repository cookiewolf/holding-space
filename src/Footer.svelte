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
		background-color: #eeeeee;
		display: flex;
		justify-content: center;
		min-height: 4rem;
		width: 100%;
		margin-top: auto;
	}

	div {
		align-items: center;
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
	}

	a {
		text-decoration: none;
	}
</style>
