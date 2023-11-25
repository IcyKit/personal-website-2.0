<script>
	import Greetings from './components/Greetings.svelte';
	import GetToKnow from './components/GetToKnow.svelte';
	import About from './components/About.svelte';
	import GetInTouch from './components/GetInTouch.svelte';
	import { fade } from 'svelte/transition';
</script>

<div transition:fade={{ delay: 500, duration: 500 }}>
	<Greetings />
	<GetToKnow />
	<About />
	<GetInTouch />
</div>
