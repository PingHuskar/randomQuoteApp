<script>
import Quote from './Quote.svelte';
let data = {};
randomQuote()
async function randomQuote() {
const response = await fetch('https://api.quotable.io/random?tags=technology')
data = await response.json()
}
</script>

<main>
	<h1>Random Quote App</h1>
	<Quote {data}/>
	<!-- <button on:click="{randomQuote}">New Quote</button> -->
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>