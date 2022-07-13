<script>
	export let primary;
	export let placeholder = "";
</script>

<input class:primary type="text" {placeholder} />

<style>
	input {
		background-color: var(--bg);
		color: var(--text-primary);
		border: 2px solid var(--secondary);
		border-radius: var(--panel-border-radius);
		padding: 0.5rem;
		transition: border 0.2s ease, filter 0.1s ease;
	}
	input:hover {
		filter: brightness(1.2);
	}
	input:focus {
		outline: none;
		border: 2px solid var(--accent);
		filter: brightness(1.2);
	}

	.primary {
		background-color: var(--primary);
	}
</style>
