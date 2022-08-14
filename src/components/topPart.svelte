<script>
    import Buttons from "./buttons.svelte";

    let email = " ";
  
  let hasBeenClicked = false;

  function validateEmail(email) {
    var emailRegEx = /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;  
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

<div class="container">
    <div class="text-container">
        <h1>Grow your TikTok like a <span>pro</span></h1>
        <p class="paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
        <div class="input-container">
            <div class="put">
                {#if hasBeenClicked && !isValidEmail} 
                <p class="validation-error">Invalid email</p>
              {/if}
                <input type="email" class="mail-input" placeholder="Email">
                <Buttons on:click={handleSubmission}>Start free trial!</Buttons> 
            </div>
            
            <div class="trial-text">
                <p class="terms-of-service">Start your free 30-day trial. By providing your email, you agree to our <span>terms of service.</span> </p>
            </div>
        </div>
    </div>
    <div class="image-container">
        <img src="images/transparent.png" alt="" class="top-image">
    </div>

</div>

<style> 
h1{
    color:var(--header);
    font-size: 1.3rem;
    font-weight: var(--semi-bold);
}
.validation-error{
        font-size:0.7rem;
        color:var(--header-border-bottom);
    }
h1 span{
    font-size: 1.4rem;
    font-weight: var(--bold);
    text-transform: uppercase;
    color:var(--header-span);
}
.input-container{
    width: 80vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: auto;
}

.paragraph{
    font-weight: var(--light);
    font-size: 0.9rem;
    color: var(--paragraph);
}
.terms-of-service{
    font-weight: var(--extra-light);
    font-size: 0.7rem;
    color: var(--paragraph);
}
.terms-of-service span{
    text-decoration: underline;
    font-weight: var(--regular);
}
.terms-of-service span:hover{
    cursor: pointer;
}
.container{
    margin: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    align-items: center;
    width: 80vw;
    height: auto;
}
.top-image{
    width: 80vw;
}
.trial-text{
    margin: auto;
    font-size: 0.9rem;
}

@media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
      display: flex;
    flex-direction: row;
    justify-content: center;
    text-align: center;
    align-items: center;
    
    height: auto;

    }
    .trial-text{
        width: 20vw;
        text-align: left;
    }
    .paragraph{
        width: 25vw;
        text-align: left;
    }
    .top-image{
        width: 25vw;
        margin-left: 2rem;
    }
    h1{
        text-align: left;
        font-size: 1.8rem;
    }
    h1 span{
        font-size: 2rem;
    }
    input{
        width: 25vw;
    }
    .input-container{
        width: 25vw;
    }
    
  }
  @media only screen and (min-width: 1800px) {
    input{
        width: 500px;
        margin-top: 0.8rem;
        margin-right: 1rem;
    }
    .put{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        width: 25vw;
    }
  }
</style>