<script>
	import Description from '../../../components/Description.svelte';
</script>

<main>
	<div class="hero">
		<h1>Apply for Holding Space For Change</h1>
	</div>
	<div>
		<form name="holding-space-for-change" method="POST" data-netlify="true" data-sveltekit-reload>
			<input type="hidden" name="form-name" value="holding-space-for-change" />

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
				<fieldset aria-describedby="contribution-description">
					<legend>What contribution would you like to make to the programme? *</legend>
					<Description id="contribution-description">
						(Your answer to this will not affect your eligibility for the programme)
					</Description>
					<label>
						<input type="radio" name="contribution" value="Solidarity2000" required />
						Solidarity tier - £2,000
					</label>

					<label>
						<input type="radio" name="contribution" value="Standard1400" required />
						Standard tier - £1,400
					</label>

					<label>
						<input type="radio" name="contribution" value="Supported800" required />
						Supported tier - £800
					</label>
				</fieldset>
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
				<label for="help-in-work-life">
					How are you hoping this programme will help you in your work or life?<br />(Up to 300
					words)
				</label>
				<textarea rows="6" id="help-in-work-life" name="help-in-work-life"></textarea>
			</div>

			<div class="question">
				<label for="course-principles">
					Provide an example of how you already exhibit one or more of the course principles in your
					life or work.<br />(Up to 300 words)
				</label>
				<textarea rows="6" id="course-principles" name="course-principles"></textarea>
			</div>

			<div class="question">
				<label for="access-requirements"
					>What might help you to learn during this programme?<br />(any access requirements / any
					suggestions for support or structure)</label
				>
				<textarea rows="6" id="access-requirements" name="access-requirements"></textarea>
			</div>

			<button type="submit">Apply</button>
		</form>
	</div>
</main>

<style>
	.hero {
		background-image: url('$lib/assets/orange.webp');
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
