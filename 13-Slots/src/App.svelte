<script>
	import Card from "./Card.svelte"
</script>

<main>
	<Card>
		<h3>Card</h3>
		<p>This is our card</p>
		
		<button slot="button">Test button</button>

		<div>
			<h4>This is below everything</h4>
		</div>
	</Card>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>