<script>
	export let name = "[PLACEHOLDER]";
	export let background = "#ff00ff";
</script>

<div class="colour">
	<div class="swatch" style:background />
	<p>{name}</p>
	<p class="hex">{background}</p>
</div>

<style>
	.swatch {
		height: 6rem;
		width: 6rem;
		border-radius: 6px;
		transition: box-shadow 0.1s ease;
	}
	.swatch:hover {
		box-shadow: 0.5rem 0.5rem var(--secondary);
	}

	.hex {
		color: var(--secondary);
		font-weight: 100;
	}
</style>
