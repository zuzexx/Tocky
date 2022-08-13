<script>
  import Buttons from "./buttons.svelte";
</script>

<div class="header-container">
  <div class="outer-container">
    <div class="inner-container">
      <img src="images/logo.png" alt="" class="logo" />
      <Buttons>Grow yout TikTok today!</Buttons>
    </div>

    <ul>
      <li>About</li>
      <li>Pricing</li>
      <li>Blog</li>
      <li>FAQ</li>
      <li>Contact</li>
    </ul>
  </div>
  <!--
    <div class="header-btns">
        <Buttons>Grow yout TikTok today!</Buttons>
        
    </div>-->
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
    .header-container, .inner-container {
      width: 50vw;
    }
    
  }
</style>
