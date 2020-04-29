<script>
    import Home from './Home.svelte';
    import Objectifs from './Objectifs.svelte';
    import Debouches from './Debouches.svelte';
    import Programme from './Programme.svelte';
    import Perso from './Perso.svelte';
    import Menu from './Menu.svelte';

    import Juju from './Juju.svelte';
    import Lea from './Lea.svelte';
    import Lea_Bis from './Lea_Bis.svelte';
    import Color from './Color.svelte';


</script>

    <div class="pages">
        <section class="seventh page">
            <Menu/>
        </section>
        <section class="first page">
            <Home/>
        </section>
        <section class="second page">
            <Objectifs/>
        </section>
        <section class="third page">
            <Debouches/>
        </section>
        <section class="fourth page">
            <Programme/>
        </section>
        <section class="fifth page">
            <Perso/>
        </section>
        <section class="sixth page">
<!--            <Menu/>-->
        </section>
    </div>
    <ul class="pagination">
    </ul>

<!--
<nav>
    <a href="#Juju" class="item" >Juju</a>
    <a href="#Juju_Accueil" class="item" >Juju Accueil</a>
    <a href="#Maria" class="item" >Maria</a>
    <a href="#Lea"class="item" >Léa</a>
    <a href="#Lea_Bis"class="item" >Léa Bis</a>
    <a href="#Color"class="item" >Color</a>
    <span class="nav-indicator"></span>
</nav>
-->

<!--
<div id="Juju">
    <Juju/>
</div>

<div id="Juju_Accueil">
    <Juju_Accueil/>
</div>

<div id="Maria">
    <Maria/>
</div>

<div id="Lea">
    <Lea/>
</div>

<div id="Lea_Bis">
    <Lea_Bis/>
</div>




<div id="Color">
    <Color/>
</div>



nav {
  display: inline-flex;
  position: relative;
  overflow: hidden;
  max-width: 100%;
  background-color: #fff;
  padding-left: 900px;
 
}

.item {
 	 color: #83818c;
	 padding: 20px;
	 text-decoration: none;
	 transition: 0.3s;
	 margin: 0 6px;
	 z-index: 1;
	 font-family: 'DM Sans', sans-serif;
	 font-weight: 500;
	 position: relative;
 } 

  .item:before {
	 content: "";
	 position: absolute;
	 bottom: -6px;
	 left: 0;
	 width: 100%;
	 height: 5px;
	 background-color: #dfe2ea;
	 border-radius: 8px 8px 0 0;
	 opacity: 0;
	 transition: 0.3s;
}
 .item:not(.navi):hover:before {
	 opacity: 1;
	 bottom: 0;
}
 .item:not(.navi):hover {
	 color: orange;
}
 

.nav-indicator {
  position: absolute;
  left: 0;
  bottom: 0;
  height: 4px;
  transition: .4s;
  z-index: 1;
  border-radius: 8px 8px 0 0;
  
}
 @media (max-width: 580px) {
	 nav {
		 overflow: auto;
	}
}

-->






