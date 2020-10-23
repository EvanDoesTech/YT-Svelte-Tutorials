<script>
	let name;
	let num;
	let isChecked = true;
	let value = 2;
	let selected;

	let questions = [
		{id: 1, text: "What is your favorite color?"},
		{id: 2, text: "What is your favorite fruit?"}
	]
</script>

<main>
	<input type="text" bind:value={name}>
	<input type="number" bind:value={num}>
	<input type="checkbox" bind:checked={isChecked}>

	<label>
		<input type="radio" bind:group={value} value={1}>
		1
	</label>
	<label>
		<input type="radio" bind:group={value} value={2}>
		2
	</label>
	<label>
		<input type="radio" bind:group={value} value={3}>
		3
	</label>

	<select bind:value={selected}>
		{#each questions as question}
			<option value={question}>
				{question.text}
			</option>
		{/each}
	</select>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>