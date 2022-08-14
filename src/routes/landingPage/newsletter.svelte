<script>
    import Buttons from "../components/buttons.svelte";

   
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
    <div class="newsletter-container">
        <div class="text-container">
            <h2>Sign up for our newsletter</h2> 
            <p>The quick, brown fox jumps over a lazy dog. DJs flock by when MTV ax quiz prog. Junk MTV quiz graced by fox whelps. Bawds jog, flick quartz, vex nymphs. Waltz</p>
        </div>
        <div class="input-container">
            <div class="inner-container">
                
                    {#if hasBeenClicked && !isValidEmail} 
                <p class="validation-error">Invalid email</p>
              {/if}
                    <input type="main" class="mail-input">
                
                
                
                <Buttons on:click={handleSubmission}>Notify me</Buttons>
            </div>
            <div class="privacy-policy">We care about the protection of your data. Read our <span>Privacy Policy</span>.</div>
        </div>
        
    </div>
</div>


<style>
    .container{
        
        margin-top: 7rem;
        background-color: var(--newsletter);
        border-radius: 20px;
        padding: 2rem;
        width: 100vw;
    }
    .validation-error{
        font-size:0.7rem;
        color:var(--header-border-bottom);
    }
    .newsletter-container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 80vw;
        text-align: center;
        margin: auto;
        
    }
    .privacy-policy{
        font-size: 0.8rem;
        font-weight: var(--light);
        color: var(--paragraph);
    }
    span{
        font-size: 0.9rem;
        text-decoration: underline;
        font-weight: var(--regular);
        color: var(--header);
    }
    p{
        color: var(--paragraph);
        font-size: 0.9rem;
        font-weight: var(--regular);
    }

    @media only screen and (min-width:1200px){
        
    .newsletter-container{
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 50vw;
       
        
    }
    .inner-container{
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 50vw;

    }
    .input-container{
        width: 50vw;
    }
    input{
        width: 600px;
        margin-top: 1rem;

    }
    
    p{
        font-size: 1rem;
    }
    }
    
</style>