<script>
	import Colours from "./views/_colours.svelte";
	import Typography from "./views/_typography.svelte";
	import Buttons from "./views/_buttons.svelte";
</script>

<main>
	<h1>Design guidelines</h1>
	<Colours />
	<Typography />
	<Buttons />
</main>

<footer />

<style>
	* {
		margin: 0;
	}

	main {
		margin: 2rem;
		display: flex;
		flex-direction: column;
		gap: 3rem;
	}

	h1 {
		color: var(--text-primary);
	}
</style>
