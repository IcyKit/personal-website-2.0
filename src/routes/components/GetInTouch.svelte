<script>
	import Badge from './Badge.svelte';
</script>

<div class="touch">
	<h2>Get in touch</h2>
	<div class="badges">
		<Badge />
		<Badge />
		<Badge />
		<Badge />
		<Badge />
		<Badge />
		<Badge />
		<Badge />
	</div>
</div>

<style>
	.touch {
		padding-top: 100px;
	}

	h2 {
		font-size: 22px;
		font-weight: 500;
		margin-bottom: 30px;
	}

	.badges {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 20px;
		align-content: stretch;
	}

	@media (max-width: 670px) {
		.touch {
			padding-top: 50px;
		}
	}
</style>
