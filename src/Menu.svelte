
<nav class="nav">

    <div class="menu">
        <ul>
            <li><a href="#home">Accueil</a></li>
            <li><a href="#objectifs">Objectifs & Compétences</a></li>
            <li><a href="#debouches">Débouchés</a></li>
            <li><a href="#programme">Programme</a></li>
        </ul>
    </div>
</nav>

<div class="toggle">
    <div on:click={openNav} class="color">Modifier la page</div>
</div>
<div id="sideForm" class="sideForm">
    <a href="javascript:void(0)" class="closebtn" on:click={closeNav}>&times;</a>
    <h1>EN GROS LE FORMULAIRE VA LA</h1>
</div>

<script>
    function openNav() {
        document.getElementById("sideForm").style.width = "500px";
    }

    function closeNav() {
        document.getElementById("sideForm").style.width = "0";
    }
</script>

<style>
    #main {
        margin-top: 100px;
    }

    .color {
        background-color: #FF7F00;
        text-align: right;
        padding-top: 15px;
        padding-bottom: 15px;
        padding-left: 20px;
        padding-right: 20px;
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

    .nav{
        padding: 20px;
        background-color: white;
        display: flex;
        width: 100%;
        position: fixed;
        box-shadow: 0 0 11px -5px #000;
        align-items: center;
        height: 40px;
    }

    .menu {
        width : 70%;
        display: flex;
        justify-content: flex-start;
        margin-left: 50px;
        align-items: center;
        position: absolute;

    }

    .toggle {
        top: 15px;
        right: 100px;
        position: relative;
        width : 100%;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    a {
        text-decoration: none;
        color: black;
        font-family: 'Raleway-Light', sans-serif;
        font-size: 15px;
        padding: 20px;
    }

    a:hover {

        color: #FF7F00;
    }


    ul {
        display: flex;
        flex-direction: row;
        justify-content: center;
    }

    li {
        list-style: none;

    }


</style>
