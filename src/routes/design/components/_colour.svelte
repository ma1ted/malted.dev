<script>
	export let name = "[PLACEHOLDER]";
	export let background = "#ff00ff";
</script>

<div class="colour" style="--col:{background}">
	<div class="swatch" style:background>
		<div class="shadow" style:background />
	</div>
	<p class="name">{name}</p>
	<p class="hex">{background}</p>
</div>

<style>
	.swatch,
	.shadow {
		position: relative;
		height: 6rem;
		width: 6rem;
		border-radius: var(--panel-border-radius);
	}
	.shadow {
		filter: brightness(0.75);
		transform: translate(8%, 8%);
		z-index: -1;
	}

	.name {
		margin: 0;
		margin-top: 1rem;
	}

	.hex {
		color: var(--secondary);
		font-size: 0.8rem;
		font-weight: 100;
		margin: 0;
	}
</style>
