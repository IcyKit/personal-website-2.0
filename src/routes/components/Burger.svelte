<script>
	import FaBars from 'svelte-icons/fa/FaBars.svelte';
	import { page } from '$app/stores';
</script>

<details class="daisydropdown daisydropdown-content daisydropdown-end">
	<summary class="m-1 btn"><FaBars /></summary>
	<ul class="daisydropdown-content z-[1] daisymenu p-2 shadow bg-base-100 rounded-box w-52">
		<li>
			<a aria-current={$page.url.pathname === '/stack' ? 'page' : undefined} href="/stack">Stack</a>
		</li>
		<li>
			<a aria-current={$page.url.pathname === '/works' ? 'page' : undefined} href="/works">Works</a>
		</li>
		<li>
			<a aria-current={$page.url.pathname === '/workspace' ? 'page' : undefined} href="/workspace"
				>Workspace</a
			>
		</li>
	</ul>
</details>

<style>
	details {
		padding: 5px;
		border-radius: 5px;
		background-color: #f6f6f6;
		border: 1px solid #ebebeb;
		color: #1f1f1f;
	}

	summary {
		width: 20px;
	}

	ul {
		box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.15);
	}

	@media (min-width: 461px) {
		details {
			display: none;
		}
	}
</style>
