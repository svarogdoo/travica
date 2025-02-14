<script lang="ts">
  export let tourData = {
    title: "",
    date: "",
    ticketLink: "",
  };
  export let photo;
</script>

<section class="card">
  <img src={photo} alt="Tour image" />
  <div class="content">
    <h2>{tourData.title}</h2>
    <p>{tourData.date}</p>
    <a href={tourData.ticketLink}>Karte</a>
  </div>
</section>

<style>
  .card {
    display: flex;
    flex-direction: column;
    background: #111111;
    color: white;
    width: 100%;
  }
  img {
    max-height: 600px;
    object-fit: cover;
  }
  .content {
    display: flex;
    flex-direction: column;
    margin-top: 10px;
    align-items: center;
  }
  h2 {
    letter-spacing: 0.2em;
    font-size: medium;
    margin-bottom: 5px;
    text-transform: uppercase;
    font-size: 0.8em;
  }
  p {
    letter-spacing: 0.2em;
    font-size: 0.8em;
  }
  a {
    margin-top: 10px;
    margin-bottom: 10px;
    letter-spacing: 0.2em;
    border-bottom: 1px solid #ffffff;
    padding-left: 5px;
    padding-right: 3px;
    padding-bottom: 3px;
    font-size: 0.8em;
  }
</style>
