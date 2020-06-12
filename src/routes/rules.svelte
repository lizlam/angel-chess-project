<script>
    import { fade } from 'svelte/transition';
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		font-size: 1.5em;
		max-width: 340px;
		margin: 0 auto;
	}

	li {
		text-align: left;
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
	<title>Rules</title>
</svelte:head>
<main in:fade>
	<h1>Rules</h1>
	<p>A common way to enhance the traditonal game of chess is by adding more powerful pieces to the board we are all so familiar with. 

	Angel Chess is played on a 9x8 board and adds a powerful Angel piece with the combination move of a Queen and a Knight.  There is also an additional
	pawn that stands "guard" in front of it as well.<br /><br /> Most rules of the basic game applies with the following differences:
    </p>
    <ul>
       <li>The Angel piece sits to the right of the King.</li>
	   <li>Pawn promotion to Angel on e-file only. (the King's lane)</li>
	   <li>When Queen castling, the King goes to the Knight's square.</li>
	   <li>When King castling, the King goes to the Bishop's square.</li>
       <li>You can not capture the opposing side's Angel if your Angel piece will be captured on the following move. (No Angel for Angel sacrifice)</li>
	   <li>Supplementary: The Angel piece can not check from a square where it can be taken by any piece except the King.</li>
	</ul>

	
</main>
