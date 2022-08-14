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
		--background:#282828;
		--header:#f0f0f0;
		--paragraph:#d4d4d4;
		--light-paragraph:#dcdcdc;
		--button-color:#0bb2ca;
		--button-hover:#891109;
		--header-border-top:#35edfa;
		--header-border-bottom:#db464f;
		--header-span:#97dee8;
		--little-grid:#9f9f9f;
		--free-trial:#3d3d3d;
		--newsletter:#242424;
		--footer:#e0e0e0;
	}
	
	
	
main{
	width: 100vw;
	margin: auto;
}

@media only screen and (min-width: 1200px) {
    
    
  }
</style>