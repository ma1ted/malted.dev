<script>
	import Colours from "./components/_colours.svelte";
	import Typeography from "./components/_typeography.svelte";
</script>

<main>
	<h1>Design guidelines</h1>

	<Colours />
	<Typeography />
</main>

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
</style>
