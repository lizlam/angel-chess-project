<script>
  import { fade } from "svelte/transition";
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    font-size: 1.5em;
    max-width: 940px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  .container {
    display: grid;
    width: 1000px;
    text-align: left;
    grid-template-areas:
      "image1 desc1"
      "desc2 image2"
      "desc3 image3";
    grid-gap: 10px;
  }

  img.image1 {
    border: 1px solid lightgrey;
    border-radius: 5px;
    grid-area: image1;
    grid-column: auto;
  }

  img.image2 {
    border: 1px solid lightgrey;
    border-radius: 5px;
    grid-area: image2;
  }

  img.image3 {
    border: 1px solid lightgrey;
    border-radius: 5px;
    grid-area: image2;
  }

  p.desc1 {
    grid-area: desc1;
  }

  p.desc2 {
    grid-area: desc2;
  }

  p.desc3 {
    grid-area: desc3;
  }

  @media (max-width: 768px) {
    .container {
      grid-template-areas:
        "image1"
        "desc1"
        "desc2"
        "image2"
        "desc3"
        "image3";
    }

    p {
      max-width: 700px;
    }
  }
</style>

<svelte:head>
  <title>Angel Chess</title>
</svelte:head>

<main in:fade>
  <h1>About</h1>
  <div class="container">
    <img class="image1" alt="Angel Chess Patent" src="patent_page1.png" />
    <p class="desc1">
      Most of what know about Angel Chess is from Louis P. d'Autremont's
      <a href="angel_chess_patent_v1.pdf">patent</a>
      . Among other things stated in the patent, his aim was to improve the game
      of chess by reaching the "thick of the game" more quickly. This would seem
      to coincide with the mobilization phase that basically starts the game 20
      moves in. He also wanted a game where the stronger player was able to
      defeat the weaker player more quickly. Having an extremely powerful piece
      like the "destroying angel" would certainly contribute to this goal. The
      patent has good insight on what motivated Louis P. d'Autremont to create
      this game and I would recommend to anyone interested to give it a read.
    </p>

    <p class="desc2">
      Angel Chess also makes a small appearance in
      <a href="ch14_encyc.pdf">Chapter 14</a>
      of The Classified Encyclopedia of Chess Variants by David Pritchard. The
      book is out of print but available in PDF form on
      <a href="http://www.jsbeasley.co.uk/">John and Sue Beasley's Website</a>
      . There seems to be a small descrepancy where Pritchard dates the game to
      1918 in oppose to the patent date of 1915. It's hard to say why without
      the leaflet or the British Chess Magazine referred to.
    </p>
    <img
      alt="Encyclopedia excerpt"
      width="300"
      class="image2"
      src="angel_chess_encyc_entry.png" />
    <p class="desc3">
      An even smaller appearance is made in the Notes sections of
      <a href="http://aworldofchess.com/">A World of Chess</a>
      by Rick Knowlton and Jean-Louis Cazaux.
    </p>
    <img
      alt="World of Chess Notes"
      width="300"
      class="image3"
      src="woc-notes-angelchess.png" />
  </div>
</main>
