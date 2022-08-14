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
    font-size: 0.9rem;
    color: var(--header);
    font-weight:var(--regular);
   
  }
  li:hover{
    cursor: pointer;
    border-bottom:1px solid var(--header-border-bottom);
    text-transform: uppercase;
    border-left:1px solid var(--header-border-top);
    font-weight:var(--medium);
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
    .header-container, .inner-container {
      width: 50vw;
    }
    li {
    padding: 2rem;
  }
    
  }
</style>
