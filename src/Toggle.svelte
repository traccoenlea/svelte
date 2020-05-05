<svg class="icon icon-eyedropper"  on:click|preventDefault|stopPropagation={toggleActive}>
    <use xlink:href="#icon-eyedropper"></use>
</svg>

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
