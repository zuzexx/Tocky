<script>
  export let containers = [
    {
      icon: "images/flexible_plans.png",
      header: "Flexible plans",
    },
    {
      icon: "images/targeted_audience.png",
      header: "Targeted audience",
    },
    {
      icon: "images/content_management.png",
      header: "Content management",
    },
    {
      icon: "images/organic_growth.png",
      header: "Organic followers",
    },
    {
      icon: "images/security.png",
      header: "Advanced security",
    },
    {
      icon: "images/support.png",
      header: "24/7 support",
    },
  ];

  export let paragraphs = [
    {
      text: "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.",
    },
  ];
</script>

<div class="container">
  <div class="text-container">
    <h2>We help you get to the top!</h2>
    <p class="paragraph">
      Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo
      ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis
      dis parturient montes, nascetur ridiculus mus.
    </p>
  </div>

  <div class="how-container">
    {#each containers as container}
      <div class="inner-container">
        <img src={container.icon} alt="icon" class="icon" />
        <h3>{container.header}</h3>
        {#each paragraphs as paragraph}
          <p>{paragraph.text}</p>
        {/each}
      </div>
    {/each}
  </div>
</div>

<style>
    .container{
        margin:auto;
        text-align: center;
        width: 80vw;
        margin-top: 9rem;
    }
    .how-container{
        width:80vw;
        display: grid;
        justify-content: center;
        align-items: center;
        grid-template-columns: 1fr 1fr;
        row-gap: 2rem;
    }
  .icon {
    width: 50px;
  }
  .inner-container p{
        max-width: 250px;
        margin: auto;
    }
    p{
      color:var(--paragraph);
      font-size: 0.9rem;
    }


  @media only screen and (min-width: 1200px) {
    .container{
       
        width: 50vw;
    }
    .how-container{
        width:50vw;
        
        grid-template-columns: 1fr 1fr 1fr;
        
    }
    p{
      font-size: 1rem;
    }
    .paragraph{
      max-width:800px;
      margin: auto;
    }
    
  }
</style>
