<script>
	let name = "";
	let src = "favicon.png";
	let count = 0;

	const incrementCounter = () => {
		count += 1;
	}

	const handleInput = (event) => {
		name = event.target.value;
	}

	const resetName = () => {
		name = "Unknown";
	}

</script>

<main>
	<h1>Hello {name}</h1>

	<input type="text" bind:value={name}>
	<button on:click={resetName}>Set name to Unknown</button>

	<img {src} alt="Svelte logo">
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	h1 {
		font-size: 72px;
		text-align: center;
	}

	h3 {
		font-size: 38px;
	}
</style>