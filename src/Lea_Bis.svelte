<script>
    import {onMount} from 'svelte';
    
    onMount(() => {
        let image = document.getElementById('imageTest');
        image.style.display = 'none';
    });


    let src = 'https://media.giphy.com/media/jOgRWnCyyRqLaCjHMS/source.gif';
    let imgAfterForm = '<img {src} alt="test"/>';

    let imgDisplay = 'none';

    function formToImage() {
        let image = document.getElementById('imageTest');
        let form = document.getElementById('form');

        if (image.style.display !== 'block') {
            form.style.display = 'none';
            image.style.display = 'block';
        }


    }

    let nomFormation = 'LP CréaWeb';
    let lieuFormation = 'IUT LENS';
    let bacDebut = 'Bac +2 minimum';
    let bacSortie = 'Bac +3';
    let modalites = 'Alternance ou continu avec stages';


</script>


<hr>
<div id="both">
    <div id="left">
        <h1 id="nomFormation">{nomFormation}</h1>
        <h1 id="lieuFormation">{lieuFormation}</h1>
        <h1 id="bacDebut">{bacDebut}</h1>
        <h1 id="bacSortie">{bacSortie}</h1>
        <h1 id="modalites">{modalites}</h1>
    </div>

    <div id="right">
        <div id="form">
            <label for="changeFormation">Titre de la formation :</label>
            <input type="text" id="changeFormation" bind:value={nomFormation}/>

            <label for="changeLieu">Lieu de la formation :</label>
            <input type="text" id="changeLieu" bind:value={lieuFormation}/>

            <label for="changeDebut">Bac nécessaire pour la formation :</label>
            <input type="text" id="changeDebut" bind:value={bacDebut}/>

            <label for="changeSortie">Bac à la sortie de formation :</label>
            <input type="text" id="changeSortie" bind:value={bacSortie}/>

            <label for="changeModalites">Modalités de la formation :</label>
            <input type="text" id="changeModalites" bind:value={modalites}/>
            <br/>
            <button on:click={formToImage}>Submit</button>
        </div>
        <img {src} alt="test" id="imageTest"/>
    </div>
</div>

<style>
    div {
        margin: 10px;
        padding: 10px;
    }

    #both {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        margin: auto;
    }

    #left {
        background: wheat;
        width: 60%;
    }

    #right {
        background: cadetblue;
        width: 40%;
    }

    #image {
        /*display: none;*/
    }
</style>
