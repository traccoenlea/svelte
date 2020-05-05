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

    <div class="toggle"> 
        <li>
            <Toggle title="Toggle Header" isActive={true}>
                <div class="content">
                    <img {src} alt="test" id="imageTest"/>
                </div>
            </Toggle>
        </li>
    </div>
   
</nav>

<style>

    .nav{
        padding: 20px;
        background-color: white;
        display: flex;
        width: 100%;
        position: fixed;
        box-shadow: 0px 0px 11px -5px #000;
    }

    .menu {

        width : 70%;
        justify-content: flex-start;
        display: flex;
        justify-content: flex-start;
        margin-left: 50px;
        align-items: center;
    }

    .toggle {

        width : 30%;
        display: flex;
        justify-content: flex-end;
        margin-right: 100px;
        align-items: center;
    }


    a {
       text-decoration: none;
       color: black;
       font-family: 'Raleway-Light', sans-serif;
        font-size: 15px;
        padding: 15px;
    }

    a:hover{
    
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


