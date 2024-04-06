<script>
  const name = "Vishwas";
  const html = "<h1>Hello World</h1>";
  const disabled = "true";
  const green = true;
  const red = "red";
  const underline = "red";
  const number = 3;
  const isPromoted = true;
</script>

<main>
  <h1>Hello {@html html}</h1>
  <button {disabled}>Bind</button>
  <button class={green ? number > 2 : underline}>Button</button>
  <h2 class:promoted={isPromoted}>Flapjack!</h2>
</main>

<style>
  .red {
    color: red;
  }
  .green {
    color: green;
  }

  .promoted {
    color: purple;
  }

  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
