<script>
	const curve = 1.2;
	const line = 0.5;
	const handle = 1;
	const resolution = 50;
	const background = "rgb(41, 50, 65)";
	const y = 5;
	const z = 30;

	const src = `
https://curve.malted.dev?
curve=${curve}&
line=${line}&
handle=${handle}&
resolution=${resolution}&
background=${background}&
y=${y}&
z=${z}`;
</script>

<iframe {src} title="Bézier Curves" />

<style>
	iframe {
		width: 30rem;
		height: 20rem;
		border: 3px solid var(--primary);
		z-index: 100;
	}
</style>
