<script>
  import t8 from "$lib/images/t8.webp";
</script>

<svelte:head>
  <title>About</title>
  <meta name="description" content="About TCreative Lab" />
</svelte:head>

<section class="bio-section">
  <div class="bio-text">
    <br />
    <h2>CONTENT CREATION</h2>
    <br />
    <p>
      Crafting high-quality, engaging visuals, videos, and designs tailored to
      your brand’s aesthetic and goals.
    </p>

    <br />
    <br />
    <h2>SOCIAL MEDIA MARKETING</h2>
    <br />
    <p>
      Strategically managing your social media profiles to increase audience
      engagement, grow your community, and ensure consistent branding. From
      content planning to analytics, we handle it all to amplify your online
      presence.
    </p>

    <br />
    <br />
    <h2>DESIGN & BRANDING</h2>
    <br />
    <p>
      Building and refining your brand identity with cohesive storytelling,
      thoughtful design, and consistent messaging. From logo creation to full
      brand guidelines, we help define who you are and how you’re perceived.
    </p>

    <br />
    <br />
    <h2>AD CAMPAIGN MANAGEMENT</h2>
    <br />
    <p>
      Creating, optimizing, and monitoring ad campaigns on platforms like
      Instagram, Facebook, and TikTok to maximize your ROI. We help your brand
      target the right audience for measurable results.
    </p>

    <br />
    <br />
    <h2>INFLUENSER COLLABORATIONS</h2>
    <br />
    <p>
      Partnering with influencers to authentically expand your brand's reach and
      credibility. We connect you with the right voices to tell your story
      effectively.
    </p>

    <br />
    <br />
    <h2>WEBSITE DEVELOPMENT</h2>
    <br />
    <p>
      Creating modern, user-friendly websites that showcase your brand’s
      identity, engage your audience, and drive results.
    </p>

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
    z-index: 10;
  }
  img {
    position: fixed;
    z-index: 0;
    opacity: 50%;
  }

  .bio-text {
    width: 30%;
    z-index: 10;
    margin-top: 7em;
  }
  h2 {
    letter-spacing: 0.1em;
    text-align: left;
  }

  p {
    font-size: 0.9em;
    letter-spacing: 0.1em;
    font-weight: 50;
    word-spacing: 0.15em;
    text-align: justify;
  }
  @media (max-width: 768px) {
    .bio-text {
      width: 80%;
      margin-top: 5em;
    }
    h1 {
      margin-bottom: 2em;
    }
  }
</style>
