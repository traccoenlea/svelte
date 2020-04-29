<script>
    // let color = 'black';
    let text = 'black';

    let color = '#122627';

    $: rgb = parseInt(color.slice(1), 16);

    $: r = (rgb & 0xff0000) >> 16;
    $: g = (rgb & 0x00ff00) >> 8;
    $: b = (rgb & 0x0000ff) >> 0;

    function changeColor() {
        let red = r;
        let green = g;
        let blue = b;

        if (red <= 50 || green <= 50 || blue <= 50) {
            document.getElementById('bgChange').style.color = 'white';
        }else if(red >= 200 || green >=200 || blue >= 200){
            document.getElementById('bgChange').style.color = 'black';
        }else if(90 <=red>= 170 || 90 <=green>= 170 || 90 <=blue>= 170){
            alert('entre 2');
        }

    }
</script>

<br/><br/><br/>
<label for="bgColor">Changement couleur bg :</label>
<br/>
<input id="bgColor" type="color" bind:value={color} style="height: 50px;">

<h2>{color}</h2>
r:{r} g:{g} b:{b}

<button on:click={changeColor}>Choisir cette couleur pour mon background</button>

<br/><br/><br/>

<!--<label for="textColor">Changement couleur text :</label>-->
<!--<br/>-->
<!--<input id="textColor" type="color" bind:value={textColor} style="height: 50px;">-->


<div id="bgChange" style="--bg-color: {color}">
    <ul>
        <li>formulaire</li>
        <li>input pour les titres</li>
        <li>Mettre genre si c bleu alors le texte devient blanc ? functions</li>
        <li>Police : Liste de polices</li>
        <li>Ajouter des conseils : si + que 2 polices choisies alors "stop" idem avec les couleurs</li>
    </ul>
</div>


<style>
    body {
        color: yellow;
    }

    #bgChange {
        background: var(--bg-color);
        padding: 30px;
        text-transform: uppercase;
        font-weight: bold;
        margin: 20px;
        font-size: 20px;

        /*color: var(--text-color);*/
    }
</style>
