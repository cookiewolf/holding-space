<script>
	import Container from './Container.svelte';
</script>

<footer>
	<Container>
		<div class="footer-items">
			<p>Holding Space Collective</p>
			<a href="mailto:hello@holdingspacetogether.co.uk">hello@holdingspacetogether.co.uk</a>
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
		min-height: 8rem;
		width: 100%;
	}

	.footer-items {
		align-items: center;
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;
		justify-content: center;
	}

	@media (min-width: 600px) {
		.footer-items {
			justify-content: space-between;
		}
	}

	p {
		color: #ffffff;
		font-family: PlexSerif, serif;
	}

	a {
		color: #ffffff;
	}
</style>
