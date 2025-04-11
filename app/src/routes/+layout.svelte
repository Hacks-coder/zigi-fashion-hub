<script lang="ts">
	import '../app.css';
	import '@fontsource-variable/inter';
	import '@fontsource-variable/lexend';
	import Header from '../components/Header/Header.svelte';
	import Hero from '../components/Main/Hero.svelte';

	let { children } = $props();
</script>

<div>
	<Header />
	<Hero />
	{@render children()}
</div>
