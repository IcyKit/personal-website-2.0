<script>
	import { page } from '$app/stores';
	import Burger from './Burger.svelte';
</script>

<nav>
	<div class="title">
		<a href="/">Efimov Nikita</a>
	</div>
	<div class="links">
		<a aria-current={$page.url.pathname === '/stack' ? 'page' : undefined} href="/stack">Stack</a>
		<a aria-current={$page.url.pathname === '/works' ? 'page' : undefined} href="/works">Works</a>
		<a aria-current={$page.url.pathname === '/workspace' ? 'page' : undefined} href="/workspace"
			>Workspace</a
		>
	</div>
	<Burger />
</nav>

<style>
	nav {
		display: flex;
		justify-content: space-between;
		padding-top: 30px;
	}

	.title {
		font-size: 16px;
		font-weight: bold;
		text-transform: uppercase;
		display: flex;
		align-items: center;
	}

	.links {
		display: flex;
		justify-content: space-between;
		gap: 15px;
	}

	a[aria-current='page'] {
		text-decoration: underline;
	}

	@media (max-width: 460px) {
		nav {
			padding-top: 15px;
		}

		.title {
			font-size: 14px;
		}

		.links {
			font-size: 14px;
			gap: 10px;
			display: none;
		}
	}
</style>
