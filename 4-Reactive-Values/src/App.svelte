<script>
	let firstName = "";
	let lastName = "";
	let src = "favicon.png"

	$: fullName = `${firstName} ${lastName}`
	$: {
		console.log(lastName);
		console.log(firstName);
	}

</script>

<main>
	<h1>Hello {fullName}</h1>

	<label for="firstname">FirstName</label>
	<input type="text" bind:value={firstName}>
	<label for="firstname">LastName</label>
	<input type="text" bind:value={lastName}>

	
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