<div class="wrap">

    <div class="boutons">

        <h1> POUR VOIR LE PROGRAMME </h1>
        <button class="btn">Télécharger le fichier </button>

    </div>

    <div id="gradient-overlay"></div>

</div>

<style>

    @font-face {
        font-family: "Raleway-Bold";
        src: url("fonts/Raleway-Bold.ttf") format("TrueType");
    }
    
    .fond {
        
        height :100vh;
        margin :0px;
        padding:0px;
    }

    .wrap {

        height: 30vh;
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
        padding : 30px;
        align-items: center;
        z-index : 99;
    
    }

    #gradient-overlay {
        background: #000000;
        height: 30vh;
        width: 100%;
        position: absolute;
        opacity: 0.3;
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
        color : white;

    }

    .btn:hover {
        background-color: white;
        color : black;
    }

    h1 {
        color : white;
        font-family: 'Raleway-Bold', sans-serif;

    }

    .body {
        background: #E2E4E7;
        padding: 0;
        text-align: center;
        font-family: 'open sans';
        position: relative;
        margin: 0;
        height: 100%;
        -webkit-font-smoothing: antialiased;
    }

    .wrapper {
        height: 100%;
        height: 100%;
        margin: 0 auto; 
        overflow: hidden;
    }

    .main_page section .page_container {
        position: relative;
        top: 25%;
        margin: 0 auto 0;
        max-width: 950px;
        z-index: 3;
    }

    .main_page section  {
        overflow: hidden;
    }

    .main_page section.page1 {
        background:rgb(230, 217, 200);
    }

    .main_page section.page2 {
        background: #555557;
    }

    .main_page section.page2 .page_container {
        margin-top: 240px;
        overflow: hidden;
    }

    .main_page section.page3 {
      background: blue ;
    }

    .main_page section.page3 .page_container {
      overflow: hidden;
      width: 500px;
      right: -285px;
    }

    .main_page section.page3 h1 {
      text-align: left;
      padding: 0;
      margin-bottom: 0;
      font-size: 70px;
      letter-spacing: -1px;
      color: black;
    }

    .body {
     margin: 0;
      overflow: hidden;
      -webkit-transition: opacity 400ms;
      -moz-transition: opacity 400ms;
      transition: opacity 400ms;
    }

    .body, .onepage-wrapper {
      display: block;
      position: static;
      padding: 0;
      width: 100%;
      height: 100%;
    }



</style>