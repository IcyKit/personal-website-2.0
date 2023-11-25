<script lang="ts">
	export let link: string;
	export let nick: string;
	export let icon;
</script>

<a href={link} target="_blank">
	<div class="badge">
		<div class="icon">
			<svelte:component this={icon} />
		</div>
		<h3>{nick}</h3>
	</div>
</a>

<style>
	.badge {
		background: #f6f6f6;
		border: 1px solid #ebebeb;
		border-radius: 10px;
		padding: 10px 0;
		display: flex;
		align-items: center;
		justify-content: center;
		transition: 0.3s all;
	}

	.badge:hover {
		background: #eeeeee;
	}

	h3 {
		font-size: 16px;
	}

	.icon {
		width: 20px;
		margin-right: 10px;
	}

	@media (max-width: 670px) {
		h3 {
			font-size: 14px;
		}

		.icon {
			width: 20px;
		}
	}
</style>
