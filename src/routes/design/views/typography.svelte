<section>
	<h2>Typeface</h2>
	<div id="fonts">
		<div id="normal">
			<h3>JetBrains Mono Regular</h3>
			<p>Used for body text</p>
			<p>ABCDEFGHIJKLMNOPQRSTUVWXYZ</p>
			<p>abcdefghijklmnopqrstuvwxyz</p>
			<p>1234567890-!"@£$%^&*()[]</p>
		</div>
		<div id="thin">
			<h3>JetBrains Mono Thin</h3>
			<p>Used for subtitle text</p>
			<p>ABCDEFGHIJKLMNOPQRSTUVWXYZ</p>
			<p>abcdefghijklmnopqrstuvwxyz</p>
			<p>1234567890-!"@£$%^&*()[]</p>
		</div>
	</div>
	<a id="font-link" href="https://www.jetbrains.com/lp/mono/">
		<img src="/icons/link.svg" alt="link" />
		<p>jetbrains.com/mono</p>
	</a>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	#fonts {
		display: flex;
		flex-wrap: wrap;
		gap: 3rem;
	}

	h3 {
		margin-top: 0;
	}
	#thin * {
		font-weight: 100;
	}

	#fonts > div > p:last-child {
		margin-bottom: 0;
	}

	#font-link {
		display: flex;
		align-items: center;
		gap: 0.5rem;
		width: fit-content;
		text-decoration: none;
		border: 2px solid var(--primary);
		border-radius: var(--panel-border-radius);

		padding: 0.5rem;
	}

	#font-link img {
		filter: invert(100%);
		width: 20px;
	}
	#font-link p {
		font-size: 0.7rem;
		font-weight: 100;
		margin: 0;
	}
</style>
