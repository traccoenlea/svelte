<script>
    import TestMenu from './TestMenu.svelte';

    let education = '/img/icon/education.svg';

    let src = '/img/fond.png';
    let langue = '/img/icon/langue.png';
    let location = '/img/icon/location.png';
    let cours = '/img/icon/cours.png';
    // let education = '/img/icon/education.png';
    let diplomas = '/img/icon/diplomas.png';
    let doc = '/img/icon/doc.png';


    //FORM MODIF

    function openNav() {
        document.getElementById("sideForm").style.width = "500px";
    }

    function closeNav() {
        document.getElementById("sideForm").style.width = "0";
    }

    //MODIF FORMULAIRE
    let nomFormation = 'LP CRÉAWEB: MÉTIERS DU NUMÉRIQUE: CONCEPTION, RÉDACTION ET RÉALISATION WEB';
    let lieuFormation = 'IUT DE LENS';
    let langueCours = 'FRANÇAIS';
    let modalites = 'ALTERNANCE ou CONTINU (avec stages)';
    let admissible = 'Bac +2 minimum';
    let sortie = 'Bac +3';
    let heures = '536';

    //FONT & COLOR
    let color = 'white';
    let textColor = 'black';

    let fonts = ['Times New Roman', 'Georgia', 'Arial', 'Verdana', 'Monospace', 'Courier New', 'Lucida Console'];
    var font = 'Raleway';

    function changeFont() {
        font = document.getElementById('fontChange').value;
    }

</script>

<TestMenu/>


<div class="fond">
<div class="textChange" id="fontHere" style="--font-family: {font}">
    <div class="texte" id="bgChange" style="--bg-color: {color}">
        <div class="allText" id="txtChange" style="--text-color: {textColor}">
            <div class="ligne"></div>
            <h2 id="nomFormation">{nomFormation}</h2>

            <div class="langue">
                <img src={location} alt="icone de lieu de formation">
                <p>{lieuFormation}</p>
            </div>

            <div class="langue">
                <img src={langue} alt="icone de la langue utilisée">
                <p>{langueCours}</p>
            </div>

            <div class="langue">
                <img src={education} alt="icone des modalités">
                <p>{modalites}</p>
            </div>

            <div class="langue">
                <img src={doc} alt="icone de niveau de formation nécessaire">
                <p> Admissible à : {admissible} </p>
            </div>

            <div class="langue">
                <img src={diplomas} alt="icone de niveau obtenu">
                <p> Niveau de sortie : {sortie} </p>
            </div>

            <div class="heures">
                <p> {heures} heures d'enseignements </p>
            </div>
        </div>


        <img src={education} class="imgToChange"/>
    </div>
</div>

    <div class="toggle">
        <div on:click={openNav} class="color">Modifier la page</div>
    </div>


    <div id="sideForm" class="sideForm">
        <a href="javascript:void(0)" class="closebtn" on:click={closeNav}>&times;</a>
        <div id="form">
            <label for="changeFormation">Titre de la formation :</label>
            <input type="text" id="changeFormation" bind:value={nomFormation}/>

            <div class="langue">
                <label for="changeLieu">
                    <img src={location} alt="icone de lieu de formation">
                </label>
                <input type="text" id="changeLieu" bind:value={lieuFormation}/>
            </div>

            <div class="langue">
                <label for="changeLangueCours">
                    <img src={langue} alt="icone de la langue utilisée">
                </label>
                <input type="text" id="changeLangueCours" bind:value={langueCours}/>
            </div>

            <div class="langue">
                <label for="changeModalites">
                    <img src={education} alt="icone des modalités">
                </label>
                <input type="text" id="changeModalites" bind:value={modalites}/>
            </div>

            <div class="langue">
                <label for="changeAdmissibilite">
                    <img src={doc} alt="icone de niveau de formation nécessaire">
                </label>
                <input type="text" id="changeAdmissibilite" bind:value={admissible}/>
            </div>

            <div class="langue">
                <label for="changeSortie">
                    <img src={diplomas} alt="icone de niveau obtenu">
                </label>
                <input type="text" id="changeSortie" bind:value={sortie}/>
            </div>

            <div class="heures">
                <label for="changeHeures">Nombre d'heures d'enseignements : </label>
                <input type="text" id="changeHeures" bind:value={heures}/>
            </div>

        </div>

        <hr>

        <div class="colorsToChange">

            <label for="bgColor">Changement couleur background :</label>
            <input id="bgColor" type="color" bind:value={color} style="height: 50px;">

            <br/><br/>


            <label for="textColor">Changement couleur du texte :</label>
            <input id="textColor" type="color" bind:value={textColor} style="height: 50px;">

            <br/><br/>


            <label for="fontChange">Changement de font :</label>

            <select id="fontChange">
                {#each fonts as font}
                    <option>{font}</option>
                {/each}
            </select>

            <br/>

            <button on:click={changeFont}>
                On change de police !
            </button>

        </div>
    </div>

</div>


<style>

    .imgToChange {
        color: yellow;
    }

    /*raleway to remove*/
    h2 {
        font-weight: 600;
        font-size: 20px;
        padding-bottom: 20px;
    }

    p {
        font-weight: 300;
        font-size: 15px;
        padding: 10px;
    }

    .color {
        background-color: #FF7F00;
        text-align: right;
        padding: 15px 20px;
        font-weight: 300;
        color: white;
        font-size: 15px;
        border-radius: 2px;
    }

    /*font & color*/

    #bgChange {
        background: var(--bg-color);
        padding: 30px;
    }

    #txtChange {
        font-weight: bold;
        margin: 20px;
        font-size: 20px;
        color: var(--text-color);
    }

    #fontHere {
        font-family: var(--font-family);
        font-size: 30px;
    }

    hr {
        margin-top: 10px;
        margin-bottom: 10px;
        width: 70px;
        height: 5px;
        color: purple;
        background: purple;
        outline: none;
        border: none;

    }



    .sideForm {
        height: 100%;
        width: 500px; /* NE PAS CHANGER LA WIDTH !!  SE CHANGE EN JS*/
        position: fixed;
        z-index: 1;
        top: 0;
        right: 0;
        background-color: #FF7F00;
        overflow-x: hidden;
        transition: 0.5s;
        padding: 20px;
        padding-top: 60px;

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

    .fond {
        height: 100vh;
        background: url('/img/fond.png') no-repeat center fixed;
        background-size: cover;
        height: 100vh;
        display: flex;
        justify-content: left;
        padding-left: 150px;
        align-items: center;
    }

    .langue {

        display: flex;
        justify-content: left;
        align-items: center;

    }

    .ligne_bas {

        border-bottom: 5px solid #EE8B29;
        height: 30px;
        width: 70px;
    }


    img {

        width: 15px;
        height: 15px;
    }

    .texte {

        background-color: white;
        width: 50vh;
        padding: 40px;
        display: flex;
        flex-direction: column;
    }

    .ligne {

        border-top: 5px solid #EE8B29;
        height: 30px;
        width: 70px;
    }



</style>

