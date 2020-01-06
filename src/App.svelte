<script>
	export let name;
	import Comp from './components/component.svelte';
	let batosha = 'alena2'
	let inputText = 'test'

	function handleClick() {
		alert('Hi!')
	}
</script>

<main>
	<h1>Hello {name}! </h1>
	<button on:click={handleClick}>Press Me</button>
	<input type="text" bind:value={inputText}>
	<Comp {batosha}>
		Hello from App
	</Comp>
</main>

<style>
	/* scoped by default */
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
