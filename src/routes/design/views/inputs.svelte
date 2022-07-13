<script>
	import Input from "../components/_input.svelte";
</script>

<section>
	<h2>Inputs</h2>
	<div id="buttons">
		<div id="normal-backdrop">
			<Input placeholder="Default input" />
		</div>
		<div id="primary-backdrop">
			<Input primary placeholder="Primary input" />
		</div>
	</div>

	<details class="input-description">
		<summary>Details</summary>
		<p>A text input should not be used against a secondary background.</p>
		<p>
			Upon hovering, an input's brightness is increased by 20% to not only provide feedback to the
			user but reinforce that the element is interactable too.
		</p>
		<p>
			When the input is in its active state, i.e. is focussed, it gains an accented border to
			clearly communicate that the element is focussed.
		</p>
	</details>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 1rem;
	}
	#buttons {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		gap: 2rem;
	}

	#buttons > div {
		padding: 2rem;
		border-radius: 14px;
	}

	#normal-backdrop {
		border: 1px solid var(--primary);
	}
	#primary-backdrop {
		background-color: var(--primary);
	}
</style>
