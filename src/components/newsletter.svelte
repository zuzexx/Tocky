<script>
    import Buttons from "./buttons.svelte";
</script>

<div class="newsletter-container">
    <div class="text-container">
        <h2>Sign up for our newsletter</h2> 
        <p>The quick, brown fox jumps over a lazy dog. DJs flock by when MTV ax quiz prog. Junk MTV quiz graced by fox whelps. Bawds jog, flick quartz, vex nymphs. Waltz</p>
    </div>
    <div class="input-container">
        <div class="inner-container">
            <input type="main" class="mail-input">
            <Buttons>Notify me</Buttons>
        </div>
        <div class="privacy-policy">We care about the protection of your data. Read our <span>Privacy Policy</span>.</div>
    </div>
    
</div>

<style>
    .newsletter-container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 80vw;
        text-align: center;
        margin: auto;
        margin-top: 7rem;
        background-color: var(--header-span);
        border-radius: 20px;
        padding: 2rem;
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
    input{
        width: 600px;
        margin-top: 1rem;

    }
    .privacy-policy{
        text-align: left;
    }
    p{
        font-size: 1rem;
    }
    }
    
</style>