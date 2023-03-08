<script>
	import Note from '$lib/assets/note-vektor.svelte';
</script>

<div class="container">
	<div class="note-container">
		<Note />
	</div>
	<div class="text">
		<h2>Presentasjonsvideo</h2>
		<p>
			Stemming av flygler og pianoer er et eget yrke som det krever år med trening for å beherske –
			et spennende kompromiss av musikalske preferanser og fysiske lover.
		</p>
		<p class="last-p">
			Arve Øfstaas er utdannet Pianostemmer og pianotekniker fra Norges Musikkhøgskole. Han ble
			uteksaminert i 2019 og er en av de fem første studentene i Norge som fikk ta denne
			musikkfaglig utdanningen på høgskolenivå
		</p>
	</div>
	<div class="video">
		<iframe
			src="https://player.vimeo.com/video/805630829?h=5b8408e6d1&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
			width="960"
			height="540"
			frameborder="0"
			allow="autoplay; fullscreen; picture-in-picture"
			allowfullscreen
			title="Main Edit Innlandet Piano 16x9 COMPRESSED.mov"
		/>
	</div>
</div>

<style>
	.container {
		background: #1e2b3a;
		position: relative;
		overflow: hidden;
		z-index: 0;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.text {
		max-width: 960px;
		margin: 48px auto 0;
		text-align: center;
		color: #fff5f6;
		position: relative;
		z-index: 1;
	}

	.note-container {
		position: absolute;
		width: 100%;
		transform: rotate(-30deg);
		scale: 1.2;
		top: 20%;
		pointer-events: none;
	}

	.video {
		margin: 96px auto;
		z-index: 1;
	}

	h2 {
		font-size: 48px;
	}

	p {
		font-size: 20px;
		margin-top: 40px;
	}

	.last-p {
		margin-top: 24px;
	}
</style>
