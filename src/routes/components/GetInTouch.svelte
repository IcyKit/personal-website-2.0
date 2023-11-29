<script>
	import Badge from './Badge.svelte';
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte';
	import FaTelegram from 'svelte-icons/fa/FaTelegram.svelte';
	import FaLinkedin from 'svelte-icons/fa/FaLinkedin.svelte';
	import FaDiscord from 'svelte-icons/fa/FaDiscord.svelte';
	import FaInstagram from 'svelte-icons/fa/FaInstagram.svelte';
	import FaVk from 'svelte-icons/fa/FaVk.svelte';

	const badges = [
		{
			component: FaGithub,
			props: {
				link: 'https://github.com/IcyKit',
				nick: 'IcyKit'
			}
		},
		{
			component: FaTelegram,
			props: {
				link: 'https://t.me/icykit',
				nick: 'IcyKit'
			}
		},
		{
			component: FaLinkedin,
			props: {
				link: 'https://www.linkedin.com/in/nikita-efimov-756461237/',
				nick: 'Nikita Efimov'
			}
		},
		{
			component: FaDiscord,
			props: {
				link: 'https://discord.com/users/193069352554201088/',
				nick: 'IcyKit'
			}
		},
		{
			component: FaInstagram,
			props: {
				link: 'https://www.instagram.com/icy_kit/',
				nick: 'icy_kit'
			}
		},
		{
			component: FaVk,
			props: {
				link: 'https://vk.com/mrkit228',
				nick: 'Nikita Efimov'
			}
		}
	];
</script>

<div class="touch">
	<h2>Get in touch <span>🤙🏻</span></h2>
	<div class="badges">
		{#each badges as badge}
			<Badge link={badge.props.link} nick={badge.props.nick} icon={badge.component} />
		{/each}
	</div>
</div>

<style>
	span {
		font-size: 28px;
		padding-left: 5px;
	}
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
		grid-template-columns: 1fr 1fr 1fr;
		gap: 20px;
		align-content: stretch;
	}

	@media (max-width: 670px) {
		span {
			font-size: 22px;
		}

		h2 {
			font-size: 18px;
		}
		.touch {
			padding-top: 50px;
		}

		.badges {
			grid-template-columns: 1fr 1fr;
		}
	}

	@media (max-width: 460px) {
		h2 {
			font-size: 18px;
			margin-bottom: 10px;
		}
	}
</style>
