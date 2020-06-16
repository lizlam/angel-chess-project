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
   
        img {
                border: 2px solid lightgrey;
                padding: 4px;
                border-radius: 4px;
        }

        .container {
                display: grid;
                grid-template-columns: 1fr 1fr;
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
9x8 boards are not too common but <a href="https://a4games.company/">A4 Games</a> has graciously made a print and play version available. You can download them here as well.</p>	

<p>Note: The downloads for the pieces contain extra pawns and bishops for playing other chess variations.</p>

        <div class="container">
          <div class="board">
            <a href="chess-board-9x8-1.pdf">PDF for the board</a>. <br />
	    <img alt="9x8 board" width="300" src="chessboard-9x8.png" />
          </div>

          <div class="pieces">
             <a href="chess-pieces-embossed.pdf">PDF for traditional pieces</a>. <br />
	    <img alt="9x8 board" width="300" src="pieces-traditional.png" />
            <br />
        
            <a href="chess-pieces-stylized-3.pdf">PDF for stylized pieces</a>. <br />
	    <img alt="9x8 board" width="300" src="pieces-styled.png" />
          <div>
        </div>
	
</main>
