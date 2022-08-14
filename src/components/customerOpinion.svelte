<script>
    import { fade } from 'svelte/transition'
	let show = false
	let status = false
	
	function toggleShow() {
		show = !show
	}

    export let customers = [
        {
            image:"images/sarah-adrian-alvarez.jpg",
            name:"Sarah Adrian Alvarez",
            
        },
        {
            image:"images/riley-rogers.jpg",
            name:"Riley Rogers",
           
        },
        {
            image:"images/rover-heathers.jpg",
            name:"Rover Heathers",
            
        },
        {
            image:"images/genevive-thomdon.jpg",
            name:"Genevive Thomdon",
           
        },
    ];

    export let opinions =[{
        opinion:"Li Europan lingues es membres del sam familie. Lor separat existentie es un myth. Por scientie, musica, sport etc, litot Europa usa li sam vocabular.  Li lingues differe solmen in li grammatica, li pronunciation e li plu commun vocabules.",
    }];

</script>

<div class="container">
    <div class="text-container">
        <h2>Become one of our satisfied customers</h2>
        <p class="text">Li Europan lingues es membres del sam familie. Lor separat existentie es un myth. Por scientie, musica, sport etc, litot Europa usa li sam vocabular.</p>

        <div class="grid-container">
            {#each customers as customer}
            <div class="quote-container" style="background-image: url({customer.image});" on:mouseenter={toggleShow}
            on:mouseleave={toggleShow} >
                
                    {#if show}
                    <div class="inner-text" transition:fade="{{ duration: 2000 }}"
                on:outrostart="{() => status = true}"
                on:outroend="{() => status = false}">
                <h4 class="name-text">{customer.name} </h4>
                {#each opinions as opinion}
                    <p class="inner-paragraph">{opinion.opinion}</p>
                {/each}
                </div>
                    {/if}
                
            </div>
            {/each}
        </div>
    </div>
</div>

<style>
    .container{
        width: 80vw;
        margin: auto;
        text-align: center;
        margin-top: 7rem;
    }
    .text{
        color: var(--paragraph);
        font-size: 0.9rem;
    }
    .quote-container{
        width: 25rem;
        height: 25rem;
        margin: auto;
        border-radius: 50%;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: fixed;
        margin-top: 2rem;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    .inner-text{
        display: flex;
        justify-content: center;
        align-items: flex-start;
        flex-direction: column;
        text-align: left;
        width: 250px;
        margin: auto;    
        color: var(--light-paragraph);
    }
    .quote-container:hover{
        cursor: crosshair;
        
        
    -webkit-filter: brightness(45%);
    -webkit-transition: all 1s ease;
    -moz-transition: all 1s ease;
    -o-transition: all 1s ease;
    -ms-transition: all 1s ease;
    transition: all 1s ease;
    transform: scale(1.05);
    }
   
    @media only screen and (min-width: 1200px) {
        .container{
            width: 50vw;
        }
        .grid-container{
            display: grid;
            justify-content: center;
            align-items: center;
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr;
            width: 50vw;
            margin: auto;
            row-gap: 1rem;
            column-gap: 1rem;
        }
        .text{
            font-size: 1rem;
        }
        
        
    }

    @media only screen and (min-width: 3050px) {
        
        .grid-container{
            display: flex;
            flex-direction: row;
            justify-content: space-evenly;
            align-items: center;
            width: 50vw;
            margin: auto;
            row-gap: 1rem;
            column-gap: 1rem;
        }
       
        
    }
</style>