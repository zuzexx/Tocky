<script>
  import ContForm from "./contForm.svelte";
  import Hiring from "./hiring.svelte";
  import Footer from "../components/footer.svelte";
</script>

<Hiring />
<div class="container">
  <img src="images/office.jpg" alt="office" />
  <ContForm />
</div>

<Footer />

<style>
  .container {
    width: 80vw;
    margin: auto;
  }
  img {
    display: none;
  }

  @media only screen and (min-width: 1440px) {
    img {
      display: flex;
      width: 25vw;
      border-radius: 20px;
      margin-top: 9rem;
    }
    .container {
      display: grid;
      justify-content: center;
      align-items: center;
      margin: auto;
      grid-template-columns: 1fr 1fr;
      width: 50vw;
      column-gap: 4rem;
    }
  }
</style>
