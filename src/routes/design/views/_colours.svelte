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
	#colours {
		display: flex;
		gap: 3rem;
		border-radius: 14px;
	}
</style>
