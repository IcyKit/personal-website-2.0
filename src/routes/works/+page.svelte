<script>
	import Work from '../components/Work.svelte';
</script>

<div class="workpage">
	<div class="title">
		<h2>Work</h2>
		<p>Here's a summary of my work</p>
	</div>
	<Work />
</div>

<style>
	.workpage {
		padding-top: 100px;
	}

	h2 {
		font-size: 24px;
		font-weight: bold;
	}

	.title > p {
		font-size: 16px;
	}

	@media (max-width: 460px) {
		.workpage {
			padding-top: 40px;
		}

		h2 {
			font-size: 16px;
		}

		.title > p {
			font-size: 14px;
		}
	}
</style>
