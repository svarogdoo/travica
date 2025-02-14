<svelte:head>
  <title>Portfolio</title>
  <meta name="description" content="Portfolio" />
</svelte:head>

<section class="portfolio-section">
  <div class="portfolio-text">
    <br />
    <h1>LOOKING FOR INSPIRATION?</h1>
    <br />
    <p>
      Check out our work on Instagram! We specialize in creating standout
      content for brands where aesthetics matter—urban coffee shops, DJs,
      events, design studios, fashion labels, and more.
    </p>

    <br />
    <div class="flex gap-x-2 justify-center">
      <a href="https://www.instagram.com/TCREATIVELAB/">@tcreativelab</a>
      <p>|</p>
      <a href="https://www.instagram.com/travica_/">@travica</a>
      <p>|</p>
      <a href="https://www.instagram.com/mali_dzin/">@mali_dzin</a>
    </div>
  </div>
</section>

<style>
  section {
    color: whitesmoke;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-bottom: 10em;
    align-items: center;
    z-index: 10;
  }

  .portfolio-text {
    width: 30%;
    z-index: 10;
    margin-top: 7em;
  }
  h1 {
    font-size: 1.8em;
    letter-spacing: 0.1em;
    text-align: center;
  }

  p,
  a {
    font-size: 1.2em;
    letter-spacing: 0.1em;
    font-weight: 50;
    word-spacing: 0.15em;
    text-align: justify;
  }
  @media (max-width: 768px) {
    .portfolio-text {
      width: 85%;
      margin-top: 5em;
    }

    h1 {
      font-size: 1em;
    }

    p,
    a {
      font-size: 0.9em;
      letter-spacing: 0.05em;
      font-weight: 50;
      word-spacing: 0.1em;
      text-align: justify;
    }
  }
</style>
