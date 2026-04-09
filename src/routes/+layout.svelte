<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import Container from '../components/Container.svelte';
	import Footer from '../components/Footer.svelte';
	import NavBar from '../components/NavBar.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Holding Space</title>
</svelte:head>

<NavBar />
<Container narrow>
	{@render children?.()}
</Container>
<Footer />

<style>
	/* Box sizing rules  */
	:global(*),
	:global(*)::before,
	:global(*)::after {
		box-sizing: border-box;
	}

	/* Remove default padding */
	:global(ul),
	:global(ol),
	:global(legend) {
		padding: 0;
	}

	/* Remove default margin */
	:global(body),
	:global(h1),
	:global(h2),
	:global(h3),
	:global(h4),
	:global(p),
	:global(ul),
	:global(ol),
	:global(li),
	:global(fieldset),
	:global(figure),
	:global(figcaption),
	:global(blockquote),
	:global(dl),
	:global(dd) {
		margin: 0;
	}

	/* Set core body defaults */
	:global(body) {
		min-height: 100vh;
		scroll-behavior: smooth;
		text-rendering: optimizeSpeed;
		line-height: 1.5;
	}

	/* Remove list styles on ul, ol elements */
	:global(ul),
	:global(ol) {
		list-style: none;
	}

	/* Make images easier to work with */
	:global(img) {
		max-width: 100%;
		display: block;
	}

	/* Inherit fonts for inputs and buttons */
	:global(input),
	:global(button),
	:global(textarea),
	:global(select) {
		font: inherit;
	}

	/* Remove all animations and transitions for people that prefer not to see them */
	@media (prefers-reduced-motion: reduce) {
		:global(*) {
			animation-duration: 0.01ms !important;
			animation-iteration-count: 1 !important;
			transition-duration: 0.01ms !important;
			scroll-behavior: auto !important;
		}
	}

	/* Global defaults */

	@font-face {
		font-family: 'PlexSans';
		src: url('/fonts/PlexSans.ttf') format('truetype');
		font-style: normal;
		font-display: swap;
	}
	@font-face {
		font-family: 'PlexSans';
		src: url('/fonts/PlexSans-Italic.ttf') format('truetype');
		font-style: italic;
		font-display: swap;
	}

	@font-face {
		font-family: 'PlexSerif';
		src: url('/fonts/PlexSerif-SemiBold.ttf') format('truetype');
		font-weight: 600;
		font-style: normal;
		font-display: swap;
	}

	@font-face {
		font-family: 'PlexSerif';
		src: url('/fonts/PlexSerif-SemiBoldItalic.ttf') format('truetype');
		font-weight: 600;
		font-style: italic;
		font-display: swap;
	}

	:global(body) {
		color: var(--text);
		display: flex;
		font-family:
			PlexSans,
			system-ui,
			-apple-system,
			BlinkMacSystemFont,
			'Segoe UI',
			Roboto,
			Oxygen,
			Ubuntu,
			Cantarell,
			'Open Sans',
			'Helvetica Neue',
			sans-serif;
		font-size: 100%;
		flex-direction: column;

		--gutter-width: 1rem;

		--orange: #ff9300;
		--orange-light: #fcd092;
		--pink: #ff4989;
		--pink-dark: #eb0052;
		--pink-light: #e193af;
		--red: #ff2500;
		--grey: #eeeeee;
		--text: #16161d;
	}

	:global(body.menu-open) {
		overflow: hidden;
	}

	:global(a) {
		color: var(--pink-dark);
	}

	@media (min-width: 600px) {
		:global(body) {
			--gutter-width: 2rem;
		}
	}

	:global(h1),
	:global(h2),
	:global(h3),
	:global(h4),
	:global(h5),
	:global(h6) {
		font-family: PlexSerif, sans;
		font-size: 100%;
		font-style: normal;
		font-weight: bold;
	}
</style>
