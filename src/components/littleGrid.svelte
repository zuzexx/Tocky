<script>
     export let statistics = [
    {
      number: "20,000+" ,
      text: "satisfied customers",
      
    },
    {
      number: "5,823" ,
      text:"New Monthly Followers" ,
      
    },
    {
      number: "4.9 / 5" ,
      text: "Trustpilot score" ,
      
    },
    {
      number: "169%"  ,
      text: "More engagement" ,
      
    },
    
  ];
</script>

<div class="grid-container">
    {#each statistics as statistic}
    <div class="inner-container">
        <h2>{statistic.number}</h2>
        <p>{statistic.text}</p>
    </div>
    {/each}

</div>
 <style>
    .grid-container{
        width: 80vw;
        display: grid;
        justify-content: center;
        align-items: center;
        margin: auto;
        text-align: center;
        text-transform: capitalize;
        border-radius: 10px;   
    }
   
    p{
      color: var(--button-hover);
      font-size: 0.9rem;
      font-weight: var(--light);
    }
    .inner-container{
        border-bottom: 1px solid var(--header-span);
    }
    @media only screen and (min-width: 800px) {
    .grid-container{
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr;
    }
    h2{
      font-size: 1.3rem;
    }
    p{
      font-size: 1rem;
    }
    
  }
  @media only screen and (min-width: 1200px) {
    .grid-container{
        grid-template-rows: 1fr;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        width: 50vw;
        margin: auto;
        margin-top: 6rem;
    }
    h2{
      font-size: 1.5rem;
    }
    p{
      font-size: 1.2rem;
    }
    .inner-container{
        border-bottom: none;
        border-left: 1px solid var(--header-span);
        border-right: 1px solid var(--header-span);
    }
    
    
}
 </style>