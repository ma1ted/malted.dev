<script>
	import Colour from "../components/_colour.svelte";
</script>

<section>
	<h2>Colours</h2>
	<div id="colours">
		<Colour name="Background" background="#293241" />
		<Colour name="Primary" background="#3d5a80" />
		<Colour name="Secondary" background="#98c1d9" />
		<Colour name="Text" background="#e0fbfc" />
		<Colour name="Accent" background="#ee6c4d" />
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	#colours {
		display: flex;
		gap: 2rem;
		flex-wrap: wrap;
	}
</style>
