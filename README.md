# MINI-PROJET-FLUX-RSS
L’objectif de ce mini projet est de développer un lecteur de flux RSS Use case: 
● récupérer le flux du 'le monde' https://www.lemonde.fr/rss/en_continu.xml 
● l'afficher sous un format listing avec image et extrait 
● prévoir la pagination ● pouvoir modifier le titre 
● pouvoir modifier l'extrait

Pour récupérer le flux rss j’ai utilisé rss2json qui est une bibliothèque qui permet de récupérer un flux rss en format json. En effet le flux rss retourne du xml et il est plus facile de gérer du json que du xml.
A partir de là il ne restait plus qu’à faire une requête http avec le module http Client de Angular et récupérer le flux de données.
J’ai ensuite utilisé nodeJS avec  le Framework expressJS pour concevoir un petit serveur qui nous a permis de déployer  l’appli sur Heroku.
Pour les use cases « modifier titre » et « modifier extrait » j’ai juste utilisé les formulaires simples de Angular (FormsModule).  Avec le « 2 way binding » le titre et l’extrait peuvent être modifiés directement à travers un pop-up.


Pour tester l'application:
Lien Heroku https://fluxreader.herokuapp.com/
ou bien Cloner le projet, aller dans le repertoire racine faire "npm install" et ensuite "ng serve"
