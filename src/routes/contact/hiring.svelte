<script>
    import Buttons from "../components/buttons.svelte";
</script>

<div class="container">

    <h1>Want to help others achieve their dreams? <br> <span>We are hiring.</span></h1>

    <Buttons>Open positions</Buttons>

</div>


<style>
    span{
        color: var(--header-span);
    }
    h1{
        color:var(--header);
        font-size: 1.7rem;
        text-align: center;
    }
    .container{
        width:80vw;
        margin: auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 5rem;
    }

    @media only screen and (min-width:1200px){
        .container{
            width: 50vw;
        }
    }
</style>
