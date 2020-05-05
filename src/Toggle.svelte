<button on:click|preventDefault|stopPropagation={toggleActive}>Appuie ici pour trigger</button>


<nav>
	1 
	<li on:click|preventDefault|stopPropagation={toggleActive}>Test</li>
</nav>

	

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
