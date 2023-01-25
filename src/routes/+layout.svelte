<main>
	<slot />
</main>

<footer class="attribution">
	Challenge by
	<a href="https://www.frontendmentor.io?ref=challenge" target="_blank"> Frontend Mentor</a>. Coded
	by
	<a href="https://www.treywilletto.com" target="_blank">Trey Willetto</a>.
</footer>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@500;700;900&display=swap');

	:root {
		--blue-100: hsl(225, 100%, 98%);
		--blue-200: hsl(225, 100%, 94%);
		--blue-400: hsl(245, 75%, 52%);
		--blue-600: hsl(224, 23%, 55%);
		--blue-800: hsl(223, 47%, 23%);
		--fw-base: 500;
		--fw-bold: 700;
		--fw-x-bold: 900;
	}
	:global(body) {
		background-image: url(../assets/pattern-background-mobile.svg);
		background-color: var(--blue-200);
		background-repeat: no-repeat;
		background-size: 100% auto;
		font-family: 'Red Hat Display', sans-serif;
		font-weight: var(--fw-base);
	}
	main {
		display: grid;
		place-items: center;
		margin-top: 70px;
	}
	.attribution {
		font-size: 11px;
		text-align: center;
		margin-top: 3rem;
	}
	.attribution a {
		color: hsl(228, 45%, 44%);
	}
	@media (min-width: 900px) {
		:global(body) {
			background-image: url(../lib/assets/pattern-background-mobile.svg);
		}
		main {
			margin-top: 90px;
		}
	}

	:global(*, *::before, *::after) {
		box-sizing: border-box;
	}
	:global(body, h1, h2, h3, h4, p, figure, blockquote, dl, dd) {
		margin: 0;
	}
	:global(img, picture) {
		max-width: 100%;
		display: block;
	}
	:global(input, button, textarea, select) {
		font: inherit;
	}
</style>
