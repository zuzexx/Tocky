<script>
  import Buttons from "../components/buttons.svelte";
</script>

<div class="header-container">
  <div class="outer-container">
    <div class="inner-container">
      <a href="#/"><img src="images/logo.png" alt="" class="logo" /></a>
      
      <Buttons>Grow yout TikTok today!</Buttons>
    </div>

    <ul>
      <a href="#/about"><li>About</li></a>
      <a href="#/price"><li>Pricing</li></a>
      <a href="#/blog"><li>Blog</li></a>
      <a href="#/faqp"><li>FAQ</li></a>
      <a href="#/contact"><li>Contact</li></a>
      
    </ul>
  </div>
</div>

<style>
  .inner-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 80vw;
  }
  .outer-container {
    display: grid;

    justify-items: center;
    align-self: center;
    grid-template-rows: 1fr 1fr;
  }
  ul {
    list-style-type: none;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
  }

  li {
    padding: 1rem;
    font-size: 0.9rem;
    color: var(--header);
    font-weight: var(--regular);
  }
  li:hover {
    cursor: pointer;
    border-bottom: 1px solid var(--header-border-bottom);
    text-transform: uppercase;
    border-left: 1px solid var(--header-border-top);
    font-weight: var(--medium);
    font-size: 1rem;
  }
  .logo {
    width: 50px;
  }
  .header-container {
    display: flex;
    flex-direction: column;
    width: 80vw;
    height: auto;
    justify-content: center;
    align-items: center;
    margin: auto;
  }

  @media only screen and (min-width: 800px) {
    .header-container,
    .inner-container {
      width: 50vw;
    }
    li {
      padding: 2.5rem;
      font-size: 1.3rem;
    }
    li:hover {
      font-size: 1.4rem;
    }
  }
</style>
