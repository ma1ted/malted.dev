<script>
	import Colours from "./views/colours.svelte";
	import Typography from "./views/typography.svelte";
	import Buttons from "./views/buttons.svelte";
	import Inputs from "./views/inputs.svelte";
</script>

<main>
	<h1>Design guidelines</h1>
	<Colours />
	<Typography />
	<Buttons />
	<Inputs />
</main>

<footer />

<style>
	* {
		margin: 0;
	}

	:global(details.input-description) {
		cursor: pointer;
		user-select: none;
	}

	:global(details.input-description > p) {
		font-size: 0.8rem;
		font-weight: 100;
	}

	main {
		margin: 2rem;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 3rem;
	}

	h1 {
		color: var(--text-primary);
	}
</style>
