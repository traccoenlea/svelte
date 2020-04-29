<h1>Test du home</h1>

<style>
    * {
       box-sizing: border-box;
       margin: 0;
       padding: 0;
    }


	html, body {
	    height: 100%;
	    width: 100%;
	}

</style>
<svelte:head>
	<title>Home</title>
</svelte:head>

<h1>Great success!</h1>

<figure>
	<img alt="Borat" src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1051&q=80">
	<figcaption>HIGH FIVE!</figcaption>
</figure>

<p><strong>Try editing this file (routes/index.html) to test hot module reloading.</strong></p>

<style>
	h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}
	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}
	figure {
		margin: 0 0 1em 0;
	}
	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}
	p {
		margin: 1em auto;
	}
	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>
