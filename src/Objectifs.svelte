<script>
    import Menu from './Menu.svelte';
</script>
<Menu/>
<div class="fond">

    <div class="groupe">
    	<div class="groupe1"> 
            <h1> OBJECTIFS & COMPÉTENCES </h1> <h1 class="orange"> DE LA FORMATION</h1> 
            <p> La Licence Professionnelle Métiers du numérique : </p>
            <p class="inter"> •  de concevoir et de réaliser des sites web aux fonctionnalités multiples </p>
            <p class="inter"> • De concevoir et de créer des contenus appropriés à chaque site et répondant à des besoins spécifiques (écrits, visuels, infographiques). </p>
        </div>

        <div class="groupe2"> 

    		<p class="titre">	  Elle leur permet également :</p>
    		<p class="inter"> • De maîtriser les connaissances et les compétences indispensables à la conception d’un projet dans le domaine du web.</p>
    		<p class="inter"> • De maîtriser les connaissances et les compétences indispensables à la conception d’un projet dans le domaine du web.</p>
    		<p class="inter"> • D’acquérir une méthodologie rigoureuse de la gestion d’un projet.</p>
    		<p class="inter"> • D’acquérir des compétences en communication orale et écrite à des fins argumentatives (présentation de projets, prise de décision, expression de choix etc.)</p>

    	</div>
    </div>
</div>


<style>
	
	.fond {
	    background: url('/img/groupe.png') no-repeat center fixed; 
	    background-size: cover;
	    height: 100vh;
	    display: flex;
        justify-content: center;
    	align-items: center;
    }

    .groupe{
        display: flex;
        height: 350px;
        justify-content: center;
    }

    .groupe1 {
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
        width: 50%;
        margin-left: 150px;
        border-right: 1px solid white;
        padding-bottom: 50px;
        padding-left: 50px;
        padding-right: 50px;
        padding-top: 10px;
    }

    .groupe2 {
        width: 50%;
        margin-right: 150px;
        padding-bottom: 50px;
        padding-left: 50px;
        padding-right: 50px;
        padding-top: 10px;
    }

    h1 {
        color : white;
        font-family: 'Raleway-Bold', sans-serif;
        font-size: 30px;
    }

    .orange {
        color: #FF7F00;
        padding-bottom: 20px;
    }

    p { 
        color : white;
        font-family: 'Raleway-Light', sans-serif;
        font-size: 15px;
        padding-top: 10px;
        line-height : 20px;
        list-style-type: disc;
    }

    .inter {

        padding-left: 40px;
    }

    .titre {

        padding-bottom: 20px;
    }

</style>
