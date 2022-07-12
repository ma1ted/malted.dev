<script>
	import Colour from "./_colour.svelte";
</script>

<section id="colours">
	<Colour name="Background" background="#293241" />
	<Colour name="Primary" background="#3d5a80" />
	<Colour name="Secondary" background="#98c1d9" />
	<Colour name="Text primary" background="#e0fbfc" />
	<Colour name="Accent" background="#ee6c4d" />
</section>

<style>
	#colours {
		display: flex;
		gap: 2rem;
	}
</style>
