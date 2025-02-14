<script>
  import Header from "./Header.svelte";
  import "./styles.css";
</script>

<div class="app">
  <Header />

  <main>
    <slot />
  </main>

  <footer>
    <p>© TCREATIVELAB</p>
  </footer>
</div>

<style>
  .app {
    display: flex;
    flex-direction: column;
    height: 100%;
    width: 100%;
    background-color: black;
    align-items: center;
  }

  main {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
  }

  footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: fixed;
    bottom: 2em;
    font-size: 0.5em;
    letter-spacing: 0.1em;
    color: rgb(228, 228, 228);
  }

  @media (max-width: 768px) {
    footer {
      bottom: 1.6em;
    }
  }
</style>
