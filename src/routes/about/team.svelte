<script>
  export let teams = [
    {
      image: "./images/team6.jpg",
      name: "John Deer",
      position: "Manager",
    },
    {
      image: "./images/team2.jpg",
      name: "Brad Pitt",
      position: "Team Leader",
    },
    {
      image: "./images/team3.jpg",
      name: " george Clooney",
      position: "Growth Specialist",
    },
    {
      image: "./images/team4.jpg",
      name: "Max Mad",
      position: "Head of Marketing",
    },
    {
      image: "./images/team5.jpg",
      name: "Eva Dark",
      position: "Sales Manager",
    },
    {
      image: "./images/team1.jpg",
      name: "Liv Big",
      position: "Customer Support",
    },
  ];
</script>

<div class="container">
  <div class="text-container">
    <h1>Meet the dream team!</h1>
    <p>
      molestias excepturi sint occaecati cupiditate non provident, similique
      sunt in culpa qui officia deserunt mollitia animi, id est laborum et
      dolorum fuga.
    </p>
  </div>
  <div class="grid">
    {#each teams as team}
      <div class="inner-container">
        <img src={team.image} alt="worker" />

        <h3>{team.name}</h3>
        <h4>{team.position}</h4>
      </div>
    {/each}
  </div>
</div>

<style>
  .grid {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    width: 80vw;
    margin: auto;
  }
  img {
    border-radius: 30px;
    width: 200px;
  }
  img:hover {
    cursor: pointer;
    border-left: 2px solid var(--header-border-top);
    border-bottom: 2px solid var(--header-border-bottom);
  }
  .container {
    width: 80vw;
    margin: auto;
    margin-top: 6rem;
    text-align: center;
  }
  h1 {
    color: var(--header);
    font-size: 1.5rem;
  }
  p {
    font-size: 1.1rem;
    color: var(--paragraph);
  }
  h4 {
    color: var(--header-span);
    font-size: 1rem;
  }

  @media only screen and (min-width: 600px) {
    .grid {
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr;
    }
    img {
      width: 250px;
    }
  }

  @media only screen and (min-width: 800px) {
    .grid {
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr;
    }
  }

  @media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
    }
    .grid {
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr 1fr;
      width: 50vw;
      margin: auto;
    }

    p {
      font-size: 1.4rem;
    }
    h1 {
      font-size: 1.9rem;
    }
  }

  @media only screen and (min-width: 1500px) {
    img {
      width: 300px;
    }
  }
</style>
