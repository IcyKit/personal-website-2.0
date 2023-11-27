<script>
	import Card from './Card.svelte';
	import { fly } from 'svelte/transition';
	let isVisible = false;

	setTimeout(() => {
		isVisible = true;
	}, 500);
</script>

{#if isVisible}
	<div class="info" transition:fly={{ y: 20, duration: 500 }}>
		<h2>Get to know me <span>🤝🏻</span></h2>
		<div class="cards">
			<Card title="Stack" descr="My tech stack" link="/stack" image="ts.png" />
			<Card title="About me" descr="Who I am" link="/" image="memoji.png" />
			<Card title="Workspace" descr="My working space" link="/workspace" image="macbook.png" />
			<Card title="Works" descr="My way" link="/works" image="web.png" />
		</div>
	</div>
{/if}

<style>
	span {
		font-size: 28px;
		padding-left: 5px;
	}
	.info {
		padding-top: 100px;
	}

	h2 {
		font-size: 22px;
		font-weight: 500;
		margin-bottom: 30px;
	}

	.cards {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr 1fr;
		justify-items: stretch;
		gap: 15px;
	}

	@media (max-width: 750px) {
		.cards {
			grid-template-columns: 1fr 1fr 1fr;
		}
	}

	@media (max-width: 570px) {
		.cards {
			grid-template-columns: 1fr 1fr;
		}
	}

	@media (max-width: 460px) {
		h2 {
			font-size: 18px;
			margin-bottom: 20px;
		}

		.info {
			padding-top: 50px;
		}
	}
</style>
