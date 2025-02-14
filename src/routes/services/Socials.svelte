<script lang="ts">
  import SpotifyIcon from "$lib/icons/Spotify.svelte";
  import DeezerIcon from "$lib/icons/Deezer.svelte";
  import YoutubeIcon from "$lib/icons/Youtube.svelte";
  import AppleIcon from "$lib/icons/Apple.svelte";

  export let song = {
    spotify: "",
    deezer: "",
    youtube: "",
    apple: "",
  };
</script>

<div class="social-links">
  <a href={song.spotify} target="_blank"> <SpotifyIcon /></a>
  <a href={song.deezer} target="_blank">
    <DeezerIcon />
  </a>
  <a href={song.youtube} target="_blank">
    <YoutubeIcon />
  </a>
  <a href={song.apple} target="_blank"> <AppleIcon /></a>
</div>

<style>
  .social-links {
    display: flex;
    justify-content: center;
    align-items: center;
    column-gap: 0.5em;
  }
</style>
