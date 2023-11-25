<script>
	import '../app.css';
	import Footer from './components/Footer.svelte';
	import Header from './components/Header.svelte';
</script>

<div class="container">
	<Header />
	<slot />
	<Footer />
</div>

<style>
	.container {
		max-width: 726px;
		margin: 0 auto;
	}

	@media (max-width: 750px) {
		.container {
			padding: 0 15px 0 15px;
		}
	}
</style>
