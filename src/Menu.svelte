<script>
    import Toggle from './Toggle.svelte';

    let src = 'https://media.giphy.com/media/jOgRWnCyyRqLaCjHMS/source.gif';

</script>


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
        <li class="liTo">
            <Toggle title="Toggle Header" isActive={true}>
                <div class="content">
                    <img {src} alt="test" id="imageTest"/>
                </div>
            </Toggle>
        </li>
    </div>



<style>
    .liTo {
         background-color: #FF7F00;
    }

    .content {
       width: 100%;

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


