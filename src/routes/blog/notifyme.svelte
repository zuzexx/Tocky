<script>
  import Buttons from "../components/buttons.svelte";

  let email = " ";

  let hasBeenClicked = false;

  function validateEmail(email) {
    var emailRegEx =
      /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
    return emailRegEx.test(String(email).toLowerCase());
  }

  function handleSubmission() {
    hasBeenClicked = true;

    if (isValidEmail) {
      // Send data somewhere
      alert("You will get an email shortly.");
    }
  }
  $: isValidEmail = validateEmail(email);
</script>

<div class="newsletter-container">
  <div class="text-container">
    <h2>Get notified about new posts!</h2>
    <p>
      The quick, brown fox jumps over a lazy dog. DJs flock by when MTV ax quiz
      prog. Junk MTV quiz graced by fox whelps. Bawds jog, flick quartz, vex
      nymphs. Waltz
    </p>
  </div>
  <div class="input-container">
    <div class="inner-container">
      {#if hasBeenClicked && !isValidEmail}
        <p class="validation-error">Invalid email</p>
      {/if}
      <input type="main" class="mail-input" />

      <Buttons on:click={handleSubmission}>Notify me</Buttons>
    </div>
  </div>
</div>

<style>
  .validation-error {
    font-size: 0.7rem;
    color: var(--header-border-bottom);
  }
  .newsletter-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 80vw;
    text-align: center;
    margin: auto;
    background-color: var(--newsletter);
    padding: 3rem;
    border-radius: 20px;
    margin: 5rem;
  }

  p {
    color: var(--paragraph);
    font-size: 0.9rem;
    font-weight: var(--regular);
  }

  @media only screen and (min-width: 1200px) {
    .newsletter-container {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 50vw;
      margin: auto;
      padding: 5rem;
    }
    .inner-container {
      display: flex;
      justify-content: space-evenly;
      align-items: center;
      width: 50vw;
    }
    .input-container {
      width: 50vw;
    }
    input {
      width: 600px;
      margin-top: 1rem;
    }

    p {
      font-size: 1rem;
    }
  }
</style>
