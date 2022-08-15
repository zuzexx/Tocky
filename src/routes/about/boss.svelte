<script>
</script>

<div class="container">
  <img src="/images/boss.jpg" alt="" />
  <div class="text-container">
    <p class="paragraph">
      Li Europan lingues es membres del sam familie. Lor separat existentie es
      un myth. Por scientie, musica, sport etc, litot Europa usa li sam
      vocabular. Li lingues differe solmen in li grammatica, li pronunciation e
      li plu commun vocabules.
    </p>
    <p class="name">Big Boss, CEO at Tocky</p>
  </div>
</div>

<style>
  .container {
    width: 80vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: auto;
    margin-top: 10rem;
  }
  .text-container {
    width: 80vw;
    padding: 1rem;
    text-align: left;
  }
  .paragraph {
    font-size: 0.9rem;
    color: var(--paragraph);
  }
  .name {
    font-weight: var(--bold);
    color: var(--header-span);
    font-size: 1rem;
  }
  img {
    width: 300px;
    margin: auto;
    border-radius: 20px;
    border-left: 2px solid var(--header-border-top);
    border-bottom: 2px solid var(--header-border-bottom);
    border-top: 2px solid var(--header-border-top);
    border-right: 2px solid var(--header-border-bottom);
  }
  @media only screen and (min-width: 600px) {
    img {
      width: 400px;
    }
  }
  @media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      margin: auto;
      margin-top: 10rem;
    }
    img {
      width: 300px;
      margin: auto;
    }
    @media only screen and (min-width: 1500px) {
      img {
        width: 400px;
      }
      .paragraph {
        width: 500px;
      }
    }
  }
</style>
