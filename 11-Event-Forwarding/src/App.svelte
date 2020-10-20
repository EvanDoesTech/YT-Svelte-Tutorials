<script>
	import Button from "./Button.svelte";

	const log = () => {
		console.log("Button clicked")
	}
</script>

<main>
	<Button on:click={log} />
	<button on:click={log}>App button</button>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>