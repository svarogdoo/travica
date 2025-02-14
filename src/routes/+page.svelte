<script lang="ts">
  import t1 from "$lib/images/t1.webp";
  import t2 from "$lib/images/t2.webp";
  import t3 from "$lib/images/t3.webp";
  import t4 from "$lib/images/t4.webp";
  import t5 from "$lib/images/t5.webp";
  import t6 from "$lib/images/t6.webp";
  import t7 from "$lib/images/t7.webp";
  import t8 from "$lib/images/t8.webp";
  import t9 from "$lib/images/t9.webp";
  import t91 from "$lib/images/t91.webp";
  import t92 from "$lib/images/t9.webp";
  import t93 from "$lib/images/t93.webp";
  import t94 from "$lib/images/t94.webp";
  import t95 from "$lib/images/t95.webp";
  import t96 from "$lib/images/t96.webp";
  import t97 from "$lib/images/t97.webp";
  import t98 from "$lib/images/t98.webp";
  import t99 from "$lib/images/t99.webp";
  import t991 from "$lib/images/t991.webp";
  import t992 from "$lib/images/t992.webp";
  import t993 from "$lib/images/t993.webp";
  import t994 from "$lib/images/t994.webp";
  import t995 from "$lib/images/t995.webp";
  import t996 from "$lib/images/t996.webp";
  import t997 from "$lib/images/t997.webp";
  import t998 from "$lib/images/t998.webp";
  import t999 from "$lib/images/t999.webp";
  import tlogo from "$lib/images/tclab-logo.svg";
</script>

<svelte:head>
  <title>TCreativeLab</title>
  <meta name="description" content="tington" />
</svelte:head>

<section>
  <div class="title">
    <a href="/about">
      <img src={tlogo} alt="TCREATIVE LAB" class="h-80 lg:h-96 w-auto" />
    </a>
    <!-- <h2><a href="/about">TCREATIVE LAB</a></h2> -->
  </div>
  <img class="first-photo opacity-60 min-h-screen" src={t1} alt="" />
  <img src={t3} alt="" />
  <img src={t4} alt="" />
  <img src={t5} alt="" />
  <img src={t8} alt="" />
  <img src={t6} alt="" />
  <img src={t7} alt="" />
  <img src={t9} alt="" />
  <img class="second-photo" src={t2} alt="" />
  <img src={t91} alt="" />
  <img src={t92} alt="" />
  <img src={t93} alt="" />
  <img src={t94} alt="" />
  <img src={t95} alt="" />
  <img src={t96} alt="" />
  <img src={t97} alt="" />
  <img src={t98} alt="" />
  <img src={t99} alt="" />
  <img src={t991} alt="" />
  <img src={t992} alt="" />
  <img src={t993} alt="" />
  <img src={t994} alt="" />
  <img src={t995} alt="" />
  <img src={t996} alt="" />
  <img src={t997} alt="" />
  <img src={t998} alt="" />
  <img src={t999} alt="" />
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
  /* .second-photo {
    display: none;
  } */

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
