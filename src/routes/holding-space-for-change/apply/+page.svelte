<script>
	import Description from '../../../Description.svelte';
</script>

<main>
	<div class="hero">
		<h1>Apply for Holding Space For Change</h1>
	</div>
	<div>
		<form name="holding-space-for-change" method="POST" data-netlify="true" data-sveltekit-reload>
			<input type="hidden" name="form-name" value="holding-space-for-change" />

			<label>
				What's your name and pronouns?
				<br />
				<input type="text" name="name" />
			</label>

			<br />

			<label
				>What's your email address?
				<br />
				<input type="email" name="email" />
			</label>

			<br />

			<fieldset aria-describedby="contribution-description">
				<legend>What contribution would you like to make to the programme?</legend>
				<Description id="contribution-description">
					(Your answer to this will not affect your eligibility for the programme)
				</Description>
				<label>
					<input type="radio" name="choice" value="Solidarity2000" />
					Solidarity tier - £2,000
				</label>
				<br />

				<label>
					<input type="radio" name="choice" value="Standard1400" />
					Standard tier - £1,400
				</label>
				<br />

				<label>
					<input type="radio" name="choice" value="Supported800" />
					Supported tier - £800
				</label>
			</fieldset>

			<br />

			<label for="your-identity"> How would you describe your identity?</label>
			<Description id="identitity-description">
				This is an optional question but your responses will help me to understand the diversity of
				experience and perspective present within the room, and consider what this means for
				potential power dynamics and experiences of the space
			</Description>

			<textarea
				rows="4"
				id="your-identity"
				name="your-identity"
				aria-describedby="identitity-description"
				placeholder="e.g. white autistic woman in her mid-40s"
			>
			</textarea>

			<br />

			<label for="your-identity"
				>How are you hoping this programme will help you in your work or life? (Up to 300 words)
			</label>
			<br />
			<textarea
				rows="4"
				id="your-identity"
				name="your-identity"
				aria-describedby="identitity-description"
			>
			</textarea>
			<br />

			<label for="your-identity"
				>Provide an example of how you already exhibit one or more of the course principles in your
				life or work. (Up to 300 words)</label
			>
			<br />
			<textarea
				rows="4"
				id="your-identity"
				name="your-identity"
				aria-describedby="identitity-description"
			>
			</textarea>
			<br />

			<label for="your-identity"
				>What might help you to learn during this programme? (any access requirements / any
				suggestions for support or structure)</label
			>
			<br />
			<textarea
				rows="4"
				id="your-identity"
				name="your-identity"
				aria-describedby="identitity-description"
			>
			</textarea>
			<br />

			<button type="submit">Send</button>
		</form>
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

	label {
		margin-top: 1rem;
		display: block;
	}

	input[type='text'] {
		width: 100%;
		max-width: 300px;
	}

	textarea {
		width: 100%;
		max-width: 600px;
	}
</style>
