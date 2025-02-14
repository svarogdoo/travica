<script lang="ts">
  import TourCard from "./TourCard.svelte";
  import { tourCards } from "./tourData";
  import tour1 from "$lib/images/tour1.jpg";
  import tour2 from "$lib/images/tour2.jpg";
</script>

<svelte:head>
  <title>Turneja</title>
  <meta name="description" content="Informacije o turneji Lexington benda" />
</svelte:head>

<section class="tour">
  <div class="tour-cards">
    <TourCard tourData={tourCards[0]} photo={tour1} />
    <TourCard tourData={tourCards[1]} photo={tour2} />
    <TourCard tourData={tourCards[0]} photo={tour1} />
    <TourCard tourData={tourCards[1]} photo={tour2} />
    <TourCard tourData={tourCards[0]} photo={tour1} />
  </div>
</section>

<style>
  .tour {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
  }
  .tour-cards {
    width: 90%;
    margin-top: 7em;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: center;
    gap: 100px;
  }
  @media only screen and (max-width: 1024px) {
    .tour-cards {
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
      row-gap: 20px;
      column-gap: 20px;
      margin-top: 4em;
    }
  }
</style>
