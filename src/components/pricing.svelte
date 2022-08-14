<script>
    import Buttons from "./buttons.svelte";

    export let text = "Li Europan lingues es membres del sam familie.";
    export let image = "images/check.png"

</script>
<div class="all-prices">
    <div class="standard-container container">
        <h3>Standard</h3>
        <p class="price"> 69€ <span>/month</span></p>
        <ul>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            
        </ul>
        <Buttons>Get Started!</Buttons>
    
    </div>
    
    <div class="premium-container container">
        <h3>Premium</h3>
        <p class="price"> 169€ <span>/month</span></p>
        <ul>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
        </ul>
        <Buttons>Get Started!</Buttons>
    
    </div>
    
    <div class="business-container container">
        <h3>Business</h3>
        <p class="price"> 420€ <span>/month</span></p>
        <ul>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
        </ul>
        <Buttons>Get Started!</Buttons>
    
    </div> 
</div>

<style>
    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        border-radius: 10px;
        border:1px solid var(--header-span);
        width: 350px;
        margin: auto;
        padding: 2rem;
    }

    .all-prices{
        margin-top: 8rem;
    }
    .container:hover{
        transform: scale(1.1);
        transition: 0.7rem;
        cursor: pointer;
    }
    .premium-container{
        border:3px solid var(--header-border-bottom);
    }
    .image{
        height: 1rem;
        margin-right: 0.8rem;
    }
    ul{
        list-style-type: none;
    }

    @media only screen and (min-width: 1440px) {
        .all-prices{
            display: flex;
            justify-content: center;
            align-items: center;
            width: 50vw;
        }
        .container{
            width: 500px;
        }
    }
</style>


