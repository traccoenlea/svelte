<!--<svg class="icon icon-eyedropper"  on:click|preventDefault|stopPropagation={toggleActive}>-->
<!--    <use xlink:href="#icon-eyedropper"></use>-->
<!--</svg>-->

<!--<button on:click|preventDefault|stopPropagation={toggleActive}>Click here mate !</button>-->

<div class="color" on:click|preventDefault|stopPropagation={toggleActive}>Modifier</div>

<!--<nav>-->
<!--	1-->
<!--	<li on:click|preventDefault|stopPropagation={toggleActive}>Test</li>-->
<!--</nav>-->

	

{#if !isActive}
	<slot></slot>

{/if}

<script>
    export let title;
    export let isActive;

    function toggleActive() {
        isActive = !isActive
    }
</script>


<style>
    .color {
        background-color: #FF7F00;
        text-align: right;
        padding-top: 15px;
        padding-bottom: 15px;
        padding-left: 20px;
        padding-right: 20px;
        font-family: 'Raleway-Light', sans-serif;
        color: white;
        font-size: 15px;
        border-radius: 2px;
    }

    .icon {
        display: inline-block;
        width: 1.5em;
        height: 1.5em;
        /*EPAISSEUR DU TRAIT*/
        stroke-width: 2px;
        /*COULEUR DU TRAIT*/
        stroke: orange;
        /*COULEUR DE REMPLISSAGE*/
        fill: purple;
    }
</style>
