<script>
	import Description from '../../../components/Description.svelte';
</script>

<main>
	<div class="hero">
		<h1>Apply for Holding Space Short Series</h1>
	</div>
	<div>
		<form name="holding-space-short-series" method="POST" data-netlify="true" data-sveltekit-reload>
			<input type="hidden" name="form-name" value="holding-space-short-series" />

			<div class="question">
				<fieldset>
					<legend>Which cohort would you like to sign up to be part of? *</legend>
					<label>
						<input type="radio" name="cohort" value="21st April to 23rd June" required />
						21st April to 23rd June
					</label>

					<label>
						<input type="radio" name="cohort" value="8th May - 5th June" required />
						8th May - 5th June
					</label>
				</fieldset>
			</div>

			<div class="question">
				<label>
					What's your name and pronouns? *
					<input type="text" name="name" required />
				</label>
			</div>

			<div class="question">
				<label
					>What's your email address? *
					<input type="email" name="email" required />
				</label>
			</div>

			<div class="question">
				<label for="your-identity"> How would you describe your identity? </label>
				<Description id="identitity-description">
					This is an optional question but your responses will help me to understand the diversity
					of experience and perspective present within the room, and consider what this means for
					potential power dynamics and experiences of the space
				</Description>
				<textarea
					rows="5"
					id="your-identity"
					name="your-identity"
					aria-describedby="identitity-description"
					placeholder="e.g. white autistic woman in her mid-40s"
				></textarea>
			</div>

			<div class="question">
				<label for="facilitating-confidence">
					How confident do you feel currently in facilitating group discussions?(1-5)
				</label>
				<textarea rows="6" id="facilitating-confidence" name="facilitating-confidence"></textarea>
			</div>

			<div class="question">
				<label for="facilitating-confidence-expanded"> Please expand on your answer </label>
				<textarea
					rows="6"
					id="facilitating-confidence-expanded"
					name="facilitating-confidence-expanded"
				></textarea>
			</div>

			<div class="question">
				<label for="experiences"
					>Is there anything else you'd like me to know about you and your experiences before the
					first session?</label
				>
				<textarea rows="6" id="experiences" name="experiences"></textarea>
			</div>

			<div class="question">
				<fieldset>
					<legend
						>Would you also like to sign up to my occasional newsletter sharing other workshops and
						events from me or my network?</legend
					>
					<label>
						<input type="radio" name="newsletter" value="Yes" />
						Yes
					</label>

					<label>
						<input type="radio" name="newsletter" value="No" />
						No
					</label>
				</fieldset>
			</div>

			<button type="submit">Apply</button>
		</form>
	</div>
</main>

<style>
	.hero {
		background-image: url('$lib/assets/short.webp');
		background-position: center;
		background-repeat: no-repeat;
		background-size: contain;
		align-items: center;
		display: flex;
		font-size: 2rem;
		height: 14rem;
		justify-content: center;
		width: 100%;
	}

	@media (min-width: 600px) {
		.hero {
			font-size: 3rem;
		}
	}

	form {
		background-color: var(--orange-light);
		border-radius: var(--gutter-width);
		display: flex;
		flex-direction: column;
		margin-block: var(--gutter-width);
		margin: auto;
		margin-bottom: 2rem;
		max-width: 600px;
		padding: 1rem var(--gutter-width);
	}

	.question {
		margin-bottom: 1.5rem;
	}

	label {
		display: block;
	}

	input[type='text'],
	input[type='email'] {
		border-radius: 4px;
		border: 1px solid var(--text);
		height: 2rem;
		margin-top: 0.25rem;
		max-width: 400px;
		padding-inline: 0.5rem;
		width: 100%;
	}

	input[type='radio'],
	input[type='email'] {
		margin-left: 0;
		accent-color: var(--pink);
		margin-top: 0.75rem;
	}

	fieldset {
		border: 0;
		padding: 0;
	}

	textarea {
		border-radius: 4px;
		max-width: 600px;
		width: 100%;
	}

	button {
		background: #ffffff;
		border-radius: 4px;
		border: 1px solid var(--text);
		cursor: pointer;
		font-size: 1.2rem;
		outline: 2px solid transparent;
		padding: 0.5rem 1rem;
		margin-left: auto;
	}

	button:hover {
		outline: 2px solid var(--pink);
	}

	:focus-visible {
		outline: 3px solid var(--pink);
	}
</style>
