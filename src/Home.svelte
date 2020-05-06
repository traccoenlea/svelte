<script>
    import Menu from './Menu.svelte';

    import Icon from 'svelte-awesome';
    import {
        mapMarker,
        globe,
        briefcase,
        checkSquareO,
        trophy
    } from 'svelte-awesome/icons';

    let src = '/img/fond.png';
    let doc = '/img/icon/doc.png';

    //FORM MODIF
    function openNav() {
        document.getElementById("sideForm").style.width = "30%";
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
    let fillColor = 'black';
    let divColor = '#FF7F00';

    let fonts = ['Times New Roman', 'Georgia', 'Arial', 'Verdana', 'Monospace', 'Courier New', 'Lucida Console'];
    var font = 'Raleway';

    function changeFont() {
        font = document.getElementById('fontChange').value;
    }
</script>

<Menu/>

<div class="fond">
    <div class="textChange" id="fontHere" style="--font-family: {font}">
        <div class="texte" id="bgChange" style="--bg-color: {color}">
            <div class="allText" id="txtChange" style="--text-color: {textColor}">
                <div class="ligne" id="ligne" style="--div-color: {divColor}"></div>
                <h2 id="nomFormation">{nomFormation}</h2>

                <div class="langue">
                    <div class="icons">
                        <Icon data={mapMarker} id="iconChange" style="fill : {fillColor}" scale="1.3"/>
                    </div>
                    <p class="uppercase">{lieuFormation}</p>
                </div>

                <div class="langue">
                    <div class="icons">
                        <Icon data={globe} id="iconChange" style="fill : {fillColor}" scale="1.3"/>
                    </div>
                    <p class="uppercase">{langueCours}</p>
                </div>

                <div class="langue">
                    <div class="icons">
                        <Icon data={briefcase} id="iconChange" style="fill : {fillColor}" scale="1.1"/>
                    </div>
                    <p class="uppercase">{modalites}</p>
                </div>

                <div class="langue">
                    <div class="icons">
                        <Icon data={checkSquareO} id="iconChange" style="fill : {fillColor}" scale="1.1"/>
                    </div>
                    <p> Admissible à : {admissible} </p>
                </div>

                <div class="langue">
                    <div class="icons">
                        <Icon data={trophy} id="iconChange" style="fill : {fillColor}" scale="1.2"/>
                    </div>
                    <p> Niveau de sortie : {sortie} </p>
                </div>

                <div class="heures">
                    <p> {heures} heures d'enseignements </p>
                </div>
            </div>
        </div>

        <div class="toggle">
            <div on:click={openNav} class="color">Modifier la page</div>
        </div>
    </div>


    <div id="sideForm" class="sideForm">
        <a href="javascript:void(0)" class="closebtn" on:click={closeNav}>&times;</a>
        <div id="form">
            <input class="nom" type="text" id="changeFormation" bind:value={nomFormation}/>

            <div class="langue">
                <input class="nom" type="text" id="changeLieu" bind:value={lieuFormation}/>
            </div>

            <div class="langue">
                <input class="nom" type="text" id="changeLangueCours" bind:value={langueCours}/>
            </div>

            <div class="langue">
                <input class="nom" type="text" id="changeModalites" bind:value={modalites}/>
            </div>

            <div class="langue">
                <input class="nom" type="text" id="changeAdmissibilite" bind:value={admissible}/>
            </div>

            <div class="langue">
                <input class="nom" type="text" id="changeSortie" bind:value={sortie}/>
            </div>

            <div class="heures">
                <input class="nom" type="number" id="changeHeures" bind:value={heures}/>
            </div>
        </div>

        <div class="colorsToChange">
            <div class="si">
                <div class="lolo">
                    <label class="what" for="bgColor">Fond :</label>
                    <input class="coloriage" id="bgColor" type="color" bind:value={color} style="height: 50px;">
                </div>

                <div class="lolo">
                    <label class="what" for="textColor">Texte :</label>
                    <input class="coloriage" id="textColor" type="color" bind:value={textColor} style="height: 50px;">
                </div>

                <div class="lolo">
                    <label class="what" for="fillColor">Icônes :</label>
                    <input class="coloriage" id="fillColor" type="color" bind:value={fillColor} style="height: 50px;">
                </div>

                <div class="lolo">
                    <label class="what" for="divColor">Trait :</label>
                    <input class="coloriage" id="divColor" type="color" bind:value={divColor} style="height: 50px;">
                </div>
            </div>

            <div class="lulu">
                <select class="ok" id="fontChange">
                    {#each fonts as font}
                        <option>{font}</option>
                    {/each}
                </select>

                <button class="ok2" on:click={changeFont}>
                    Je choisis cette police.
                </button>
            </div>
        </div>
    </div>
</div>


<style>

    .uppercase {
        text-transform: uppercase;
    }

    .icons {
        width: 25px;
        display: flex;
        justify-content: center;
    }

    .ok {
        outline: none;
        border: none;
        background-color: rgba(255, 255, 255, 0.10);
        text-align: right;
        padding: 20px;
        font-weight: 300;
        color: white;
        font-size: 12px;
        border-radius: 6px;
        font-family: 'Raleway-Light', sans-serif;
        cursor: pointer;
        width: 35%;
        margin-right: 20px;
    }

    .ok2 {
        outline: none;
        border: none;
        background-color: rgba(255, 255, 255, 0.10);
        color: white;
        font-size: 12px;
        border-radius: 6px;
        text-align: center;
        font-family: 'Raleway-Light', sans-serif;
        cursor: pointer;
        padding: 10px;
        width: 150px;
    }

    .lulu {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 85%;
        margin-top: 35px;
    }

    .si {
        display: flex;
        align-items: center;
        width: 85%;
        justify-content: center;
    }

    .what {
        font-size: 12px;
        font-family: 'Raleway-Bold', sans-serif;
        color: rgba(255, 255, 255, 0.50);
        text-transform: uppercase;
        margin-left: 12px;
        margin-top: 12px;
    }

    .nom {
        display: flex;
        width: 330px;
        border: none;
        background-color: rgba(255, 255, 255, 0.10);
        font-family: 'Raleway-Bold', sans-serif;
        color: white;
        padding-right: 25px;
        padding-left: 25px;
        padding-top: 15px;
        padding-bottom: 15px;
        border-radius: 6px;
        font-size: 14px;
        margin: 10px 0px;
        outline: none;
        height: 15px;
    }

    #iconChange {
        fill: var(--fill-color);
        background: red;
    }

    #ligne {
        border-top: 5px solid var(--div-color);
    }

    h2 {
        text-transform: uppercase;
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
        padding: 15px 20px;
        font-weight: 300;
        color: white;
        font-size: 15px;
        text-align: center;
        font-family: 'Raleway-Light', sans-serif;
        cursor: pointer;
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

    .sideForm {
        width: 0; /* NE PAS CHANGER LA WIDTH !!  SE CHANGE EN JS*/
        height: 100vh;
        position: fixed;
        z-index: 1;
        top: 0;
        right: -40px;
        background-color: rgba(1, 1, 1, 0.80);
        overflow-x: hidden;
        transition: 0.5s;
        padding: 20px;
        padding-top: 60px;
        box-shadow: 15px 45px 45px black;
    }

    /* CROIX */

    .sideForm a {
        padding: 20px;
        text-decoration: none;
        font-size: 50px;
        color: white;
        display: block;
        transition: 0.3s;
    }

    .sideForm a:hover {
        color: white;
    }


    .sideForm .closebtn {
        position: absolute;
        top: 0;
        right: 25px;
        font-size: 40px;
        margin-left: 50px;
    }

    /* Rectangle gauche */

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
        margin-top: 60px;
    }

    .ligne {
        height: 30px;
        width: 70px;
    }


    .colorsToChange {
        display: flex;
        flex-wrap: wrap;
        height: 150px;
        width: 100%;
        padding-top: 10px;
        padding-bottom: 10px;
    }


    .coloriage {
        border: none;
        display: flex;
        flex-direction: wrap;
        width: 45px;
        border: none;
        border-radius: 6px;
        outline: none;
        background-color: rgba(255, 255, 255, 0.10);
        height: 10px;
        padding: 10px;
    }

    .lolo {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

</style>
