<script>
    function myFunction() {
        var element = document.getElementById("myDIV");
        element.classList.toggle("mystyle");
    }

    function toggle(){
        // toggle = toggleClass("active");
        var menu = document.getElementById('menu-icon');
        menu.classList.toggle('active');
        var overlay = document.getElementById('overlay-menu');
        overlay.classList.toggle('open');
        // $(".overlay-menu").toggleClass("open");
    }
</script>

<nav>
    <div class="menu-icon" id='menu-icon' on:click={toggle}>
        <span></span>
    </div>
</nav>

<section class="container">
    <h1>Overlay Menu Concept</h1>
</section>

<section class="overlay-menu" id="overlay-menu">
    <div class="container">
        <div class="row">
            <div class="columns half">
                <h2>Menu left</h2>
                <ul>
                    <li>About Us</li>
                    <li>Our Work</li>
                    <li>Contact Us<li>
                </ul>
            </div>
            <div class="columns half">
                <h2>Menu Right</h2>
                <ul>
                    <li>More Menus</li>
                    <li>Log In</li>
                    <li>Do Something<li>
                </ul>
            </div>
        </div>
    </div>
</section>


<style>
    @import url(https://fonts.googleapis.com/css?family=Lato:300,400|Architects+Daughter);
    /* Grid System */

    * {
        box-sizing: border-box;
    }

    .container {
        max-width: 960px;
        position: relative;
        margin: 0 auto;
        padding: 0;
    }

    .container:before,
    .container:after {
        content: "";
        display: table;
    }

    .container:after {
        clear: both;
    }

    .row {}

    .row:before,
    .row:after {
        content: "";
        display: table;
    }

    .row:after {
        clear: both;
    }

    .columns {
        float: left;
        display: block;
        margin-bottom: 0;
        vertical-align: top;
        padding: 0;
    }

    .columns.half {
        width: 50%;
    }
    /* Main Styles */
    html{font-size: 16px;}

    body {
        background: #2e2e2e;
        background: url(https://ununsplash.imgix.net/photo-1429091967365-492aaa5accfe?fit=crop&fm=jpg&h=1700&q=75&w=1050) center center no-repeat;
        background-size: cover;
        font-family: 'Lato', 'Arial', sans-serif;
        font-weight: 400;
        font-size: 1rem;
        line-height: 1.4;
        letter-spacing: 2px;
        color: #fff;
        height: 100%;
        height: 100vh;
    }

    /* Text */

    h1 {
        margin: 5rem 0;
        text-align: center;
        text-shadow: 0 2px 2px rgba(200, 100, 0, 1);
        font-size: 3rem;
        letter-spacing: 5px;
        font-family: 'Architects Daughter', cursive;
    }

    h2 {
        font-size: 2.5rem;
        margin: 10px 0;
    }

    /* Nav Bar */

    nav {
        background: #9a5250;
        color: #2e2e2e;
        font-size: 0.2rem;
        position: fixed;
        width: 100%;
        left: 0;
        top: 0;
        box-shadow: 0px 2px 10px 0px rgba(0,0,0,0.5);
        z-index: 200;
    }

    .menu-icon {
        background: #007482;
        width: 50px;
        height: 50px;
        margin: 0 0 0 auto;
        position: relative;
        cursor: pointer;
        transition: background 0.5s;
    }

    .menu-icon span,
    .menu-icon span:before,
    .menu-icon span:after {
        cursor: pointer;
        border-radius: 1px;
        height: 2px;
        width: 35px;
        background: white;
        position: absolute;
        left: 15%;
        top: 50%;
        display: block;
        content: '';
        transition: all 0.5s ease-in-out;
    }

    .menu-icon span:before {
        left: 0;
        top: -10px;
    }

    .menu-icon span:after {
        left: 0;
        top: 10px;
    }

    .menu-icon.active {
        background: #304453;
    }

    .menu-icon.active span {
        background-color: transparent;
    }

    .menu-icon.active span:before,
    .menu-icon.active span:after {
        top: 0;
    }

    .menu-icon.active span:before {
        transform: rotate(135deg);
    }

    .menu-icon.active span:after {
        transform: rotate(-135deg);
    }
    /* Menu */

    .overlay-menu {
        background: rgba(48, 68, 83, 0.9);
        color: #ffffff;
        position: fixed;
        left: 0;
        top: 0;
        height: 100%;
        overflow-y: auto;
        -webkit-overflow-scrolling: touch;
        width: 100%;
        padding: 50px 0;
        opacity: 0;
        text-align: center;
        transform: translateY(-100%);
        transition: all 0.5s;
    }

    .overlay-menu.open {
        opacity: 1;
        transform: translateY(0%);
    }

    .overlay-menu .columns {
        transform: translateY(5%);
        opacity: 0;
        transition: all 0.4s;
        transition-delay: 0s;
    }

    .overlay-menu.open .columns {
        transition: all 1s;
        transition-delay: 1s;
        opacity: 1;
        transform: translateY(0%);
    }

    .overlay-menu .columns:nth-child(2) {
        transition-delay: 0s;
    }

    .overlay-menu.open .columns:nth-child(2) {
        transition-delay: 1.25s;
    }


    .overlay-menu ul {
        font-size: 1.5rem;
    }
    .overlay-menu ul li{
        padding: 1rem;
    }

    @media screen and (max-width: 600px) {
        html {font-size: 12px;}

        .columns.half {
            width: 100%;
            margin: 10px 0;
        }
    }
</style>
