<script>
	import Header from "./components/header.svelte";
	import TopPart from "./components/topPart.svelte";
	import LittleGrid from "./components/littleGrid.svelte";
	import Trusted from "./components/trusted.svelte";
</script>

<header>
	<Header/>
</header>
<main>
<TopPart/>
<LittleGrid/>
<Trusted/>
</main>
<footer>

</footer>

<style>
	
main{
	width: 80vw;
	margin: auto;
}
@media only screen and (min-width: 1200px) {
    main {
      width: 50vw;
    }
    
  }
</style>