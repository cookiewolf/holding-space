<script>
	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Holding Space for Change</h1>
	</div>

	<div class="highlight">
		<p>Facilitating better conversations, deeper connection and more meaningful change</p>
	</div>

	<div class="programmes">
		<div class="programme short">
			<h2>Holding Space Short Series</h2>
			<p>
				A 5 or 10 week accessible peer learning space for those wanting to build confidence and
				learn practical facilitation tools
			</p>
			<a href={resolve('/holding-space-short-series')}>Find out more</a>
		</div>
		<div class="programme year">
			<h2>Holding Space for Change Programme</h2>
			<p>
				A deep, 9-month journey for people holding complex spaces who want to transform their
				facilitation practice and how they lead change.
			</p>
			<a href={resolve('/holding-space-for-change')}>Find out more</a>
		</div>
	</div>

	<div class="team">
		<h2>Meet the Team</h2>
		<p>
			We’re a collective of facilitators building capacity within communities and organisations
			through inclusive, participatory, and equitable facilitation practices
		</p>
		<a href={resolve('/facilitators')}>Find out more</a>
	</div>
</main>

<style>
	.hero {
		align-items: center;
		background-image: url('$lib/assets/bubbles.webp');
		background-position: center;
		background-repeat: no-repeat;
		background-size: contain;
		display: flex;
		font-size: 3rem;
		height: 20rem;
		justify-content: center;
		width: 100%;
	}

	.highlight {
		border: 1px solid var(--grey);
		border-radius: 1rem;
		margin: auto;
		max-width: 80%;
		padding: var(--gutter-width);
		text-align: center;
	}

	.programmes {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		justify-content: space-between;
		margin: 2rem 0;
	}

	h2 {
		font-size: 1.3rem;
		margin: 0;
		padding: 0;
		margin-bottom: 1rem;
	}

	.programme {
		border-radius: 1rem;
		min-width: 0;
		padding: 1rem;
		width: 100%;
		border: 1px solid var(--grey);
		background-position: 50%;
		background-repeat: no-repeat;
		background-size: cover;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}

	.short {
		background-image: url('$lib/assets/short.webp');
	}

	.year {
		background-image: url('$lib/assets/programme.webp');
	}

	p + a {
		margin-top: 1rem;
	}

	a {
		align-self: flex-end;
	}

	.team {
		background-color: #eeeeee;
		border-radius: 1rem;
		min-width: 0;
		padding: 1rem;
		width: 100%;
		margin-bottom: 2rem;
	}

	@media (min-width: 600px) {
		.programmes {
			flex-wrap: wrap;
			flex-direction: row;
		}

		.programme {
			width: calc(50% - 0.5rem);
		}
	}
</style>
