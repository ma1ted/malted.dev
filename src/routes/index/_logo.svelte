<div id="root">
	<div id="vertical">
		<div />
		<div />
		<div />
	</div>
	<div id="horizontal">
		<div />
		<div />
		<div />
	</div>
</div>

<style>
	* {
		--size: 2;
		--width: calc(1rem * var(--size));
		--height: calc(6rem * var(--size));
	}

	#root {
		position: relative;
		height: var(--height);
	}

	#horizontal {
		flex-direction: column;
		bottom: 0;
	}
	#vertical {
		flex-direction: row;
	}
	#horizontal,
	#vertical {
		display: flex;
		gap: var(--width);
		position: absolute;
	}

	#horizontal > div {
		width: var(--height);
		height: var(--width);
	}
	#vertical > div {
		width: var(--width);
		height: var(--height);
	}

	#horizontal > div,
	#vertical > div {
		background: var(--accent);
		border-radius: calc(var(--width) / 2);
	}
</style>
