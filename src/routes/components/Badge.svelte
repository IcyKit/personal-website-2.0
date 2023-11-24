<script lang="ts">
	import DiGithubBadge from 'svelte-icons/di/DiGithubBadge.svelte';

	export let link: string;
	export let nick: string;
	export let icon;
</script>

<a href="https://google.com" target="_blank">
	<div class="badge">
		<div class="icon">
			<DiGithubBadge />
		</div>
		<h3>IcyKit</h3>
	</div>
</a>

<style>
	.badge {
		background: #f6f6f6;
		border: 1px solid #ebebeb;
		border-radius: 10px;
		padding: 5px 0;
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
		width: 35px;
		margin-right: 5px;
	}

	@media (max-width: 670px) {
		h3 {
			font-size: 14px;
		}

		.icon {
			width: 30px;
		}
	}
</style>
