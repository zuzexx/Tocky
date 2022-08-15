<script>
  import Buttons from "../components/buttons.svelte";
</script>

<div class="container">
  <h3>Become a top content creator on tiktok</h3>
  <h1>Get tikTok followers using our powerfull growth strategies</h1>
  <div class="grid">
    <p class="first-paragraph">
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
      Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut
      fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem
      sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit
      amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora
      incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad
      minima veniam, quis nostrum exercitationem ullam corporis suscipit
      laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum
      iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae
      consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?
      At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
      praesentium voluptatum deleniti atque corrupti quos dolores et quas
      molestias excepturi sint occaecati cupiditate non provident, similique
      sunt in culpa qui officia deserunt mollitia animi, id est laborum et
      dolorum fuga.
    </p>
    <p class="second-paragraph">
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
      Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut
      fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem
      sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit
      amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora
      incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad
      minima veniam, quis nostrum exercitationem ullam corporis suscipit
      laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum
      iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae
      consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?
      At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
      praesentium voluptatum deleniti atque corrupti quos dolores et quas
      molestias excepturi sint occaecati cupiditate non provident, similique
      sunt in culpa qui officia deserunt mollitia animi, id est laborum et
      dolorum fuga.
    </p>
  </div>
  <a href="#/contact"><Buttons>Contact us</Buttons></a>
</div>

<style>
  h3 {
    text-transform: uppercase;
    font-size: 0.8rem;
    color: var(--header-span);
  }
  h1 {
    text-transform: capitalize;
    color: var(--header);
    font-size: 1.2rem;
  }
  p {
    color: var(--paragraph);
    padding: 1rem;
  }
  .grid {
    font-size: 0.8rem;
    width: 80vw;
    border-top: 2px solid var(--header-border-top);
    border-right: 2px solid var(--header-border-bottom);
  }
  .container {
    width: 80vw;
    margin: auto;
    margin: 5rem;
  }

  @media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
      margin: auto;
    }
    h3 {
      font-size: 1rem;
    }
    h1 {
      font-size: 1.5rem;
    }
    .grid {
      width: 50vw;
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr;
      column-gap: 3rem;
      text-align: left;
      font-size: 1.1rem;
      border-top: 2px solid var(--header-border-top);
      margin: auto;
      border-right: none;

      border-left: 2px solid var(--header-border-bottom);
    }
    p {
      padding: 2rem;
      margin: auto;
    }
  }
</style>
