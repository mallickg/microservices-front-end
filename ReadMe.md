# MicroServices Frond-End - Pilot Project

## Liste des tâches à effectuer

- [ ] Receuil d'experience (BLSNet/Application Monolithique)
- [ ] Quelles alternatives au monolithique ?
- [ ] IFrames - Comment ca fonctionne ?
- [ ] IFrames - Avantages / Inconvénients 
- [ ] Web Components - Comment ca fonctionne ?
- [ ] Web Components - Avantages / Inconvénients
- [ ] Framework intégrés - Comment ca fonctionne ?
- [ ] Framework intégrés - Avantages / Inconvénients
- [ ] Créer un composant gérant le login de l'application 
principale
- [ ] Créer un composant gérant le changement de langue
- [ ] Créer un composant "Menu"
- [ ] Créer un composant "feature 1"
- [ ] Créer un composant "feature 2"
- [ ] Créer un composant "feature 3"
- [ ] Faire communiquer 2 composants 
- [ ] Gestion du routage
- [ ] Gestion des dépendances externes partagés
- [ ] Ansible - IT Automation

## Receuil d'experience (BLSNet/Application Monolithique)

- Base de code énorme
- Instabilité de l'application plus fréquente pour le 
developpeur (Les causes pouvant engendrer une instabilité étant
plus nombreuses)
- Temps de démarrage plus long
- Packaging de l'application plus long
- Des conflits difficiles à gérer entre les dependances 
externes de plus en plus nombreuses
- Augmentation de la dette technique permanente (Des technologies 
devenues obsolètes avec les temps)
- Migration vers des technogies plus modernes devenue couteuses
à cause de la taille de la base de code.
- Evolution de l'application difficile car chaque developpement peut
engendrer des effets de bords difficile à anticiper. (Cout de devs
et de tests plus élevés).
- Un nouveau developpeur mettra beaucoup plus de temps à maitriser
l'application à cause de la taille de la base de code et des
techniologies devenues veillissantes avec le temps.
- La defaillance d'une fonctionnalité peut engendrer 
l'indisponibilité ou l'instabilité de l'application entière.

## Quelles alternatives au monolithique ?

L'idée est de remplacer le front end d'une application web
devenue trop grosse. Pour ce faire, nous pourrions 
imaginer diviser cette application en plusieurs petites 
modules. De donner chaque module à des developpeurs différents 
ou à des équipes de developpement différentes pour ensuite les 
agréger sur un même front end. Chaque developpeur ou équipe
pourrais avoir le choix de la technologie à utiliser et 
serait responsable du developpement, de l'evolution et de la
maintenance de son/ses module(s).

### Quelles options pour le developpeur ?

#### Les frameworks

Les frameworks nous imposent un cadre et nous poussent à
réfléchir et développer comme l'auteur du Framework.
Ils necessitent également d'investir sur la formation à
chaque sortie d'un nouveau framework.
Le pattern suivant résume bien l'histoire qu'il peut y avoir
entre un developpeur et un framework :

##### Rinse, Wash, Repeat (…Forever…)

- “Cool” Framework comes out
- Learn “Cool” Framework
- Create “Cool” web app
- Next year…
- “COOLER” Framework comes out
- Abandon “Cool Legacy” web app
- Learn “COOLER” Framework
- Build new and improved “COOLER” web app
- Rinse, Wash, Repeat... 

Malgré tout, le fait d'avoir un cadre peut être rassurant pour un developpeur.
Il impose généralement l'utisation de bonnes pratiques et 
l'assurance d'une evolution constante (jusqu'au prochain
nouveau framework).
Chacun des frameworks dispose aussi d'une communauté de 
développeur plus au mois grande qui permet le partage de 
connaissances.

##### Historique des Frameworks JavaScript (liste non-exhaustive) :

![alt text](https://cdn-images-1.medium.com/max/800/1*V3Dyq3LSEElX4u3EQTUBrQ.png)


#### Les Web Components

Les Web Components sont un nouveau standard du W3C (Consortium international travaillant
à l'élaboration de nouveaux standard du developpement
WEB). Ils sont aujourd'hui supporté de façon native par Google Chrome
et via des polyfills pour les autres navigateurs.
Il donnent la possibilité de _composantiser_ le WEB avec de petits
modules reutilisable qui s'intègre dans des applications
WEB comme dans un puzzle.   
Le plus intéresssant et qu'il ne sont dépendant d'aucun
framework car il sont écrit en pur HTML, CSS et JavaScript.
Pour autant, il n'empeche pas de pouvoir écrire ces composants à l'aide d'un framework
mais il seront alors encapsulés dans le web component.


_The difference between an app and a component has nothing to do with the amount of code it has, I like to put it simple: apps don't depend on others to live, while a component can only work within an app._

## Links

[Building Microfrontends](https://medium.com/@_rchaves_/building-microfrontends-part-i-creating-small-apps-710d709b48b7)

[Frameworks vs Web Components](https://medium.com/@oneeezy/frameworks-vs-web-components-9a7bd89da9d4)

[Micro frontends](https://medium.com/@tomsoderlund/micro-frontends-a-microservice-approach-to-front-end-web-development-f325ebdadc16)