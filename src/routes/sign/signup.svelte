<script>
  import Buttons from "../components/buttons.svelte";
</script>

<div class="container">
  <div class="text-container">
    <img src="images/logo.png" alt="" />
    <h1>Sign Up to your account</h1>
    <p>or <a href="#/signin">sign in</a></p>
  </div>

  <form action="">
    <div class="name-container cont">
      <label for="name" class="name-label" />
      <input
        type="text"
        class="name-input"
        name="name"
        required
        placeholder="Full Name"
      />
    </div>

    <div class="email-container cont">
      <label for="email" class="email-label" />
      <input
        type="email"
        class="email-input"
        name="email"
        required
        placeholder="Email"
      />
    </div>
    <div class="password-container cont">
      <label for="password" class="where" />
      <input
        type="text"
        class="password-input"
        name="password"
        required
        placeholder="Email"
      />
    </div>

    <div class="password-container cont">
      <label for="password" class="where" />
      <input
        type="text"
        class="password-input"
        name="password"
        required
        placeholder="Repeat Pasword"
      />
    </div>

    <Buttons>Submit</Buttons>
  </form>
</div>

<style>
  form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 80vw;
  }
  img {
    width: 40px;
  }
  .text-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 80vw;
    margin: auto;
    text-align: center;
  }

  label {
    color: var(--paragraph);
  }

  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    text-align: left;
    width: 80vw;
  }

  h1 {
    color: var(--header);
  }
  p {
    color: var(--paragraph);
  }
  a {
    color: var(--header-span);
    font-weight: var(--bold);
    text-decoration: none;
  }

  @media only screen and (min-width: 1200px) {
    form {
      margin: auto;
      margin-top: 2rem;
      max-width: 700px;
    }

    .container {
      width: 50vw;
      max-width: 700px;
      margin: auto;
    }
    .text-container {
      max-width: 700px;
    }
    input {
      max-width: 700px;
    }
  }
</style>
