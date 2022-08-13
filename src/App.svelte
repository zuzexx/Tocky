<script>
	import Header from "./components/header.svelte";
	import TopPart from "./components/topPart.svelte";
	import LittleGrid from "./components/littleGrid.svelte";
	import Trusted from "./components/trusted.svelte";
	import HowItWorks from "./components/howItWorks.svelte";
import Ready from "./components/ready.svelte";
import CustomerOpinion from "./components/customerOpinion.svelte";
import Pricing from "./components/pricing.svelte";
import Faq from "./components/faq.svelte";
import Newsletter from "./components/newsletter.svelte";
import Footer from "./components/footer.svelte";

</script>

<header>
	<Header/>
</header>
<main>
<TopPart/>
<LittleGrid/>
<Trusted/>
<HowItWorks/>
<Ready/>
<CustomerOpinion/>
<Pricing/>
<Faq/>
<Ready/>
<Newsletter/>
<Footer/>
</main>


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