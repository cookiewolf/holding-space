<script lang="ts">
	let { title, date, time, description } = $props();
</script>

<li>
	<div>
		<h2>
			{title}
		</h2>

		<p>
			{date} @ {time}
		</p>
		<p>
			{description}
		</p>
	</div>
</li>

<style>
	li {
		background-color: #eeeeee;
		border-radius: 1rem;
		list-style: none;
		margin: 1rem 0;
		max-width: 600px;
		min-width: 0;
		padding-block: 0.5rem;
		padding-inline: 1rem;
		width: 100%;
	}
</style>
