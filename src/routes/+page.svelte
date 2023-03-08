<script>
	import '../styles.css';
	import Hero from '$lib/components/Hero.svelte';
	import Futures from '$lib/components/Futures.svelte';
	import Presentation from '$lib/components/Presentation.svelte';
</script>

<div class="hero-container">
	<Hero presentationId="presentationId" />
</div>
<main>
	<section class="not-full">
		<Futures />
	</section>
	<section id="presentationId">
		<Presentation />
	</section>
</main>

<style>
	.not-full {
		max-width: 1440px;
		margin: 0 auto;
	}

	@media screen and (max-width: 1440px) {
		.not-full {
			margin: 0 50px;
		}
	}
</style>
