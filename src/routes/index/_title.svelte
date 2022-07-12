<script>
	import { onMount } from "svelte";
	import { fade, fly } from "svelte/transition";

	const endString = "malted.dev";
	const startScramble = 10;
	const wrongIterations = 3;

	let titleVisible;
	let subtitleVisible;
	let target = "";

	onMount(async () => {
		titleVisible = true;
		for (let i = 0 - startScramble; i < endString.length * wrongIterations; i++) {
			for (let c in endString) {
				if (i / wrongIterations >= c) target += endString[c];
				else if (!endString[c].match(/[a-zA-Z]/)) target += endString[c];
				else target += String.fromCharCode(Math.floor(Math.random() * 26) + 97);
			}
			await new Promise((r) => setTimeout(r, 30));
			target = "";
		}
		target = endString;
		subtitleVisible = true;
	});
</script>

<div id="container">
	{#if titleVisible}
		<h1 in:fade>{target}</h1>
	{/if}
	{#if subtitleVisible}
		<div id="sub">
			<h2 in:fly={{ y: -50, duration: 500 }}>Coming soon.</h2>
			<div id="links" in:fly={{ y: -100, duration: 500 }}>
				<a href="https://github.com/ma1ted">
					<img src="/icons/github.svg" alt="GitHub" />
				</a>
				<a href="https://twitter.com/ma1ted">
					<img src="/icons/twitter.svg" alt="Twitter" />
				</a>
			</div>
		</div>
	{/if}
</div>

<style>
	#container {
		display: flex;
		flex-direction: column;
		gap: 2rem;
		margin-top: 15rem;
		margin-left: 4rem;
	}
	@media (max-width: 600px) {
		#container {
			margin-top: 12rem;
			margin-left: 1rem;
		}
		h1 {
			font-size: 2.5rem !important;
		}
	}

	h1 {
		font-size: 5rem;
		margin: 0;
	}

	h2 {
		font-weight: 100;
		font-size: 2rem;
	}

	#sub {
		display: flex;
		flex-direction: column;
		gap: 0.8rem;
	}

	#links {
		display: flex;
		gap: 1.5rem;
	}
	#links img {
		width: 2rem;
		filter: var(--text-primary-filter);
	}
</style>
