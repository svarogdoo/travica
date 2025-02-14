<script lang="ts">
  import t1 from "$lib/images/t1.jpeg";
  // import t2 from "$lib/images/t2.jpg";
  import t3 from "$lib/images/t3.jpeg";
  import t4 from "$lib/images/t4.jpeg";
  import t5 from "$lib/images/t5.jpeg";
  import t6 from "$lib/images/t6.jpeg";
  import t7 from "$lib/images/t7.jpeg";
  // import t8 from "$lib/images/t8.jpg";
  import t9 from "$lib/images/t9.jpeg";
</script>

<svelte:head>
  <title>TCreativeLab</title>
  <meta name="description" content="tington" />
</svelte:head>

<section>
  <div class="title">
    <h2><a href="/about">TCREATIVE LAB</a></h2>
  </div>
  <img class="first-photo opacity-70 min-h-screen" src={t1} alt="" />
  <img src={t3} alt="" />
  <!-- <img class="second-photo" src={t2} alt="" /> -->
  <img src={t4} alt="" />
  <img src={t5} alt="" />
  <img src={t6} alt="" />
  <img src={t7} alt="" />
  <!-- <img src={t8} alt="" /> -->
  <img src={t9} alt="" />
</section>

<style>
  section {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .title {
    display: flex;
    position: fixed;
    width: 100%;
    height: 100%;
    justify-content: space-around;
    letter-spacing: 0.3em;
    align-items: center;
    align-content: center;
    color: white;
    z-index: 20;
  }
  .second-photo {
    display: none;
  }

  /* @media (max-width: 768px) {
    .title {
      font-size: 0.9em;
    }
    .first-photo {
      display: none;
    }
    .second-photo {
      display: block;
    }
  } */
</style>
