<script>
	import { resolve } from '$app/paths';
</script>

<main>
	<div class="hero">
		<h1>Holding Space Series</h1>
	</div>

	<div class="page">
		<a href={resolve('/holding-space-short-series/apply')} class="button-link right">Register</a>

		<p>
			The <b>Holding Space Series</b> is a simple, accessible 5 or 10 week programme for anyone who wants
			to build their confidence and practical skills in facilitation.
		</p>

		<p>
			You might be seeking a hands-on introduction, or perhaps you’d just appreciate regular space
			with other facilitators to experiment with new tools and techniques. Each session you’ll be
			guided through an exercise, experience it together as a group, and then reflect on how it can
			be adapted and applied in your own context.
		</p>

		<p>Across the series, you’ll:</p>

		<ul>
			<li>Learn and practise facilitation exercises you can use straight away</li>
			<li>Explore how to work with real-life group dynamics and challenges</li>
			<li>Reflect on your own instincts, habits, and approach</li>
			<li>Build a small toolkit of practices to support how you hold space</li>
		</ul>

		<p>
			Sessions take place weekly on Zoom (1 or 2 hours depending on the cohort), with additional
			reflection prompts and materials shared to help you integrate your learning over time.
		</p>

		<p>
			You’re welcome to join individual sessions, but those who attend regularly often find the
			experience more rewarding as relationships and learning deepen across the group.
		</p>

		<p>
			This series can stand alone as a practical introduction, or act as a stepping stone into the
			more in-depth <b>Holding Space for Change</b> programme — where you’ll deepen your practice over
			a longer, cohort-based journey.
		</p>

		<p>
			This series is offered on a pay-what-you-can basis, with a suggested contribution of £100 to
			support the time, care, and facilitation involved, while ensuring cost is not a barrier to
			participation.
		</p>

		<p>The next series will kick off on the following dates:</p>

		<ul>
			<li>Tuesdays 12.30 - 1.30 BST from 21st April to 23rd June (10 week programme)</li>
			<li>Fridays 10-12 BST from 8th May - 5th June (5 week programme)</li>
		</ul>

		<a href={resolve('/holding-space-short-series/apply')} class="button-link">Register</a>

		<p class="highlight">
			“Participating in the Holding Space programme was an enriching and collaborative experience. I
			felt encouraged to show up as my whole self when taking on the facilitating role, and I loved
			that we tried out techniques in real time each week. Since finishing the course, I have used
			many of these new tools in my facilitation work - most recently creating and running a
			visioning session for my co-op. I felt more confident in holding space in this way, and it was
			a lot of fun trying out different activities with the group. The techniques that Ray taught
			unlocked creativity and enthusiasm in the team, and together we came up with a strong set of
			shared values to centre in our work.” - Jade, Catalyst Collective
		</p>
	</div>
</main>

<style>
	.hero {
		align-items: center;
		background-image: url('$lib/assets/short.webp');
		background-position: center;
		background-repeat: no-repeat;
		background-size: contain;
		display: flex;
		font-size: 3rem;
		height: 14rem;
		justify-content: center;
		width: 100%;
	}

	p + p {
		margin-top: 1rem;
	}

	ul {
		list-style: disc;
		list-style-position: inside;
		margin-bottom: 1rem;
	}

	.page {
		display: flex;
		flex-direction: column;
	}

	.button-link {
		align-self: center;
		background-color: var(--pink);
		border-radius: 4px;
		color: var(--text);
		display: inline-block;
		font-size: 1.2rem;
		margin-top: 2rem;
		outline: 2px solid transparent;
		padding: 0.5rem 1rem;
		text-decoration: none;
	}

	.button-link.right {
		align-self: flex-end;
		margin-top: 0;
		margin-bottom: 1rem;
	}

	.button-link:hover {
		outline: 2px solid var(--orange-light);
	}

	.highlight {
		background-color: var(--orange-light);
		border-radius: 1rem;
		margin: 1rem 0;
		padding: 1rem;
	}
</style>
