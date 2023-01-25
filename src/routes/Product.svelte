<div class="product">
	<img src="src/assets/icon-music.svg" alt="music icon" class="music-icon" />
	<div class="product-details">
		<p class="product-name">Annual Plan</p>
		<p class="product-price">$59.99/year</p>
	</div>
	<a href="#">Change</a>
</div>

<style lang="scss">
	.product {
		background-color: var(--blue-100);
		display: grid;
		grid-auto-flow: column;
		// grid-template-columns: 1rem, 1fr, min-content;
		padding: 1rem;
		align-items: center;
		border-radius: 1rem;
		margin-bottom: 20px;
		font-size: 0.9rem;

		&-details {
			line-height: 1.25rem;
			text-align: left;
		}
		&-name {
			font-weight: var(--fw-x-bold);
			color: var(--blue-800);
		}
		&-price {
			color: var(--blue-600);
		}
	}
	a {
		font-weight: var(--fw-x-bold);
		text-align: right;
	}
</style>
