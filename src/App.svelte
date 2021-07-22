<script lang="ts">
	export let name: string;
	import '@nextbitlabs/trend-line';
	let data = [[1,1], [2,2], [3, 1.5], [4, 2.5]];
</script>

<main>
	<h1>Hello {name}!</h1>
	<trend-line {data}></trend-line>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
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

	trend-line {
		--background: #eee;
	}
</style>