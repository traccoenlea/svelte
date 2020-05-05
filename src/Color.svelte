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

        let color = 0;

        let total = 0;

        // if (red <= 50 && green <= 50 && blue <= 50) {
        //     document.getElementById('bgChange').style.color = 'white';
        //     color = 1;
        // }else if(red >= 200 && green >=200 && blue >= 200){
        //     document.getElementById('bgChange').style.color = 'black';
        //     color = 1;
        // }

        if(color === 0){
            for(let i = 1; i<=3; i++){
                if(i === 1){
                    total += red;
                }else if(i === 2){
                    total += green;
                }else if(i=== 3){
                    total += blue;
                }
            }
            if(total < 200){
                document.getElementById('bgChange').style.color = 'white';
            }else{
                document.getElementById('bgChange').style.color = 'black';
            }
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
