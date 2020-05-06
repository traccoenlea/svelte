<script>
    import TestMenu from './TestMenu.svelte';
</script>
<TestMenu/>

<div class="wrap">

    <div class="boutons">
        <h1> POUR VOIR LE PROGRAMME </h1>
        <a class="btn" href="/img/pdf/programme.pdf"
   download="Programme LP CREAWEB">Télécharger l'image</a>
    </div>



</div>

<style>

    .fond {
        height: 100vh;
        margin: 0px;
        padding: 0px;
    }

    .wrap {

        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        display: flex;
        flex-direction: column;
        background: url(/img/programme.jpg) no-repeat center fixed;
        background-size: cover;
    }

    .boutons {

        display: flex;
        flex-direction: column;
        justify-content: center;
        padding: 50px;
        align-items: center;
        z-index: 99;

    }

    .btn {
        width: 250px;
        height: 45px;
        font-family: 'Raleway-Bold', sans-serif;
        font-size: 12px;
        text-transform: uppercase;
        letter-spacing: 1.5px;
        cursor: pointer;
        border: 1px solid white;
        background-color: transparent;
        color: white;
        margin: 50px;

    }

    .btn:hover {
        background-color: white;
        color: black;
    }


    h1 {
        color: white;
        font-family: 'Raleway-Bold', sans-serif;
        font-size: 40px;
    }

    a {
        display: flex;
        align-items: center;
        justify-content: center;
        text-decoration: none;
    }

</style>
