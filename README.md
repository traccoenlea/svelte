POURQUOI SVELTE ?

nouveauté donc intéressant
code compilé
virtual dom
html - css - js
installation simple et rapide


PRÉSENTATION DU SITE

POURQUOI ?
L’objectif c’était de pouvoir créer un site facile d'utilisation, type wordpress like pour présenter des formations universitaires et pouvoir le modifier à sa guise.
COMMENT ?
En faisant une interface moderne, premièrement avec une maquette représentative du produit final, puis en utilisant HTML, CSS et JS.
DESIGN
On a choisi une interface minimaliste qui pouvait nous permettre de mettre en place nos connaissances sur svelte, en utilisant quelques propriétés.
On a choisi de faire un design simple mais élégant, l’idée est en trois jours pouvoir construire un site qui fonctionne et soit agréable à l’oeil.


RÉPARTITION DU GROUPE

•  LÉA : DÉVELOPPEMENT SVELTE + GIT
•  JULIETTE :  DESIGN + HTML / CSS
•  MARIA : DESIGN + HTML / CSS

FONCTIONNALITÉS & MISE EN PRATIQUE
Nous avons choisi d’utiliser des composants pour certaines parties du site afin d’optimiser les pages. Pour cela nous avons choisi de : 
créer un composant par page du slider (Home, Objectifs, Débouchés et Programme)
créer un composant Menu implémenté sur chaque page (ci-dessus)

Durant la phase de développement, nous avons créé de nombreux composants afin de tester différentes fonctionnalités, ce qui nous évitait de créer des conflits en travaillant sur les mêmes fichiers.

Comme dit précédemment, Svelte regroupe HTML, CSS et Javascript. Nous avons donc implémenté quelques aspects du site en Svelte.
les images ont des sources définies en variable
les svg viennent d’une dépendance Svelte en collaboration avec fontAwesome
les fonctions activées au clic sont implémentées en Svelte 
les fonctionnalités de personnalisation comprennent la modification de texte en instantané par Svelte ainsi que les changements de couleurs et police de façon immédiate

DIFFICULTÉS RENCONTRÉES
•  MANQUE D’INFORMATIONS
petite communauté donc difficile de trouver toutes les réponses
•  DIFFICULTÉS EN JS
il faut avoir de bonnes bases en JS pour comprendre Svelte
•  FONCTIONNEMENT
manque de temps pour l’utiliser à son potentiel maximum


Ressentis personnels : 

Juliette :
J’ai bien aimé utiliser svelte, je l’ai trouvé, comme Maria, simple d’utilisation. Ce que j’ai adoré le plus c’est le fait que les erreurs s’affichent dans le terminal, par exemple pour un point virgule. 


Maria :
Svelte est un framework de “facile utilisation”, avec une très bonne optimisation et rapidité au moment de développer une application web ou mobile, la précompilation de code le rend plus  attractif notamment grâce au fait que l'on peut voir presque en temps réel les changements. 
La division du code ouverte aide à le faire plus efficace et permet d’ajouter des fonctions de manière gratuite, c’est qui est super!. Bref, je l’ai trouvé très attirant et moins lourd en comparaison des autres frameworks.

Léa :
J’ai aimé appréhender Svelte, malheureusement, n’ayant pas beaucoup de temps pour apprendre en profondeur la technologie avant de devoir créer un site, j’ai dû me contenter des quelques premiers chapitres des tutoriels proposés par Svelte.
N’étant pas une grande fan de Javascript, ni même très douée dans ce langage de programmation, je me suis surprise à persévérer pour essayer de trouver des solutions aux problèmes rencontrés. 

BILAN 
c’est compliqué d’apprendre une techno par soi-même
nous sommes fières car nous avons réussi à produire un site complet (design et fonctionnel)
doc qu’en anglais





INTRODUCTION 

code compilé : c'est à dire que le code il est optimisé pour être le plus léger possible.  Par exemple ça nous permet de voir les erreurs dans le terminal. 

Virtual DOM :  Chaque fois que l'état de notre application change, le virtual DOM est mis à jour naturellement. 

Installation rapide et efficace, et c’est variable selon tout les niveau. Par exemple un débutant peut installer un projet svelte  sans problème, sans difficulté notamment grâce à la doc qui sont sur leur site. 

(présentation Svelte = pourquoi on a choisi Svelte -> qu’est-ce qui nous a attiré dans Svelte ?)


nouveauté 
code compilé
virtual DOM
html, css, js
Installation rapide et efficace

Svelte c’est un nouveau framework .js de code précompilé, qui permet d’écrire moins du code et d’avoir du HTML, CSS et JavaScript dans une seule feuille. Pendant le processus de développement, la compilation se fait dans de petits modules indépendants JS. Résultant en une application plus rapide et plus simple. (n'utilise pas virtual DOM).
On a choisi cette nouvelle technologie car elle plus vive au niveau du chargement et n’a pas besoin de dépendances pour s’initialiser, c’est qui le rend idéal pour les concepteurs web.
Beaucoup de façons d’installer, selon le niveau de l’utilisateur
Nous avons choisi de faire :

npx degit sveltejs/template my-svelte-project
cd my-svelte-project
npm install
npm run dev

2. PRÉSENTATION DU SITE 

Pour présenter svelte, on a décidé de faire une version one page plus attirante de l’offre académique des formations de L’IUT DE LENS,  au niveau développement et design web. Avec une interface amicale, plus moderne et minimaliste, avec l'amélioration de l'accessibilité du site, en permettant à l'utilisateur changer quelques caractéristiques de la page: la couleur, le format et la taille de police, et des information pertinent de filière proposé.

Pourquoi ? Le Besoin
Le besoin c’est de pouvoir faire un site facile, wordpress like pour présenter des formations universitaires. 


Comment ? 
En faisant une interface moderne, premièrement avec une maquette représentative du produit final, puis en utilisant JS, HTML et CSS.


Design
On a choisi une interface un peu minimaliste qui peut nous permettre de mettre en place nos connaissances sur svelte, en utilisant un peu de ses propriétés.
Nouveau design on a voulu partir sur quelques de simplet mais élégant, l’idée est en trois jours pouvoir construire un site qui fonctionne et soit agréable à l’oeil

Répartition du groupe ? 

Léa : Développement svelte
Juju : Design + HTML CSS
María: Design + HTML CSS


Fonctionnalités

3. MISE EN PRATIQUE SVELTE

Choix par rapport aux composants
Nous avons choisi d’utiliser des composants pour certaines parties du site afin d’optimiser les pages. Pour cela nous avons choisi de : 
créer un composant par page du slider (Home, Objectifs, Débouchés et Programme)
créer un composant Menu implémenté sur chaque page (ci-dessus)

Durant la phase de développement, nous avons créé de nombreux composants afin de tester différentes fonctionnalités, ce qui nous évitait de créer des conflits en travaillant sur les mêmes fichiers.

Ce qui est en Svelte dans le site : images etc
Comme dit précédemment, Svelte regroupe HTML, CSS et Javascript. Nous avons donc implémenté quelques aspects du site en Svelte.
les images ont des sources définies en variable
les svg viennent d’une dépendance Svelte en collaboration avec fontAwesome
les fonctions activées au clic sont implémentées en Svelte 
les fonctionnalités de personnalisation comprennent la modification de texte en instantané par Svelte ainsi que les changements de couleurs et police de façon immédiate





4. DIFFICULTÉS RENCONTRÉES

manque d’information sur comment faire des choses qu’ils ne sont pas expliqué  : de plus c’est en anglais 
pas de grosses connaissances de JS au préalable très compliqué de comprendre svelte 
comprendre le fonctionnement

Il n’a pas assez d'information à propos de l’utilisation de svelte, il y a que le bases. même si sur le site existe le tutorial, c’est aussi un peu compliqué.

On ne maitrisez pas beaucoup JS, et ca le rendre difficile, car  d’abord svelte utilise JS pure pour faire son processus de précompilation, et en conséquence peut le rendre lente dans son processus d'apprentissage.

Même si c’est facile à apprendre, il faut comprendre chacun de ses composantes et fonctionnalités. Svelte, comme des autres framework, il faut le dédier du temps pour le bien maîtriser, et il a fallu plus de temps pour l’apprendre complètement, en parlant des toutes fonctionnalités et aussi pour faire un appli plus puissante.



5. RESSENTI PERSONNEL PAR RAPPORT À SVELTE 

Juju ; j’ai bien aimé utiliser svelte, j’ai trouvé comme Maria simple d’utilisation. le plus que j’ai adoré c’est le fait que les erreurs s’affichent dans le terminal, pour un pint virgule. 


Maria._
Svelte, c’est un framework de “facile utilisation”, avec une très bonne optimisation et rapidité au moment de développer une application web ou mobile, la précompilation de code rendre plus  attractive le fait, qu’on peut voir presque en temps réel les changements. 
La division du code ouverte aide à le faire plus efficace et permet d’ajouter des fonctions de manière gratuite, c’est qui est super!. Bref, j’ai le trouve très attirante et moins lourde en comparaison des autres frameworks.

Léa
J’ai aimé appréhender Svelte, malheureusement, n’ayant pas beaucoup de temps pour apprendre en profondeur la technologie avant de devoir créer un site, j’ai dû me contenter des quelques premiers chapitres des tutoriels proposés par Svelte.
N’étant pas une grande fan de Javascript, ni même très douée dans ce langage de programmation, je me suis surprise à persévérer pour essayer de trouver des solutions. 


Bilan : 

c’est compliqué d’apprendre une techno par soi-même
fières = produire un site complet (design et fonctionnalités)
doc en anglais


6. RÉFÉRENCES 

https://madewithsvelte.com/svelte-awesome
https://github.com/RobBrazier/svelte-awesome#more-advanced-cases
https://robbrazier.github.io/svelte-awesome/
https://github.com/FortAwesome/Font-Awesome
https://www.npmjs.com/package/@fortawesome/free-regular-svg-icons





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
