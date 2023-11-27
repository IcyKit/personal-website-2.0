<script>
	import FaBars from 'svelte-icons/fa/FaBars.svelte';
</script>

<details class="daisydropdown">
	<summary class="m-1 btn"><FaBars /></summary>
	<ul class="p-2 shadow daisymenu daisydropdown-content z-[1] bg-base-100 daisyrounded-box w-52">
		<li><a>Item 1</a></li>
		<li><a>Item 2</a></li>
	</ul>
</details>

<style>
	summary {
		width: 20px;
		text-decoration: none;
	}

	.dropdown-summary::-webkit-details-marker {
		display: none;
	}
	.dropdown-summary::marker {
		display: none;
	}
</style>
