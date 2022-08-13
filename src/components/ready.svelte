
<script>
    import Buttons from "./buttons.svelte";
</script>

<div class="container">
    <h2>Start your free trial today!</h2>
    <Buttons>I want a free trial!</Buttons>
</div>
<style>

    .container{
        width:80vw;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    @media only screen and (min-width: 1200px) {
        .container{
            width: 50vw;
        }
    }

</style>