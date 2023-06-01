<script lang="ts">
	let kittenTime = false;
	const toggleKittenTime = () => {
		kittenTime = kittenTime ? false : true;

	}
</script>

<main>
    <a 
	target="picture"
	on:click={toggleKittenTime}
	>
		<h1>
		{
		kittenTime 
		? "Kitten Time!"
		: "I have something to show you..."
		}
		</h1>
	</a>
	
	<img 
		id="picture"
		src="https://media.tenor.com/wL59aqQiwzAAAAAd/cat-kitty.gif"
		hidden={!kittenTime}
	/>
</main>

<style>
	h1 {
		font-size: 4em;
		color: beige;
	}
	
	main {
		font-family: luminari;
		background-color: darkred;
		color: beige;
		padding: 1em;
		min-height: 50rem;
		border-radius: 1rem;
	}
	
	a h1:hover {
		color: cyan;
 	}

	#picture {
		border-radius: 2rem;
		height: 30em;
		width: 30rem;
 	}

	@media (prefers-color-scheme: light) {
		main { background-color: beige; color: darkred; }

	}
</style>

