<script>
	import { resolve } from '$app/paths';
	import Container from './Container.svelte';
</script>

<header>
	<Container>
		<div>
			<a href={resolve('/')}> Home </a>
			<nav>
				<ul>
					<li>
						<a href={resolve('/short-series')}>Short Series</a>
					</li>
					<li>
						<a href={resolve('/year-series')}>Year Series</a>
					</li>
					<li>
						<a href="https://raythespirit.com/holding-space-together" target="_blank" rel="noopener"
							>Facilitation Blog</a
						>
					</li>
				</ul>
			</nav>
		</div>
	</Container>
</header>

<style>
	header {
		align-items: center;
		display: flex;
		justify-content: space-between;
		min-height: 4rem;
		width: 100%;
	}

	div {
		align-items: center;
		display: flex;
		justify-content: space-between;
		flex-wrap: wrap;
	}

	nav ul {
		display: flex;
		flex-direction: row;
		gap: 1rem;
	}

	a {
		text-decoration: none;
	}

	nav a:hover {
		text-decoration: underline;
	}

	nav li {
		list-style: none;
	}
</style>
