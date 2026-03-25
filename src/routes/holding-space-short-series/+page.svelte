<script>
	import Session from '../../Session.svelte';

	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Short Series</h1>
	</div>
	<div>
		<ul>
			<Session
				title="Session 1"
				date="1st April"
				time="9am"
				description="The first session in the series"
			/>
			<Session
				title="Session 2"
				date="8th April"
				time="9am"
				description="The second session in the series"
			/>
			<Session
				title="Session 3"
				date="15th April"
				time="9am"
				description="The third session in the series"
			/>
			<Session
				title="Session 4"
				date="22nd April"
				time="9am"
				description="The fourth session in the series"
			/>
		</ul>
	</div>
	<div>
		<a href={resolve('/holding-space-short-series/apply')}>Apply</a>
	</div>
</main>

<style>
	.hero {
		align-items: center;
		background-color: #eeeeee;
		display: flex;
		height: 10rem;
		justify-content: center;
		width: 100%;
	}

	ul {
		padding: 0;
		margin: 1rem 0;
	}
</style>
