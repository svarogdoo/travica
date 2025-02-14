<script lang="ts">
  import Socials from "../Socials.svelte";
  import { albumSongs, type Song } from "../musicData";
  import { onMount } from "svelte";

  let songId: any;
  let credits = false;
  let lyrics = true;
  let song: Song = {
    albumId: 0,
    id: 0,
    name: "",
    spotify: "",
    deezer: "",
    apple: "",
    youtube: "",
    isActive: false,
    lyrics: "",
    credits: "",
  };

  onMount(() => {
    const params = new URLSearchParams(window.location.search);
    credits = params.get("credits") !== null ? true : false;
    lyrics = params.get("lyrics") !== null ? true : false;
    songId = params.get("id");

    song = albumSongs.find((song) => song.id == songId) ?? song;
  });

  function handleLyricsAndCredits() {
    credits = !credits;
    lyrics = !lyrics;
  }
</script>

<section>
  <Socials {song} />
  <div class="lyrics-credits">
    <button on:click={handleLyricsAndCredits} class:underline={lyrics}
      >LYRICS</button
    >
    <p>/</p>
    <button on:click={handleLyricsAndCredits} class:underline={credits}
      >CREDITS</button
    >
  </div>
  <h1>{song?.name}</h1>
  {#if lyrics}
    <p class="lyrics">{@html song?.lyrics}</p>
  {/if}
  {#if credits}
    <p class="credits">{@html song?.credits}</p>
  {/if}
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    width: 100%;
    align-items: center;
    row-gap: 1em;
    margin-top: 7em;
    color: white;
    margin-bottom: 12em;
    text-transform: uppercase;
    font-size: 0.8em;
  }

  h1 {
    text-transform: uppercase;
    letter-spacing: 0.2em;
    font-size: 1em;
    margin-top: 2em;
    margin-bottom: 1em;
  }

  .lyrics-credits {
    display: flex;
    align-items: center;
    font-size: 0.8em;
    letter-spacing: 0.1em;
    margin-top: 3px;
    column-gap: 0.2em;
  }

  .underline {
    text-decoration: none;
    position: relative;
  }

  .underline:after {
    position: absolute;
    height: 0.8px;
    margin: 0 auto;
    content: "";
    left: 0;
    right: 0;
    width: 90%;
    color: #000;
    background-color: white;
    left: -4px;
    bottom: -2px;
  }

  .lyrics,
  .credits {
    display: flex;
    flex-direction: column;
    text-wrap: wrap;
    text-align: center;
    white-space: pre-line;
    margin-bottom: 1em;
  }

  @media (max-width: 768px) {
    section {
      margin-top: 5em;
    }
    h1 {
      font-size: 0.8em;
    }
    p {
      font-size: 0.75em;
    }
  }
</style>
