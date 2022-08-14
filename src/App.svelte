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
<body>
	
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
</body>




<style>

	:root{
		--background:#f3f3f3;
		--header:#001446;
		--paragraph:#141a74;
		--light-paragraph:#c6ddea;
		--button-color:#0c213a;
		--button-hover:#9ec0ea;
		--header-border-top:#35edfa;
		--header-border-bottom:#db464f;
		--header-span:#97dee8;
	}
	
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