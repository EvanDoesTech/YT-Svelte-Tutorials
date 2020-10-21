<script>
	import Button from "./Button.svelte";

	const log = () => {
		console.log("Element clicked")
	}
</script>

<main>
	<Button on:click={log} />
	<button on:click|once={log}>App button</button> 
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>