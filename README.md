POURQUOI SVELTE ?

- nouveauté donc intéressant
- code compilé
- virtual dom
- html - css - js
- installation simple et rapide


PRÉSENTATION DU SITE

POURQUOI ?
- L’objectif c’était de pouvoir créer un site facile d'utilisation, type wordpress like pour présenter des formations
 universitaires et pouvoir le modifier à sa guise.<br/>
COMMENT ?
- En faisant une interface moderne, premièrement avec une maquette représentative du produit final, puis en utilisant
 HTML, CSS et JS.<br/>
DESIGN
-On a choisi une interface minimaliste qui pouvait nous permettre de mettre en place nos connaissances sur svelte, en
 utilisant quelques propriétés.
- On a choisi de faire un design simple mais élégant, l’idée est en trois jours pouvoir construire un site qui
 fonctionne et soit agréable à l’oeil.


RÉPARTITION DU GROUPE
- LÉA : DÉVELOPPEMENT SVELTE + GIT
- JULIETTE :  DESIGN + HTML / CSS
- MARIA : DESIGN + HTML / CSS

FONCTIONNALITÉS & MISE EN PRATIQUE<br/>
Nous avons choisi d’utiliser des composants pour certaines parties du site afin d’optimiser les pages. Pour cela
nous avons choisi de : 
- créer un composant par page du slider (Home, Objectifs, Débouchés et Programme)
- créer un composant Menu implémenté sur chaque page (ci-dessus)

Durant la phase de développement, nous avons créé de nombreux composants afin de tester différentes fonctionnalités, ce qui nous évitait de créer des conflits en travaillant sur les mêmes fichiers.

Comme dit précédemment, Svelte regroupe HTML, CSS et Javascript. Nous avons donc implémenté quelques aspects du site en Svelte.
- les images ont des sources définies en variable
- les svg viennent d’une dépendance Svelte en collaboration avec fontAwesome
- les fonctions activées au clic sont implémentées en Svelte 
- les fonctionnalités de personnalisation comprennent la modification de texte en instantané par Svelte ainsi que les
 changements de couleurs et police de façon immédiate

DIFFICULTÉS RENCONTRÉES
- MANQUE D’INFORMATIONS<br/>
petite communauté donc difficile de trouver toutes les réponses
- DIFFICULTÉS EN JS<br/>
il faut avoir de bonnes bases en JS pour comprendre Svelte 
- FONCTIONNEMENT<br/>
manque de temps pour l’utiliser à son potentiel maximum


Ressentis personnels : 

Juliette :<br/>
J’ai bien aimé utiliser svelte, je l’ai trouvé, comme Maria, simple d’utilisation. Ce que j’ai adoré le plus c’est le fait que les erreurs s’affichent dans le terminal, par exemple pour un point virgule. 


Maria :<br/>
Svelte est un framework de “facile utilisation”, avec une très bonne optimisation et rapidité au moment de développer une application web ou mobile, la précompilation de code le rend plus  attractif notamment grâce au fait que l'on peut voir presque en temps réel les changements. 
La division du code ouverte aide à le faire plus efficace et permet d’ajouter des fonctions de manière gratuite, c’est qui est super!. Bref, je l’ai trouvé très attirant et moins lourd en comparaison des autres frameworks.

Léa :<br/>
J’ai aimé appréhender Svelte, malheureusement, n’ayant pas beaucoup de temps pour apprendre en profondeur la technologie avant de devoir créer un site, j’ai dû me contenter des quelques premiers chapitres des tutoriels proposés par Svelte.
N’étant pas une grande fan de Javascript, ni même très douée dans ce langage de programmation, je me suis surprise à persévérer pour essayer de trouver des solutions aux problèmes rencontrés. 

BILAN <br/>
- c’est compliqué d’apprendre une techno par soi-même
- nous sommes fières car nous avons réussi à produire un site complet (design et fonctionnel)
- doc qu’en anglais


6. RÉFÉRENCES 

https://madewithsvelte.com/svelte-awesome
https://github.com/RobBrazier/svelte-awesome#more-advanced-cases
https://robbrazier.github.io/svelte-awesome/
https://github.com/FortAwesome/Font-Awesome
https://www.npmjs.com/package/@fortawesome/free-regular-svg-icons


<br/><br/>


// POUR RÉCUPÉRER LE PROJET :

```bash
git pull
cd svelte-app
npm install
```
npm install : installer les dépendances nécessaires

```bash
npm run dev
```
pour lancer le projet qui est accessible à cette adresse : http://localhost:5000
