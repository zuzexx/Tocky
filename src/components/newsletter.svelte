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
    }

    @media only screen and (min-width:1200px){
        
    .newsletter-container{
        flex-direction: row;
        justify-content: center;
        width: 50vw;
        
    }
    }
    
</style>