<script>
	import { fly } from 'svelte/transition';
	let isVisible = false;

	setTimeout(() => {
		isVisible = true;
	}, 2500);
</script>

{#if isVisible}
	<div class="footer" transition:fly={{ y: 20, duration: 500 }}>
		<div class="footer__top">
			<div class="links">
				<h3>Links</h3>
				<ul>
					<li>
						<a href="/about">Home</a>
					</li>
					<li>
						<a href="/stack">Stack</a>
					</li>
					<li>
						<a href="/workspace">Workspace</a>
					</li>
					<li>
						<a href="/works">Works</a>
					</li>
				</ul>
			</div>
			<div class="elsewhere">
				<h3>Elsewhere</h3>
				<ul>
					<li>
						<a href="https://t.me/icykit" target="_blank">Telegram</a>
					</li>
					<li>
						<a href="https://github.com/IcyKit" target="_blank">GitHub</a>
					</li>
					<li>
						<a href="https://discord.com/users/193069352554201088/" target="_blank">Discord</a>
					</li>
					<li>
						<a href="https://www.linkedin.com/in/nikita-efimov-756461237/" target="_blank"
							>LinkedIn</a
						>
					</li>
				</ul>
			</div>
		</div>
		<p>© 2023 Nikita Efimov. All Rights Reserved.</p>
	</div>
{/if}

<style>
	.footer {
		padding-top: 100px;
		padding-bottom: 20px;
	}

	.footer__top {
		display: grid;
		grid-template-columns: 1fr 1fr;
		margin-bottom: 50px;
	}

	h3 {
		font-size: 16px;
		font-weight: bold;
		margin-bottom: 30px;
	}

	ul {
		display: flex;
		flex-direction: column;
		gap: 12px;
	}

	a:hover {
		color: rgb(102, 102, 102);
	}

	p {
		color: #aaaaaa;
		font-size: 14px;
	}

	@media (max-width: 425px) {
		.footer {
			padding-top: 50px;
		}

		.footer__top {
			margin-bottom: 40px;
			justify-items: center;
		}

		h3 {
			margin-bottom: 20px;
		}

		p {
			text-align: center;
		}

		h3,
		li,
		p {
			font-size: 14px;
		}
	}
</style>
