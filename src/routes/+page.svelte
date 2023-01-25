<script>
	import Product from './Product.svelte';
	import hero from '$lib/assets/illustration-hero.svg';
</script>

<div class="product-card">
	<div class="hero-img">
		<img src={hero} alt="Smiling, dancing girl listing to music in headphones" />
	</div>
	<div class="order-summary">
		<h1>Order Summary</h1>
		<p>
			You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you
			like!
		</p>
		<Product />
		<button>Proceed to Payment</button>
		<a class="cancel">Cancel Order</a>
	</div>
</div>

<style>
	.product-card {
		width: 325px;
		border-radius: 20px;
		overflow: hidden;
		box-shadow: 0 15px 35px -20px hsla(243, 60%, 52%, 0.7);
	}
	.order-summary {
		background-color: white;
		padding-block: 35px;
		padding-inline: 25px;
		text-align: center;
	}
	.order-summary h1 {
		font-size: 1.5rem;
		color: var(--blue-800);
		font-weight: var(--fw-x-bold);
	}
	.order-summary p {
		color: var(--blue-600);
		line-height: 1.5;
		font-size: 1rem;
	}
	.order-summary *:not(:last-child) {
		margin-bottom: 20px;
	}
	button {
		width: 100%;
		border: none;
		padding: 1rem;
		border-radius: 1rem;
		background-color: var(--blue-400);
		color: var(--blue-100);
		font-weight: var(--fw-bold);
		letter-spacing: 0.5px;
		box-shadow: 0 12px 23px -6px hsla(245, 60%, 52%, 0.7);
	}
	button:hover {
		cursor: pointer;
		opacity: 0.7;
		text-decoration: none;
	}
	.cancel {
		color: var(--blue-600);
		font-weight: var(--fw-x-bold);
	}
	.cancel:hover {
		cursor: pointer;
		color: var(--blue-800);
	}
	@media (min-width: 900px) {
		.product-card {
			width: 450px;
		}
		.order-summary {
			padding: 50px;
		}
		.order-summary *:not(:last-child) {
			margin-bottom: 25px;
		}
	}
</style>
