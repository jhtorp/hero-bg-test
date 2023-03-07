<script>
	import '../styles.css';
	import Hero from '$lib/components/Hero.svelte';
	import Futures from '$lib/components/Futures.svelte';
</script>

<div class="hero-container">
	<Hero />
</div>
<main>
	<Futures />
</main>

<style>
	main {
		max-width: 1440px;
		margin: 0 auto;
	}

	@media screen and (max-width: 1440px) {
		main {
			margin: 0 50px;
		}
	}
</style>
