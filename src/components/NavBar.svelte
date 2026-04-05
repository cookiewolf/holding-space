<script>
	import { resolve } from '$app/paths';
	import Container from './Container.svelte';
	import NavMenu from './NavMenu.svelte';
	import newtab from '$lib/assets/new-tab.svg';
</script>

<header>
	<Container>
		<div class="contents">
			<a href={resolve('/')} class="logo"> Holding Space Collective </a>
			<div class="mobile">
				<NavMenu />
			</div>
			<nav class="desktop">
				<ul>
					<li>
						<a href={resolve('/holding-space-short-series')}>Short Series</a>
					</li>
					<li>
						<a href={resolve('/holding-space-for-change')}>Holding Space For Change</a>
					</li>
					<li>
						<a href="https://raythespirit.com/holding-space-together" target="_blank" rel="noopener"
							>Facilitation Blog <img alt="opens in new tab" src={newtab} /></a
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
		border-bottom: 1px solid var(--grey);
		display: flex;
		justify-content: space-between;
		min-height: 4rem;
		width: 100%;
	}

	.contents {
		align-items: center;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
	}

	.logo {
		font-size: 1.3rem;
	}

	nav ul {
		display: flex;
		flex-direction: row;
		gap: 1rem;
	}

	a {
		font-family: PlexSerif, serif;
		text-decoration: none;
	}
	nav li {
		list-style: none;
	}

	nav a {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	nav a:hover {
		text-decoration: underline;
	}

	nav img {
		height: 1rem;
		width: 1rem;
	}

	.mobile {
		display: block;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.desktop {
		display: none;
	}

	@media (min-width: 800px) {
		.contents {
			align-items: baseline;
		}
		.desktop {
			display: contents;
		}

		.mobile {
			display: none;
		}
	}
</style>
