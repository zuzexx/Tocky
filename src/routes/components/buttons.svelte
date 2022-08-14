<button on:click>
  <slot />
</button>

<style>
  button {
    border: none;
    border-radius: 50px;
    width: 10rem;
    height: 3rem;
    /*background-color: var(--button-color);*/
    background: linear-gradient(
        to left,
        var(--button-color) 50%,
        var(--button-hover) 50%
      )
      right;
    color: var(--button-hover);
    background-size: 200% 100%;
    font-family: var(--font-family);
    font-weight: var(--regular);
    font-size: 0.8rem;
  }
  button:hover {
    cursor: pointer;
    /*background-color: var(--button-hover);*/
    border: 2px solid var(--button-color);
    color: var(--button-color);
    background-position: left;
    transition: all 0.7s linear;
    font-weight: var(--semi-bold);
  }

  @media only screen and (min-width: 1200px) {
    button {
      width: 14rem;
      height: 3rem;
      font-size: 1rem;
    }
  }
</style>
