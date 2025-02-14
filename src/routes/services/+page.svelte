<script lang="ts">
  import { albums, albumSongs } from "./musicData";
  import Socials from "./Socials.svelte";

  let albumSongsLocal = albumSongs;

  function toggleActive(albumId: number, id: number) {
    albumSongsLocal.find(
      (x) => x.albumId === albumId && x.id === id
    )!.isActive = !albumSongsLocal.find(
      (x) => x.albumId === albumId && x.id === id
    )!.isActive;
    albumSongsLocal = [...albumSongsLocal]; // Trigger reactivity
  }
</script>

<svelte:head>
  <title>Muzika</title>
  <meta name="description" content="Diskografija Lexington benda" />
</svelte:head>

<section>
  {#each albums as album}
    <div class="album">
      <h2>{album.name}</h2>
      <div class="album-songs">
        {#each albumSongsLocal.filter((x) => x.albumId === album.id) as song, i}
          <div class="album-song">
            <p>{i + 1}.</p>
            <div class="song-button">
              <button
                type="button"
                on:click={() => toggleActive(song.albumId, song.id)}
              >
                <p>{song.name}</p></button
              >
              {#if song.isActive}
                <div class="extra-info">
                  <Socials {song} />
                  <div class="lyrics-credits">
                    <a href="/music/song?id={song.id}&lyrics">LYRICS</a>
                    <p>/</p>
                    <a href="/music/song?id={song.id}&credits">CREDITS</a>
                  </div>
                </div>
              {/if}
            </div>
          </div>
        {/each}
      </div>
    </div>
  {/each}
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    width: 100%;
    color: whitesmoke;
    justify-content: center;
    margin-top: 7em;
  }

  section,
  p,
  h2 {
    text-transform: uppercase;
    font-size: 0.9em;
  }

  h2 {
    margin-bottom: 1em;
    border-bottom-width: 1px;
    border-color: white;
  }

  .album {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 5em;
  }

  .album-songs {
    display: flex;
    flex-direction: column;
    row-gap: 1em;
    width: 90%;
  }

  .album-song {
    display: flex;
    width: 100%;
    justify-content: space-between;
  }

  .song-button {
    display: flex;
    flex-direction: column;
    align-items: end;
    row-gap: 0.5em;
  }

  .extra-info {
    display: flex;
    flex-direction: column;
    row-gap: 0.2em;
    align-items: end;
    margin-bottom: 0.1em;
  }

  .lyrics-credits {
    display: flex;
    align-items: center;
    font-size: 0.7em;
    letter-spacing: 0.1em;
    margin-top: 3px;
  }

  @media (max-width: 768px) {
    section {
      margin-top: 5em;
    }
    p {
      font-size: 0.8em;
    }
  }
</style>
