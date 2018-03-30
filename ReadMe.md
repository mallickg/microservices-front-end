# MicroServices Frond-End - Pilot Project

## Liste des tâches à effectuer

- [ ] Receuil d'experience (BLSNet/Application Monolithique)
- [ ] Quelles alternatives au monolithique ?
- [ ] Comment faire du micro services front end ?
- [ ] IFrames - Comment ca fonctionne ?
- [ ] IFrames - Avantages / Inconvénients 
- [ ] Customs Elements - Comment ca fonctionne ?
- [ ] Customs Elements - Avantages / Inconvénients
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

_The difference between an app and a component has nothing to do with the amount of code it has, I like to put it simple: apps don't depend on others to live, while a component can only work within an app._

