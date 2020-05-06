<script>
    function openNav() {
        document.getElementById("sideForm").style.width = "500px";
    }

    function closeNav() {
        document.getElementById("sideForm").style.width = "0";
    }

    //MODIF FORMULAIRE

    let nomFormation = 'LP CréaWeb TEST';
    let lieuFormation = 'IUT LENS';
    let bacDebut = 'Bac +2 minimum';
    let bacSortie = 'Bac +3';
    let modalites = 'Alternance ou continu avec stages';
//    LP CRÉAWEB: MÉTIERS DU NUMÉRIQUE: CONCEPTION, RÉDACTION ET RÉALISATION WEB
</script>



<div class="toggle">
    <div on:click={openNav} class="color">Modifier la page</div>
</div>


<div id="sideForm" class="sideForm">
    <a href="javascript:void(0)" class="closebtn" on:click={closeNav}>&times;</a>
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
    </div>
</div>


<style>
    .toggle {
        background: red;
    }

    .color {
        background-color: #FF7F00;
        text-align: right;
        padding: 15px 20px;
        font-family: 'Raleway-Light', sans-serif;
        color: white;
        font-size: 15px;
        border-radius: 2px;
    }

    .sideForm {
        height: 100%;
        width: 0; /* NE PAS CHANGER LA WIDTH !!  SE CHANGE EN JS*/
        position: fixed;
        z-index: 1;
        top: 0;
        right: 0;
        background-color: #FF7F00;
        overflow-x: hidden;
        padding-top: 60px;
        transition: 0.5s;
    }

    /*à remplacer par les inputs pour le padding*/
    .sideForm h1 {
        padding: 20px;
    }

    .sideForm a {
        padding: 20px;
        text-decoration: none;
        font-size: 50px;
        color: purple;
        display: block;
        transition: 0.3s;
    }

    .sideForm a:hover {
        color: red;
    }

    .sideForm .closebtn {
        position: absolute;
        top: 0;
        right: 25px;
        font-size: 36px;
        margin-left: 50px;
    }

</style>
