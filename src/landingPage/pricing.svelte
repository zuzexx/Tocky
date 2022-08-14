<script>
    import Buttons from "../components/buttons.svelte";

    export let text = "Li Europan lingues es membres del sam familie.";
    export let image = "images/check.png"

</script>
<div class="containers">
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
</div>


<style>
    .price{
        color:var(--header-span);
        font-weight: var(--bold);
        font-size: 1.5rem;
    }
    .price span{
        font-weight: var(--medium);
        font-size: 1rem;
        color:var(--light-paragraph);
        text-transform: lowercase;
    }
    li{
        color: var(--little-grid);
    }
    .containers{
        width:100vw;
    }
    .premium-container h3{
        color:var(--button-hover);
    }
    .all-prices:hover .container {
  filter: blur(1px);
    -webkit-transition: all 1s ease;
    -moz-transition: all 1s ease;
    -o-transition: all 1s ease;
    -ms-transition: all 1s ease;
    transition: all 1s ease;
    transform: scale(0.9);
}

.all-prices .container:hover {
    filter:blur(0);
    -webkit-transition: all 1s ease;
    -moz-transition: all 1s ease;
    -o-transition: all 1s ease;
    -ms-transition: all 1s ease;
    transition: all 1s ease;
    transform: scale(1.05);
}
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
        margin: auto;
        margin-top: 8rem;
        width:80vw;
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
        .price{
            font-size: 2.5rem;
        }
        
    }
</style>


