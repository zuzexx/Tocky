<script>
 
	import  Router from "svelte-spa-router";
  import About from "./routes/about/about.svelte";
  import Blog from "./routes/blog/blog.svelte"
  import Contact from "./routes/contact/contact.svelte"
  import Faqp from "./routes/faqp/faqp.svelte"
  import Price from "./routes/price/price.svelte"
  import LandingPage from "./routes/landingPage/landingPage.svelte";
  import Header from "./routes/components/header.svelte";
import NotFound from "./routes/notFound/notFound.svelte";


  let routes = {
    "/": LandingPage,
    "/about": About,
    "/blog":Blog,
    "/contact":Contact,
    "/faqp":Faqp,
    "/price":Price,
    "*":NotFound,
  }


  
</script>

<header>
  <Header />
</header>
<main>
  <Router {routes}/>
</main>








