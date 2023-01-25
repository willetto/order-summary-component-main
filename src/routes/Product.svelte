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
		grid-template-columns: max-content 1fr min-content;
		gap: 1rem;
		padding: 1rem;
		align-items: center;
		border-radius: 1rem;
		margin-bottom: 20px;
		font-size: 0.9rem;
		@media screen and (min-width: 900px) {
			padding: 25px;
			margin-bottom: 25px;
		}
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
		&:hover {
			cursor: pointer;
			opacity: 0.7;
			text-decoration: none;
		}
	}
</style>
