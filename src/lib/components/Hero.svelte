<script>
	import backgroundVideo from '$lib/assets/background-test.mp4';
	import posterImg from '$lib/assets/bg-loop-still.webp';
	import ButtonSolid from '$lib/components/buttons/ButtonSolid.svelte';
	import ButtonBorder from '$lib/components/buttons/ButtonBorder.svelte';
	import logo from '$lib/assets/logo.svg';

	export let presentationId;
</script>

<div class="hero">
	<div class="nav">
		<img src={logo} alt="Logoen til Innlandet Piano som er ut som et flygel" />
		<ButtonBorder text="Ta kontakt" width="180px" height="50px" />
	</div>
	<div class="hero-text-container">
		<div class="hero-text">
			<h2>Stemming, service, reparasjoner & renovering</h2>
			<h1>INNLANDET PIANO</h1>
			<p>
				Utfører alt av stemming, service, reparasjoner og renoveringer på flygler og pianoer over
				hele landet
			</p>
			<div class="buttons">
				<a href="#">
					<ButtonSolid text="Ta kontakt" />
				</a>
				<a href="#{presentationId}">
					<ButtonBorder text="Se presentasjon" />
				</a>
			</div>
		</div>
	</div>
	<video class="video-bg" autoplay muted loop playsinline poster={posterImg}>
		<source src={backgroundVideo} type="video/mp4" />
	</video>
</div>

<style>
	.buttons {
		display: flex;
		gap: 64px;
	}

	.hero {
		display: flex;
		min-height: 100vh;
		position: relative;
		background: #333;
		overflow: hidden;
		background: rgba(0, 0, 0, 0.3);
		width: 100%;
		flex-direction: column;
		align-items: center;
	}

	.nav {
		display: flex;
		justify-content: space-between;
		align-items: center;
		width: 90%;
		max-width: 1440px;
		min-height: 8vh;
	}

	.hero-text-container {
		display: flex;
		justify-content: center;
		flex-direction: column;
		align-items: center;
		color: #fff5f6;
		min-width: 800px;
		min-height: 84vh;
	}

	.hero-text {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.video-bg {
		width: 100%;
		min-height: 100%;
		position: absolute;
		top: 0;
		left: 0;
		object-fit: cover;
		z-index: -1;
	}

	h1 {
		font-size: 96px;
	}
	h2 {
		font-size: 31px;
		letter-spacing: 3px;
		font-weight: 600;
	}
	p {
		font-size: 25px;
		letter-spacing: 5%;
		line-height: 1.5;
		width: 70%;
		margin-top: 16px;
		text-align: center;
		margin-bottom: 48px;
	}
</style>
