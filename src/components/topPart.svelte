<script>
    import Buttons from "./buttons.svelte";

</script>

<div class="container">
    <div class="text-container">
        <h1>Grow your TikTok like a <span>pro</span></h1>
        <p class="paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
        <div class="input-container">
            <input type="email" class="mail-input">
            <Buttons>Start free trial!</Buttons>
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
    }
    
  }
</style>