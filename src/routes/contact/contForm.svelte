<script>
    import Buttons from "../components/buttons.svelte";
</script>

<div class="container">

    <div class="text">
        <h2>Let's work <span>together!</span></h2>
        <p>The quick, brown fox jumps over a lazy dog. DJs flock by when MTV ax quiz prog. Junk MTV quiz graced by fox whelps. Bawds jog, flick quartz, vex nymphs. Waltz, bad nymph, for quick jigs vex! Fox nymphs grab quick-jived waltz. </p>
    </div>

    
    <form action="">

        <div class="name-container">
            <div class="first-name cont">
                <label for="name" class="name">First Name</label>
                <input type="text" class="first-name-input" name="name" required>
    
            </div>
            <div class="last-name cont">
                <label for="name-last" class="name-last">Last Name</label>
                <input type="text" class="last-name-input" name="name-last" required>
            </div>
        </div>
        <div class="email-container cont">
            <label for="email" class="email-label">Email</label>
            <input type="email" class="email-input" name="email" required>
        </div>
        <div class="company-container cont">
            <label for="company" class="company-label">Company</label>
            <input type="text" class="company-input" name="company">
        </div>
        <div class="phone-container cont">
            <label for="phone" class="phone">Phone</label>
            <input type="number" class="phone-input" name="phone">
        </div>
        <div class="more-container cont">
            <label for="more" class="more">How can we help you?</label>
            <textarea type="text" class="more-input" name="more" rows="5"></textarea>
        </div>
        <div class="where-container cont">
            <label for="where" class="where">Where did you hear about us?</label>
            <input type="text" class="where-input" name="where">
        </div>
    
        <Buttons>Submit</Buttons>
    
    </form>
    
</div>



<style>


    label{
        color:var(--paragraph);
    }
    textarea{
        height: 8rem;
    }
    form, .text{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: left;
        width: 80vw;
        margin: auto;
        margin-top: 6rem;
    }
    .cont{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-end;
        text-align: left;
    }
    .text{
        text-align: right;
    }
    h2{
        font-size: 1.6rem;
        color: var(--header);
    }
    p{
        font-size: 1rem;
        color: var(--paragraph);
    }
    span{
        color: var(--header-span);
    }

    @media only screen and (min-width:1440px){
        form, .text{
            width: 25vw;
        }
        form{
            margin-top: 2rem;
        }
        .name-container{
            display: grid;
            grid-template-columns: 1fr 1fr;
            column-gap: 1vw;
            align-items: center;
            justify-content: center;
            width: 25vw;
        }
        .first-name-input, .last-name-input{
            width:11vw;
        }
        .container{
            width: 25px;
           
        }
        input, textarea{
            width:25vw;
        }
    }
</style>