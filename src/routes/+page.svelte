<script>
	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Holding Space for Change</h1>
	</div>

	<div class="programmes">
		<div class="programme">
			<h2>Holding Space for Change</h2>
			<p>Year series description</p>
			<a href={resolve('/holding-space-for-change')}>Find out more</a>
		</div>
		<div class="programme">
			<h2>Holding Space Short Series</h2>
			<p>Short series description</p>
			<a href={resolve('/holding-space-short-series')}>Find out more</a>
		</div>
	</div>
</main>

<style>
	.hero {
		align-items: center;
		background-color: #eeeeee;
		display: flex;
		height: 20rem;
		justify-content: center;
		width: 100%;
	}

	.programmes {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		margin: 2rem 0;
	}

	h2 {
		margin: 0;
		padding: 0;
	}

	.programme {
		background-color: #eeeeee;
		border-radius: 1rem;
		min-width: 0;
		padding: 1rem;
		width: 100%;
	}

	@media (min-width: 600px) {
		.programmes {
			flex-direction: row;
		}

		.programme {
			width: 100%;
		}
	}
</style>
