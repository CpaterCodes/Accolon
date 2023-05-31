<script lang="ts">
</script>

<main>
    <a 
	href="https://media.tenor.com/wL59aqQiwzAAAAAd/cat-kitty.gif"
	target="picture"
	on:click={() => alert("It's kitten time!")}
	>
		<h1> I have something to show you!!! </h1>
	</a>
	<iframe name="picture" id="picture" frameborder="0"/>
</main>

<style>
	main {
		font-family: fantasy;
	}
	
	a {
		color: lime;
	}

	a:hover {
		color: cyan;
 	}

	a:visited {
		color: orange;
	}
 
	#picture {
		border-radius: 15rem;
		height: 30em;
		width: 30em;
 	}
</style>

