<svelte:head>
	<title>ACCUEIL</title>
</svelte:head>

<script>
	import {onMount} from 'svelte';

    onMount(() => {
        let image = document.getElementById('imagehero');
        image.style.display = 'none';
    });


    let src = 'https://images.unsplash.com/photo-1504384764586-bb4cdc1707b0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80';
    let imgAfterForm = '<img {src} alt="hero"/>';

    let imgDisplay = 'none';

    function formToImage() {
        let image = document.getElementById('imagehero');
        let form = document.getElementById('form');

        if (image.style.display !== 'block') {
            form.style.display = 'none';
            image.style.display = 'block';
        }

    }
</script>

<article class="box">
	<h2>
		<slot>
			<span class="missing">LP CRÉAWEB: MÉTIERS DU NUMÉRIQUE: CONCEPTION, RÉDACTION ET RÉALISATION WEB</span>
		</slot>
	</h2>

	<div class="address">
		<slot>
			<span class="missing">IUT DE LENS</span>
		</slot>
	</div>

	<div class="langue">
		<slot>
			<span class="missing">FRANÇAIS</span>
		</slot>
	</div>

    	<div class="categorie">
		<slot>
			<span class="missing">ALTERNANCE</span>
		</slot>
	</div>

    	<div class="admission">
		<slot>
			<span class="missing">Admissible à : Bac+2</span>
		</slot>
	</div>

    	<div class="niveau">
		<slot>
			<span class="missing">Niveau de sortie:</span>
		</slot>
	</div>

    	<div class="temps">
		<slot>
			<span class="missing">536 heures d'enseignement dont 134 heures de projets</span>
		</slot>
	</div>
</article>

<style>
	.box {
		width: 300px;
		border: 1px solid #aaa;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		padding: 1em;
	}

	.box {
		padding: 0 0 0.2em 0;
		margin: 0 0 1em 0;
		border-bottom: 1px solid #ff3e00;
	}

	.address, .langue,.categorie,.admission, .niveau, .temps {
		padding: 0 0 0 1.5em;
		background:  0 50% no-repeat;
		background-size: 1em 1em;
		margin: 0 0 0.5em 0;
		line-height: 1.2;
	}

	.address { background-image: url(../icon/adresse.svg) }
	.langue   { background-image: url(../icon/language.svg) }
	.categorie { background-image: url(../icon/categorie.svg) }
	.admission   { background-image: url(../icon/admis.svg) }
	.niveau { background-image: url(../icon/niveau.svg) }
	.temps   { background-image: url(../icon/temps.svg) }
	.missing { color: #999 }

</style>
