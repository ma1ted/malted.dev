<script>
	export let primary;
	export let warn;
</script>

<button class:primary class:warn>
	<slot />
</button>

<style>
	button {
		border: none;
		border-radius: var(--panel-border-radius);
		padding: 0.5rem 1rem;
		cursor: pointer;
		background-color: var(--bg);
		filter: brightness(1.2);
		transition: filter 0.1s ease, transform 0.03s ease;
	}
	button:hover {
		filter: brightness(1.4);
	}
	button:active {
		filter: brightness(1.6);
		transform: scale(0.9);
	}

	.primary {
		background-color: var(--primary);
	}

	.warn {
		background-color: var(--accent);
		filter: none;
	}
	.warn:hover {
		filter: brightness(1.2);
	}
	.warn:active {
		filter: brightness(1.4);
		transform: scale(0.6);
	}
</style>
