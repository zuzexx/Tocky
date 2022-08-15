<script>
  import Router from "svelte-spa-router";
  import About from "./routes/about/about.svelte";
  import Blog from "./routes/blog/blog.svelte";
  import Contact from "./routes/contact/contact.svelte";
  import Faqp from "./routes/faqp/faqp.svelte";
  import LandingPage from "./routes/landingPage/landingPage.svelte";
  import Header from "./routes/components/header.svelte";
  import NotFound from "./routes/notFound/notFound.svelte";
  import Signup from "./routes/sign/signup.svelte";
  import Signin from "./routes/sign/signin.svelte";

  let routes = {
    "/": LandingPage,
    "/about": About,
    "/blog": Blog,
    "/contact": Contact,
    "/faqp": Faqp,
    "/signup": Signup,
    "/signin": Signin,
    "*": NotFound,
  };
</script>

<header>
  <Header />
</header>
<main>
  <Router {routes} />
</main>
