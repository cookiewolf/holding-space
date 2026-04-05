<script lang="ts">
	import { resolve } from '$app/paths';
	import newtab from '$lib/assets/new-tab.svg';

	let open = $state(false);

	$effect(() => {
		if (open) {
			document.body.classList.add('menu-open');
		} else {
			document.body.classList.remove('menu-open');
		}
	});
</script>

<button aria-label="menu" class="menu-icon" onclick={() => (open = !open)}>
	<div></div>
	<div></div>
	<div></div>
</button>

<nav>
	<ul class="nav-links" class:open>
		<li>
			<a href={resolve('/holding-space-short-series')} onclick={() => (open = !open)}
				>Short Series</a
			>
		</li>
		<li>
			<a href={resolve('/holding-space-for-change')} onclick={() => (open = !open)}
				>Holding Space For Change</a
			>
		</li>
		<li>
			<a
				href="https://raythespirit.com/holding-space-together"
				target="_blank"
				rel="noopener"
				onclick={() => (open = !open)}
				>Facilitation Blog <img alt="opens in new tab" src={newtab} />
			</a>
		</li>
	</ul>
</nav>

<style>
	button {
		background: transparent;
		border-radius: 4px;
		border: 1px solid var(--pink-dark);
		cursor: pointer;
		display: flex;
		flex-direction: column;
		gap: 3px;
		height: 2rem;
		justify-content: center;
		padding: 0.25rem;
		width: 2rem;
	}

	.menu-icon div {
		background-color: var(--pink-dark);
		border-radius: 4px;
		height: 3px;
	}

	.nav-links {
		display: flex;
		flex-direction: column;
		gap: 20px;
		list-style: none;
	}

	.nav-links li {
		display: inline;
	}

	.nav-links a {
		align-items: center;
		color: var(--pink-dark);
		display: flex;
		font-family: PlexSerif, serif;
		font-size: 1.3rem;
		justify-content: center;
		text-decoration: none;
	}

	img {
		height: 1.3rem;
		width: 1.3rem;
	}

	@media (max-width: 800px) {
		.nav-links {
			background-color: white;
			display: none;
			height: calc(100vh - 4rem);
			left: 0;
			padding: 3rem;
			position: absolute;
			right: 0;
			text-align: center;
			top: 4rem;
			width: 100%;
		}

		.open {
			display: flex;
		}

		.nav-links li {
			margin: 2rem 0;
		}

		nav {
			align-items: center;
			display: flex;
			justify-content: space-between;
		}
	}
</style>
