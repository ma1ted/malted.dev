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
	<p class="desc">
		The default and primary buttons' background colours have been brightened by 30% from their
		respective reference colours to ensure their visibility against backgrounds of the same colours,
		with the exception being the warn variant, which is not brightened at all in its default state
		as it should not be used against a background of the same colour.
	</p>
	<p class="desc">
		Upon hovering, the buttons' brightnesses are increased by 30% to not only provide feedback to
		the user but reinforce that the elements are interactable too.
	</p>
	<p class="desc">
		When the buttons are in their active state, i.e. are being pressed, their sizes are scaled down
		by 10%, along with the colours being brightened by another 30% to provide satisyfing feedback to
		the user.
	</p>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	#display {
		display: flex;
		flex-direction: row;
		gap: 2rem;
		width: fit-content;
	}
	#display > div {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		border-radius: 14px;
		padding: 1rem;
		width: fit-content;
	}

	#normal-backdrop {
		border: 2px solid var(--primary);
	}
	#primary-backdrop {
		background-color: var(--primary);
	}
	#secondary-backdrop {
		background-color: var(--secondary);
	}

	.desc {
		font-weight: 100;
		font-size: 0.8rem;
		margin: 0;
	}
</style>
