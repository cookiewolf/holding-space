<script>
	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Holding Space</h1>
	</div>

	<div class="programmes">
		<div class="programme">
			<h2>Short Series</h2>
			<p>Short series description</p>
			<a href={resolve('/short-series')}>Find out more</a>
		</div>
		<div class="programme">
			<h2>Year Series</h2>
			<p>Year series description</p>
			<a href={resolve('/year-series')}>Find out more</a>
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
		margin-top: 2rem;
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
