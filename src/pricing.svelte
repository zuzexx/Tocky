<script>
    import Buttons from "./components/buttons.svelte";

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
    
    </div>
    
    <div class="business-container container">
        <h3>Business</h3>
        <p class="price"> 420€ <span>/month</span></p>
        <ul>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            <li><img src="{image}" alt="" class="image">{text}</li>
            
    
    </div> 
</div>

<style>
    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
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
    }
</style>


