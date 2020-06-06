<script>
    import { fade } from 'svelte/transition';
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		font-size: 1.5em;
		max-width: 540px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>

<svelte:head>
	<title>Angel Chess</title>
</svelte:head>

<main in:fade>
	<h1>Angel Chess</h1>
	<p>Angel Chess is a chess variation created in the early 1900's by <br /> Louis P. d'Autremont.</p>
        <img alt="Angel Chess Patent" src="angel_chess_patent.png" />
        <p>It is played on a 9x8 board with an extra pawn and Angel piece.<br />  
          The Angel moves like a Queen and Knight with some special rules around capturing. <br /><br />
          This site is dedicated to the exploration of this game. </p>
</main>