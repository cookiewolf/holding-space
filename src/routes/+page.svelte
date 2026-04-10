<script>
	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Holding Space Collective</h1>

		<div class="highlight">
			<p>Facilitating better conversations, deeper connection and more meaningful change</p>
		</div>
	</div>

	<div class="programmes">
		<div class="programme short">
			<div class="clear">
				<a href={resolve('/holding-space-short-series')} class="headinglink">
					<h2>Holding Space Short Series</h2>
				</a>
			</div>
			<div class="glass">
				<p>
					A 5 or 10 week accessible peer learning space for those wanting to build confidence and
					learn practical facilitation tools.
				</p>
				<a href={resolve('/holding-space-short-series')}>Find out more</a>
			</div>
		</div>

		<div class="programme year">
			<div class="clear">
				<a href={resolve('/holding-space-for-change')} class="headinglink">
					<h2>Holding Space for Change Programme</h2>
				</a>
			</div>
			<div class="glass">
				<p>
					A deep, 9-month journey for people holding complex spaces who want to transform their
					facilitation practice and how they lead change.
				</p>
				<a href={resolve('/holding-space-for-change')}>Find out more</a>
			</div>
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
		background-size: cover;
		display: flex;
		flex-direction: column;
		font-size: 2.5rem;
		height: 16rem;
		justify-content: center;
		text-align: center;
		width: 100%;
	}

	h1 {
		margin-top: 2rem;
	}

	@media (min-width: 600px) {
		.hero {
			height: 450px;
			font-size: 3rem;
			background-size: contain;
		}

		h1 {
			margin-top: 8rem;
		}
	}

	.highlight {
		background-color: #ffffff80;
		border-radius: 1rem;
		font-size: 1rem;
		margin: auto 1rem;
		max-width: 400px;
		padding: 1rem;
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
		font-size: 1.8rem;
		margin: 0;

		margin-bottom: 1rem;
	}

	.headinglink {
		color: var(--text);
		text-decoration: none;
	}

	.programme {
		background-position: 50% 50%;
		background-repeat: no-repeat;
		background-size: 150%;
		border-radius: 1rem;
		border: 1px solid var(--grey);
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		min-width: 0;
		width: 100%;
	}

	.programme h2 {
		padding: 1rem;
	}

	.clear {
		height: 12rem;
	}

	.glass {
		background-color: #ffffff80;
		padding: 1rem;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		height: 10rem;
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
		border-radius: 1rem;
		border: 1px solid var(--grey);
		min-width: 0;
		padding: 1rem;
		width: 100%;
		margin-bottom: 2rem;
	}

	.team > a {
		display: inline-block;
		margin-top: 1rem;
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
