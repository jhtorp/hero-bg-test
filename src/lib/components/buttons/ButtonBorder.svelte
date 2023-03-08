<script>
	export let text;
	export let width = '250px';
	export let height = '60px';
</script>

<button style="width: {width}; height: {height};">{text}</button>

<style>
	button {
		font-size: 20px;
		background: none;
		border: 2px solid #fff5f6;
		color: #fff5f6;
		cursor: pointer;
		transition: 0.2s;
		font-family: 'Barlow', sans-serif;
	}

	button:hover {
		background: #fff5f6;
		color: #191a1c;
	}
</style>
