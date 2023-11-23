<script lang="ts">
	export let title: string;
	export let descr: string;
	export let image: string;
</script>

<div class="card">
	<div class="title">
		<h3>{title}</h3>
		<p>{descr}</p>
	</div>
	<div class="image">
		<img src={image} alt="card image" />
	</div>
</div>

<style>
	.card {
		background: #f6f6f6;
		border: 1px solid #ebebeb;
		border-radius: 20px;
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 15px 0 15px 0;
	}

	.title {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin-bottom: 10px;
	}

	h3 {
		font-size: 16px;
		font-weight: bold;
	}

	p {
		font-size: 14px;
	}

	.image {
		width: 100px;
	}

	@media (max-width: 460px) {
		h3 {
			font-size: 12px;
			line-height: 12px;
		}

		p {
			font-size: 10px;
		}

		.title {
			margin-bottom: 8px;
		}

		.image {
			width: 80px;
		}
	}

	@media (max-width: 400px) {
		.title {
			margin-bottom: 5px;
		}

		.image {
			width: 70px;
		}
	}
</style>
