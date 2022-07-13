<script>
	import Button from "../components/_button.svelte";
</script>

<section>
	<h2>Buttons</h2>
	<div id="display">
		<div id="normal-backdrop">
			<Button>Default button</Button>
			<Button primary>Primary button</Button>
			<Button warn>Warning button</Button>
		</div>
		<div id="primary-backdrop">
			<Button>Default button</Button>
			<Button primary>Primary button</Button>
			<Button warn>Warning button</Button>
		</div>
		<div id="secondary-backdrop">
			<Button>Default button</Button>
			<Button primary>Primary button</Button>
			<Button warn>Warning button</Button>
		</div>
	</div>

	<details class="input-description">
		<summary>Details</summary>
		<p>
			The default and primary buttons' background colours have been brightened by 20% from their
			respective reference colours to ensure their visibility against backgrounds of the same
			colours, with the exception being the warn variant, which is not brightened at all in its
			default state as it should not be used against a background of the same colour.
		</p>
		<p>
			Upon hovering, a button's brightness is increased by 20% to not only provide feedback to the
			user but reinforce that the element is interactable too.
		</p>
		<p>
			When a button is in its active state, i.e. is being pressed, its size is scaled down by 10%,
			along with its colours being brightened by another 20% to provide satisyfing feedback to the
			user.
		</p>
	</details>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	#display {
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;
	}

	#display > div {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		border-radius: 14px;
		padding: 2rem;
	}

	#normal-backdrop {
		border: 1px solid var(--primary);
	}
	#primary-backdrop {
		background-color: var(--primary);
	}
	#secondary-backdrop {
		background-color: var(--secondary);
	}
</style>
