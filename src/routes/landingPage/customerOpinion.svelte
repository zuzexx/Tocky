<script>
</script>

<div class="container">
  <div class="text-container">
    <h2>Become one of our satisfied customers</h2>
    <p class="text">
      Li Europan lingues es membres del sam familie. Lor separat existentie es
      un myth. Por scientie, musica, sport etc, litot Europa usa li sam
      vocabular.
    </p>

    <div class="grid-container">
      <div
        class="quote-container sarah"
        style="background-image: url('images/sarah-adrian-alvarez.jpg');"
      >
        <div class="inner-text">
          <h4 class="name-text">Sarah Adrian Alvarez</h4>

          <p class="inner-paragraph">
            "Li Europan lingues es membres del sam familie. Lor separat
            existentie es un myth. Por scientie, musica, sport etc, litot Europa
            usa li sam vocabular. Li lingues differe solmen in li grammatica, li
            pronunciation e li plu commun vocabules."
          </p>
        </div>
      </div>
      <div
        class="quote-container riley"
        style="background-image: url(images/riley-rogers.jpg);"
      >
        <div class="inner-text">
          <h4 class="name-text">Riley Rogers</h4>

          <p class="inner-paragraph">
            "Li Europan lingues es membres del sam familie. Lor separat
            existentie es un myth. Por scientie, musica, sport etc, litot Europa
            usa li sam vocabular. Li lingues differe solmen in li grammatica, li
            pronunciation e li plu commun vocabules."
          </p>
        </div>
      </div>

      <div
        class="quote-container"
        style="background-image: url(images/rover-heathers.jpg);"
      >
        <div class="inner-text">
          <h4 class="name-text">Rover Heathers</h4>

          <p class="inner-paragraph">
            "Li Europan lingues es membres del sam familie. Lor separat
            existentie es un myth. Por scientie, musica, sport etc, litot Europa
            usa li sam vocabular. Li lingues differe solmen in li grammatica, li
            pronunciation e li plu commun vocabules."
          </p>
        </div>
      </div>

      <div
        class="quote-container"
        style="background-image: url(images/genevive-thomdon.jpg);"
      >
        <div class="inner-text">
          <h4 class="name-text">Genevive Thomdon</h4>

          <p class="inner-paragraph">
            "Li Europan lingues es membres del sam familie. Lor separat
            existentie es un myth. Por scientie, musica, sport etc, litot Europa
            usa li sam vocabular. Li lingues differe solmen in li grammatica, li
            pronunciation e li plu commun vocabules."
          </p>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .container {
    width: 80vw;
    margin: auto;
    text-align: center;
    margin-top: 7rem;
  }
  .text {
    color: var(--paragraph);
    font-size: 0.9rem;
  }
  .quote-container {
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
  .quote-container:hover .inner-text {
    visibility: visible;
    opacity: 1;
  }
  .inner-text {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    flex-direction: column;
    text-align: left;
    width: 250px;
    margin: auto;
    color: var(--light-paragraph);
    opacity: 0;
    visibility: hidden;
    -webkit-transition: visibility 0s, opacity 0.5s linear;
    transition: visibility 0s, opacity 0.5s linear;
    background-color: var(--background);
    border-radius: 20px;
    padding: 1rem;
  }
  .quote-container:hover {
    cursor: crosshair;

    transition: 1s ease;
    transform: scale(1.05);
  }

  @media only screen and (min-width: 1200px) {
    .container {
      width: 50vw;
    }
    .grid-container {
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
    .text {
      font-size: 1rem;
    }
  }

  @media only screen and (min-width: 3050px) {
    .grid-container {
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
