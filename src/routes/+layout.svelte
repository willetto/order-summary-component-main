<slot />

<style>
	@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@500;700;900&display=swap');

	:root {
		--blue-100: hsl(225, 100%, 98%);
		--blue-200: hsl(225, 100%, 94%);
		--blue-400: hsl(245, 75%, 52%);
		--blue-600: hsl(224, 23%, 55%);
		--blue-800: hsl(223, 47%, 23%);
	}
	:global(body) {
		background-image: url(../assets/pattern-background-mobile.svg);
		background-color: var(--blue-200);
		background-repeat: no-repeat;
		background-size: 100% auto;
		font-family: 'Red Hat Display', sans-serif;
		font-weight: 500;
	}

	@media (min-width: 900px) {
		:global(body) {
			background-image: url(../assets/pattern-background-desktop.svg);
		}
	}
</style>
