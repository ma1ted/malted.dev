<script>
	export let checkbox;
	export let checked;
	export let name;

	export let primary;
	export let placeholder = "";
</script>

{#if checkbox}
	<input type="checkbox" class="checkbox" {checked} {name} />
{:else}
	<input class:primary type="text" {placeholder} {name} />
{/if}

<style>
	input[type="checkbox"] {
		width: 1rem;
		height: 1rem;
		accent-color: var(--accent);
	}
	input[type="text"] {
		background-color: var(--bg);
		color: var(--text-primary);
		border: 2px solid var(--secondary);
		border-radius: var(--panel-border-radius);
		padding: 0.5rem;
		transition: border 0.2s ease, filter 0.1s ease;
	}
	input[type="text"]:hover {
		filter: brightness(1.2);
	}
	input[type="text"]:focus {
		outline: none;
		border: 2px solid var(--accent);
		filter: brightness(1.2);
	}

	input[type="text"].primary {
		background-color: var(--primary);
	}
</style>
