<script>
    import Juju from './Juju.svelte';
    import Maria from './Maria.svelte'
    import Lea from './Lea.svelte'


    let name = 'world';
</script>

<nav>
    <a href="#Juju">Juju</a>
    <a href="#Maria">Maria</a>
    <a href="#Lea">Léa</a>
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
