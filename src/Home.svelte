<script>

	let src = '/img/fond.png';
	let langue = '/img/icon/langue.png';
	let location = '/img/icon/location.png';
	let cours = '/img/icon/cours.png';

</script>


<div class="fond">

	<div class="texte"> 

		<div class="ligne"></div>
		<h2> LP CRÉAWEB: MÉTIERS DU NUMÉRIQUE: CONCEPTION, RÉDACTION ET RÉALISATION WEB </h2> 

		<div class="langue">
			<img src={location}>
			<p> IUT DE LENS  </p> 
		</div>

		<div class="langue">
			<img src={langue}>
			<p> FRANÇAIS  </p> 
		</div>

		<div class="langue">
			<img src={location}>
			<p> ALTERNANCE  </p> 
		</div>

		<div class="langue">
			<img src={langue}>
			<p> Admissible à : Bac+2 </p>
		</div>

		<div class="langue">
			<img src={location}>
			<p> Niveau de sortie : Bac +3 </p>
		</div>

		<div class="heures">
			<p> 536 heures d'enseignement dont 134 heures de projets </p>
		</div>

	</div>

</div>

<style>
	
	.fond {
	    height :100vh;
	    background: url('/img/fond.png') no-repeat center fixed; 
	    background-size: cover;
	    height: 100vh;
	    display: flex;
    	justify-content: left;
    	padding-left: 150px;
    	align-items: center;
    }

    .langue {

    	display: flex;
    	justify-content: left;
    	align-items: center;

    }

    .ligne_bas {
	    
	    border-bottom: 5px solid #EE8B29;
	    height: 30px;
	    width: 70px;
	}


    img {

    	width: 15px;
    	height: 15px;
    }

    .texte {

    	background-color: white;
    	width: 50vh;
    	padding: 40px;
    	display: flex;
    	flex-direction: column;
    }

    .ligne {
	    
	    border-top: 5px solid #EE8B29;
	    height: 30px;
	    width: 70px;
	}

	h2 {
    	font-family: 'Raleway-SemiBold', sans-serif;
    	font-size: 17px;
    	padding-bottom: 20px;
    }

    p {
    	font-family: 'Raleway-Regular', sans-serif;
    	font-size: 15px;
    	padding: 10px;
    }

</style>

