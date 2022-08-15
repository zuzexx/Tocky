<script>
  import Buttons from "../components/buttons.svelte";
</script>

<div class="main">
  <div class="container">
    <h2>Start your free trial today!</h2>
    <a href="#/signup"><Buttons>I want a free trial!</Buttons></a>
  </div>
</div>

<style>
  .main {
    width: 100vw;
    background-color: var(--free-trial);
    padding: 2rem;
    margin-top: 7rem;
  }
  .container {
    width: 80vw;
    display: flex;
    justify-content: space-between;
    align-items: center;

    margin-top: 10rem;
    margin: auto;
  }

  @media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
    }
  }
</style>
