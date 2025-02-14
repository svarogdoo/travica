<script>
  import t1 from "$lib/images/t1.jpeg";
</script>

<svelte:head>
  <title>About</title>
  <meta name="description" content="About TCreative Lab" />
</svelte:head>

<section class="bio-section">
  <!-- TODO use t8 but as webp -->
  <img class="mob" src={t1} alt="Lexington background" />
  <img class="desk" src={t1} alt="Lexington background" />
  <div class="bio-text">
    <h1>Who We Are?</h1>

    <p>
      We’re not your typical marketing agency. T Creative Lab started as a group
      of friends who shared a deep passion for aesthetics, social media, and
      storytelling. Long before we even called it a business, we were creating
      content for ourselves, constantly experimenting with visuals, captions,
      and strategies. Our social media pages became our creative playground, a
      place where we crafted stories, shared ideas, and refined our skills. And
      then, something interesting happened—we started getting noticed.
    </p>

    <br />
    <p>
      It began with a simple question: “Who manages your page?” Friends, local
      business owners, and even complete strangers started reaching out, asking
      us to help them with their brands. One client turned into another, then
      another. Before we knew it, we had built something real, something
      exciting. And the best part? We were loving every second of it.
    </p>

    <br />
    <p>
      From restaurants and bars to streetwear brands, DJs, and small businesses,
      we’ve worked with people who share our vision: to stand out. Every brand
      has a story, and our job is to bring it to life through custom-made
      creative solutions. No generic templates. No one-size-fits-all strategies.
      We dive deep into what makes your brand unique and craft content that
      speaks directly to your audience.
    </p>

    <br />
    <p>
      Branding isn’t just about a cool logo or catchy slogan—it’s about creating
      a feeling. A vibe. Something people connect with and remember. That’s
      where we come in. We mix creativity with strategy, aesthetics with
      engagement, and turn ideas into scroll-stopping content. We help brands
      define their voice, build a strong identity, and connect with the right
      audience in a way that feels authentic.
    </p>

    <br />
    <p>
      Our approach is personal. We don’t believe in cookie-cutter marketing
      plans. Instead, we develop tailor-made strategies that reflect your
      brand’s essence. Whether it’s a sleek rebrand, a social media glow-up, or
      a full-scale content strategy, we make sure your brand doesn’t just
      exist—it thrives. We take the time to understand your goals, your
      audience, and your industry to craft something that’s not only visually
      stunning but also effective in driving engagement and growth.
    </p>

    <br />
    <p>
      Our core values? Creativity, dedication, and a personal approach. We
      believe that great branding is more than just aesthetics—it’s about
      storytelling, connection, and strategy. And most importantly, it’s about
      making sure your brand gets the recognition it deserves.
    </p>

    <br />
    <p>
      Want something truly custom-made for your business? Let’s create something
      amazing together. Let’s build your brand in a way that stands out,
      resonates, and lasts.
    </p>

    <br />
    <p>— Uroš Travica, Founder</p>
    <a href="https://www.instagram.com/travica_/"><p>@travica_</p></a>

    <br />
    <br />
  </div>
</section>

<style>
  section {
    color: whitesmoke;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    /* text-transform: uppercase; */
    z-index: 10;
  }
  img {
    position: fixed;
    z-index: 0;
    opacity: 30%;
  }
  .mob {
    display: none;
  }
  .bio-text {
    width: 40%;
    z-index: 10;
    margin-top: 7em;
  }
  h1 {
    margin-bottom: 2em;
    font-size: 1em;
    text-align: left;
  }
  h2,
  h3 {
    font-size: 0.8em;
    letter-spacing: 0.1em;
    font-weight: 500;
    word-spacing: 0.2em;
    margin-top: 0.4em;
  }
  p,
  li,
  span {
    font-size: 0.8em;
    letter-spacing: 0.1em;
    font-weight: 50;
    word-spacing: 0.15em;
  }
  @media (max-width: 768px) {
    .bio-text {
      width: 90%;
      margin-top: 5em;
    }
    h1 {
      margin-bottom: 2em;
    }
    .desk {
      display: none;
    }
    .mob {
      display: block;
    }
  }
</style>
