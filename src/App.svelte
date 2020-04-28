<script>
    import Juju from './Juju.svelte';
    import Maria from './Maria.svelte';
    import Lea from './Lea.svelte';
    import Lea_Bis from './Lea_Bis.svelte';


    let name = 'world';
</script>

<nav>
    <a href="#Juju">Juju</a>
    <a href="#Maria">Maria</a>
    <a href="#Lea">Léa</a>
    <a href="#Lea_Bis">Léa Bis</a>
</nav>

<h1>Hello {name}!</h1>

<div id="Juju">
    <Juju/>
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

