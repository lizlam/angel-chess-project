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
	<title>Angel Chess</title>
</svelte:head>

<main in:fade>
	<h1>About</h1>
	<p>Most of what know about Angel Chess is from Louis P. d'Autremont's <a href="angel_chess_patent_v1.pdf">patent</a>.</p>
        <img alt="Angel Chess Patent" src="patent_page1.png" />
       
        <p>Angel Chess also makes a small appearance in Chapter 14 of The Classified Enclopedia of Chess 
        Variants by David Pritchard.  The book is now out of print but is available in PDF form on
        <a href="http://www.jsbeasley.co.uk/">John and Sue Beasley's Website</a>. </p>

        <img alt="Encyclopedia excerpt" width="300" src="angel_chess_encyc_entry.png" />
</main>      
