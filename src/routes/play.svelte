<script>
    import { fade } from 'svelte/transition';
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		font-size: 1.5em;
		max-width: 440px;
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
	<title>Play</title>
</svelte:head>

<main in:fade>
	<h1>Play</h1>
	<p>The easiest way to start playing Angel Chess is to make a board and use a regular set of chess pieces. You will need 2 extra pawns and 2 extra pieces to represent the Angels.<br /><br />
9x8 boards are not too common but <a href="https://a4games.company/">A4 Games</a> has graciously made a print and play version available. You can download the <a href="chess-board-9x8-1.pdf">PDF</a> here as well.</p>	
	<img alt="9x8 board" width="300" src="chessboard-9x8.png" />
	
</main>
