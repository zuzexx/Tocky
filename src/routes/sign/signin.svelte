<script>
  import Buttons from "../components/buttons.svelte";
</script>

<div class="container">
  <div class="text-container">
    <img src="images/logo.png" alt="" />
    <h1>Sign In to your account</h1>

    <p>or <a href="#/signup">sign up</a></p>
  </div>

  <form action="">
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
        placeholder="Password"
      />
    </div>
    <div class="bottom-container">
      <div class="check">
        <input type="checkbox" name="radio">
      <label for="radio">Remember me</label>
      </div>
      <p class="password-forgot">Forgot your password?</p>
    </div>

    <Buttons>Submit</Buttons>
  </form>
</div>

<style>
  .bottom-container{
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 50vw;
  }
  .password-forgot{
    color: var(--header-span);
    font-size: 0.8rem;
  }
  .password-forgot:hover{
    cursor: pointer;
    text-decoration: underline;
  }
  .check{
    display: flex;
    width:100px;
    justify-content: center;
    align-items: center;
    font-size: 0.7rem;
  }
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
  h1{
    color: var(--header);
  }
  p{
    color: var(--paragraph);
  }
  a{
    color: var(--header-span);
    font-weight: var(--bold);
    text-decoration: none;
  }

  @media only screen and (min-width: 1200px) {
    form {
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
    .bottom-container{
      max-width: 700px;
    }
  }
</style>
