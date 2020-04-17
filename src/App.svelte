<script>
  import Lol from "./Lol.svelte";
</script>

<style>
	:global(body) {
		/* this will apply to <body> */
		margin: 0;
		padding: 0;
	}

  main {
    height: 100%;
    width: 100%;
    background-color: darkslateblue;
  }
</style>

<main>
  <Lol />
</main>
