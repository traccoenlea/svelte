
<script>
    import Toggle from './Toggle.svelte';

    let src = 'https://media.giphy.com/media/jOgRWnCyyRqLaCjHMS/source.gif';

</script>



<nav class="nav">
    <ul>
        <li><a href="#home">Accueil</a></li>
        <li><a href="#objectifs">Objectifs & Compétences</a></li>
        <li><a href="#debouches">Débouchés</a></li>
        <li><a href="#programme">Programme</a></li>
        <li>
            <Toggle title="Toggle Header" isActive={true}>
            <div class="content">
                <img {src} alt="test" id="imageTest"/>
            </div>
        </Toggle>
        </li>
    </ul>
</nav>

<style>
    .nav{
        padding: 20px;
    }
   a {
       text-decoration: none;
       color: black;
   }

    ul {
        display: flex;
        flex-direction: row;
        /*A MODIF SELON TES ENVIES : */
        justify-content: space-around;
    }

    li {
        list-style: none;

    }
</style>

