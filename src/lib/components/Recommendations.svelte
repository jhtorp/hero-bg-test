<script>
	import quote from '$lib/assets/quote.svg';
	import avatar from '$lib/assets/avatar.png';
</script>

<div class="container">
	<img class="quote quote1" src={quote} alt="" />
	<div class="cards">
		<div class="card">
			<p class="content">
				“Raskt på pletten når han blir innkalt. Stabilt og godt resultat. Det merkes at Arve har
				stor interesse for faget. Han er dedikert, og bidrar til å holde vårt Steinway-flygel i
				toppform”
			</p>
			<div class="profile">
				<img src={avatar} alt="" />
				<div class="who">
					<p class="name">Håvard Amlie</p>
					<p>kirketjener i Ås kirke - Vestre Toten</p>
				</div>
			</div>
		</div>
		<div class="card">
			<p class="content">
				“Musikklinja ved Gjøvik Vgs setter stor pris på en fast kontrakt og det gode samarbeidet med
				Innlandet Piano om stemming og vedlikehold av skolens pianoer og flygler”
			</p>
			<div class="profile">
				<img src={avatar} alt="" />
				<div class="who">
					<p class="name">Line Løvland Øfstaas</p>
					<p>Pianist og Avdelingsleder for musikklinja - Gjøvik Vgs</p>
				</div>
			</div>
		</div>
		<div class="card">
			<p class="content">
				“Raskt på pletten når han blir innkalt. Stabilt og godt resultat. Det merkes at Arve har
				stor interesse for faget. Han er dedikert, og bidrar til å holde vårt Steinway-flygel i
				toppform”
			</p>
			<div class="profile">
				<img src={avatar} alt="" />
				<div class="who">
					<p class="name">Knut Anders Sørum</p>
					<p>Komponist, musiker og sanger</p>
				</div>
			</div>
		</div>
	</div>
	<img class="quote quote2" src={quote} alt="" />
</div>

<style>
	.quote {
		position: absolute;
		z-index: -1;
	}

	.quote1 {
		top: 0;
		left: 0;
		transform: translate(-50%, -128px);
	}

	.quote2 {
		transform: rotate(180deg) translate(-50%, -128px);
		right: 0;
		bottom: 0;
	}

	.container {
		position: relative;
		width: 100%;
		margin: 128px 0;
	}

	.content {
		padding-bottom: 32px;
		font-size: 20px;
		line-height: 1.5;
	}

	.cards {
		display: flex;
		justify-content: space-between;
		gap: 8%;
	}
	.profile {
		display: flex;
		align-items: center;
		gap: 24px;
	}

	.card {
	}

	.name {
		font-weight: 500;
	}
</style>
