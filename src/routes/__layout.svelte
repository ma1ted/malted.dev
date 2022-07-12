<slot />

<style>
	@font-face {
		font-family: "JetBrains Mono";
		src: url("/fonts/JetBrainsMono-Regular.woff2") format("woff2");
		font-weight: normal;
		font-style: normal;
		font-display: swap;
	}
	@font-face {
		font-family: "JetBrains Mono";
		src: url("/fonts/JetBrainsMono-Thin.woff2") format("woff2");
		font-weight: 100;
		font-style: normal;
		font-display: swap;
	}

	:root {
		--text-primary: #e0fbfc;
		--text-primary-filter: invert(93%) sepia(6%) saturate(1459%) hue-rotate(174deg) brightness(104%)
			contrast(104%);

		--bg: #293241;
		--bg-filter: invert(15%) sepia(40%) saturate(408%) hue-rotate(177deg) brightness(98%)
			contrast(90%);

		--primary: #3d5a80;
		--primary-filter: invert(28%) sepia(85%) saturate(305%) hue-rotate(173deg) brightness(97%)
			contrast(86%);

		--secondary: #98c1d9;
		--secondary-filter: invert(85%) sepia(6%) saturate(1934%) hue-rotate(171deg) brightness(89%)
			contrast(89%);

		--accent: #ee6c4d;
		--accent-filter: invert(56%) sepia(14%) saturate(6741%) hue-rotate(331deg) brightness(100%)
			contrast(87%);

		font-family: "JetBrains Mono", monospace;
		color: var(--text-primary);
		background: var(--bg);
	}

	:global(::selection) {
		background: var(--accent);
	}
</style>
