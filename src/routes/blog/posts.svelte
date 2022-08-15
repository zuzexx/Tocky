<script>
  import { text } from "svelte/internal";

  export let datas = [
    {
      picture: "images/tiktok5.jpg",
      header: "Everything you need to know about TikTok",
      date: "Mar 16, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "What to post on TikTok",
      date: "Mar 10, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "5 Biggest TikTok Secrets",
      date: "Feb 12, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "A beginners guide to TikTok",
      date: "Feb 10, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "20 TikTok Tips",
      date: "Feb 8, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "How to run a TikTok Contest",
      date: "Feb 4, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "Everything you need to know about TikTok",
      date: "Mar 16, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "What to post on TikTok",
      date: "Mar 10, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "5 Biggest TikTok Secrets",
      date: "Feb 12, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "A beginners guide to TikTok",
      date: "Feb 10, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "20 TikTok Tips",
      date: "Feb 8, 2022",
    },
    {
      picture: "images/tiktok5.jpg",
      header: "How to run a TikTok Contest",
      date: "Feb 4, 2022",
    },
  ];

  export let texts = [
    {
      text: "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem.",
      icon: "images/rover-heathers.jpg",
      name: "Rover Heathers",
    },
  ];
</script>

<div class="container">
  <div class="text">
    <h1>Tocky Blog</h1>
    <p class="main-text">
      The quick, brown fox jumps over a lazy dog. DJs flock by when MTV ax quiz
      prog. Junk MTV
    </p>
  </div>
  <div class="grid-container">
    {#each datas as data}
      <div class="inner-container">
        <img src={data.picture} alt=" " class="pictures" />
        <div class="text">
          <h3>{data.header}</h3>
          {#each texts as text}
            <p class="inner-text">{text.text}</p>
            <div class="author-container">
              <img src={text.icon} alt="" class="icon" />

              <div class="author-text">
                <p class="name-p">{text.name}</p>
                <p class="date">{data.date}</p>
              </div>
            </div>
          {/each}
        </div>
      </div>
    {/each}
  </div>
</div>

<style>
  .container {
    width: 80vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin: auto;
    margin-top: 4rem;
  }
  p {
    color: var(--paragraph);
    font-size: 0.9rem;
  }
  h1 {
    color: var(--header);
    font-size: 1.3rem;
  }
  .grid-container {
    width: 80vw;
    margin-top: 4rem;
  }
  .pictures {
    width: 80vw;
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
  }
  .icon {
    width: 50px;
    border-radius: 20px;
  }
  .inner-container {
    text-align: left;
    width: 80vw;
    border-radius: 20px;
    border-left: 2px solid var(--header-border-top);
    border-top: 2px solid var(--header-border-top);
    border-right: 2px solid var(--header-border-bottom);
    border-bottom: 2px solid var(--header-border-bottom);
    margin-top: 2rem;
  }
  .inner-container:hover {
    opacity: 0.7;
    cursor: pointer;
    transform: scale(0.9);
    transition: 0.7rem;
  }
  .inner-text {
    font-size: 0.8rem;
  }
  .text {
    padding: 1rem;
  }

  @media only screen and (min-width: 700px) {
    .container {
      width: 50vw;
    }
    .grid-container {
      width: 50vw;
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr;
      column-gap: 2vw;
      row-gap: 2rem;
    }
    .inner-container {
      width: 23vw;
    }
    .pictures {
      width: 23vw;
    }
  }

  @media only screen and (min-width: 1700px) {
    .grid-container {
      width: 50vw;
      display: grid;
      justify-content: center;
      align-items: center;
      grid-template-columns: 1fr 1fr 1fr;
      column-gap: 2vw;
    }
    .inner-container {
      width: 15vw;
    }
    .pictures {
      width: 15vw;
    }
    .author-container {
      display: flex;
      flex-direction: row;
      justify-content: flex-start;
      align-items: center;
      width: 15vw;
      font-size: 0.4rem;
    }
    .author-text {
      margin-left: 1rem;
    }
  }
</style>
