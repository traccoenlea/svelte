<h1>page de Léa</h1>


<ul>
    <li>formulaire</li>
    <li>input pour les titres</li>
    <li>Mettre genre si c bleu alors le texte devient blanc ? functions</li>
    <li>Police : Liste de polices</li>
    <li>Ajouter des conseils : si + que 2 polices choisies alors "stop" idem avec les couleurs</li>
</ul>


<script>
    let color = 'purple';
    let textColor = 'blue';

    let fonts = ['Times New Roman', 'Georgia', 'Arial', 'Verdana', 'Monospace', 'Courier New', 'Lucida Console'];
    var font = 'Impact';

    function changeFont() {
        font = document.getElementById('fontChange').value;
    }

</script>


<div id="bgChange" style="--bg-color: {color}">là c'est le background qu'on change</div>
<div id="txtChange" style="--text-color: {textColor}">là c'est le texte qu'on veut changer !</div>


<label for="bgColor">Changement couleur bg :</label>
<input id="bgColor" type="color" bind:value={color} style="height: 50px;">


<label for="textColor">Changement couleur text :</label>
<input id="textColor" type="color" bind:value={textColor} style="height: 50px;">


<label for="fontChange">Changement de font :</label>

<select id="fontChange">
    {#each fonts as font}
        <option>{font}</option>
    {/each}
</select>

<button on:click={changeFont}>
    On change de police !
</button>


<div id="fontHere" style="--font-family: {font}">
    Là on change de font pour cette div !
</div>


<style>
    #bgChange {
        background: var(--bg-color);
        padding: 30px;
    }

    #txtChange {
        text-transform: uppercase;
        font-weight: bold;
        margin: 20px;
        font-size: 20px;
        color: var(--text-color);
    }

    #fontHere {
        font-family: var(--font-family);
        font-size: 30px;
    }
</style>
