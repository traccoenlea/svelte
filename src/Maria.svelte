<svelte:head>
	<title>ACCUEIL</title>
</svelte:head>

<script>
	import Box from './Box.svelte';
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

<Box>
	<h2>LP CRÉAWEB: MÉTIERS DU NUMÉRIQUE: CONCEPTION, RÉDACTION ET RÉALISATION WEB</h2>
	<li>IUT DE LENS</li>
	<li>FRANÇAIS</li>
	<li>ALTERNANCE</li>
	<li>Admissible à: Bac+2</li>
	<li>Niveau de sortie:</li>
	<br>
	<li>536 heures d'enseignement dont 134 heures de projets</li>
</Box>