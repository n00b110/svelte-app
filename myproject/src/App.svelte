<script>
  const name = "Vishwas";
  const html = "<h1>Hello World</h1>";
  const disabled = "true";
</script>

<main>
  <h1>Hello {@html html}</h1>
  
  <button {disabled}>Bind</button>
</main>

<style>
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
