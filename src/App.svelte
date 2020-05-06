<script>
    import Home from './Home.svelte';
    import Objectifs from './Objectifs.svelte';
    import Debouches from './Debouches.svelte';
    import Programme from './Programme.svelte';

</script>


<div class="pages">
    <section id="home" class="first page">
        <Home/>
    </section>
    <section id="objectifs" class="second page">
        <Objectifs/>
    </section>
    <section id="debouches" class="third page">
        <Debouches/>
    </section>
    <section id="programme" class="fourth page">
        <Programme/>
    </section>
</div>
<ul class="pagination">
</ul>
