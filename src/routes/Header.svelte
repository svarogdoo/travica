<script>
  import { page } from "$app/stores";
</script>

<header>
  <nav>
    <ul>
      {#if $page.url.pathname !== "/"}
        <li aria-current={$page.url.pathname === "/" ? "page" : undefined}>
          <a href="/">HOME</a>
        </li>
      {/if}
      {#if $page.url.pathname !== "/about"}
        <li aria-current={$page.url.pathname === "/about" ? "page" : undefined}>
          <a href="/about">ABOUT</a>
        </li>
      {/if}
      {#if $page.url.pathname !== "/services"}
        <li
          aria-current={$page.url.pathname === "/services" ? "page" : undefined}
        >
          <a href="/services">SERVICES</a>
        </li>
      {/if}
      {#if $page.url.pathname !== "/portfolio"}
        <li
          aria-current={$page.url.pathname === "/portfolio"
            ? "page"
            : undefined}
        >
          <a href="/portfolio">PORTFOLIO</a>
        </li>
      {/if}
      {#if $page.url.pathname !== "/contact"}
        <li
          aria-current={$page.url.pathname === "/contact" ? "page" : undefined}
        >
          <a href="/contact">CONTACT</a>
        </li>
      {/if}
    </ul>
  </nav>
</header>

<style>
  header {
    display: flex;
    width: 100%;
    max-width: 500px;
    justify-content: space-between;
    position: fixed;
    margin-top: 2.5em;
    padding: 0em 0.8em;
    z-index: 100;
  }

  nav {
    display: flex;
    width: 100%;
    justify-content: center;
  }

  ul {
    position: relative;
    display: flex;
    width: 100%;
    list-style: none;
    justify-content: space-around;
    align-items: center;
    color: whitesmoke;
    letter-spacing: 0.1em;
    font-size: 0.8em;
    max-width: 800px;
  }

  a:hover {
    color: white;
  }

  @media (max-width: 768px) {
    header {
      margin-top: 1.6em;
    }
  }
</style>
