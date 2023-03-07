<script>
	import flygelIcon from '$lib/assets/flygel.svg';
</script>

<div class="container">
	<div class="card">
		<div class="heading">
			<img src={flygelIcon} alt="" />
			<h3>Stemming</h3>
		</div>
		<p>
			Flygler og pianoer bør stemmes minst én gang i året uavhengig av bruk, men gjerne oftere.
			Produsentene anbefaler minst to ganger i året. Dette for å best mulig ivareta instrumentet, og
			bidra til at det holder seg over tid
		</p>
	</div>
	<div class="card">
		<div class="heading">
			<img src={flygelIcon} alt="" />
			<h3>Service</h3>
		</div>
		<p>
			Et piano består av mange deler som skal fungere optimalt sammen. Dette kan man merke ved at
			for eksempel en eller flere toner låter ujevnt eller skarpt eller at tangenter oppleves
			forskjellige å spille på. Derfor trenger instrumentet også med jevne mellomrom en service hvor
			pianoteknikeren regulerer og intonerer instrumentet.
		</p>
	</div>
	<div class="card">
		<div class="heading">
			<img src={flygelIcon} alt="" />
			<h3>Reparasjoner</h3>
		</div>
		<p>
			Tangenter eller pedaler som ikke virker, toner som ikke låter, knirk eller annen ulyd? Det
			aller meste på et flygel eller piano lar seg reparere! For å forebygge slike problemer
			anbefaler Innlandet Piano å få installert et eget klimaanlegg for å bevare kvaliteten til
			instrumentet og holde stemmingen bedre.
		</p>
	</div>
	<div class="card">
		<div class="heading">
			<img src={flygelIcon} alt="" />
			<h3>Renovering</h3>
		</div>
		<p>
			Av og til kan det være nødvendig med en større gjennomgang av flygelet eller pianoet for å
			hjelpe det tilbake til et bra instrument! Mekaniske deler kan være utslitt og må byttes, eller
			det trenger en større gjennomgang med justeringer.
		</p>
	</div>
</div>

<style>
	.container {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 128px;
		margin-top: 128px;
		margin-bottom: 128px;
	}

	.heading {
		display: flex;
		align-items: center;
		gap: 20px;
		font-size: 25px;
	}

	p {
		line-height: 1.5;
		font-size: 20px;
	}
</style>
