# Projet-technique-de-programmation

Ce projet s'inscrit dans le cadre de nôtre cours de programmation de l'UE 13 technique de programmation du master 1 Analyse et politique économique, parcours Data Science pour l'économie de l'entreprise et du futur (DS2E) & statistique économétrie (SE).
Il a pour but de faire un webscraping du site web de l'agence immobilière Nexity (www.nexity.fr) afin d'avoir une alerte par mail des offres de logement disponible qui répondent aux critères ci-dessous :

- Type de bien : maison ou appartement
- Localisation : Strasbourg
- Loyer mensuel maximum : 1000 €
- Autres critères : meublé ou non 

Pour que les codes fonctionnent normalement sans trop de difficulté, il faut au préalable importer certains packages dans python. Nous avons utilisé la version 3.9 de python ensuite installé les packages qui suivent :

- Beautyfulsup (from bs4)
- numpy (as np)
- time
- pandas (as pd)
- requests
- MIMEtext (from email.mime.text)
- MIMEapplication (email.mime.application)
- MIMEmultipart (email.mime.mutipart)
- Urllib3
- re
- ceil (from math)
- SMTP
- smtplib
- random
- sys
- math
- intertools (as it)

Description des codes:

Pour mener ce projet la première des choses à faire c'est bien évidemment de trouver un site "webscrapable".
Aprés cela, nous avons utilisé des fonctions permettant de recupérer les données html du site et de les stocker dans un data frame.
Ensuite, nous avons créée une boucle qui filtre toutes les informations qui répondent à nos critère sur l'ensemble des données se trouvant sur le site. 
Enfin, nous avons utilisé une autre fonction qui permet d'envoyer une alerte par mail dès qu'il y a une offre répondant à nos critères.
Cette alerte sera sous forme de tableau qui en plus des critères cités ci-dessus contient également les liens des offres. En cliquant sur un lien, il nous renvoie sur l'offre sélectionnée et on peut voir toutes les informations sur ce logement.

Nous nous sommes assurés d'avoir un code lisible et compréhensible pour tout le monde. Pour cela, on a mis des commentaires dans les codes pour que ça soit plus compréhensible.
A noter que ce code s'applique aussi pour des projets d'offre d'emploi, d'achat de bien (ex : billets d'avion) etc. 
De plus, vous pouvez l'appliquer pour vous-même en modifiant juste l’adresse e-mail «XXXXXX@gmail.com » et en mettant la vôtre à la place. De ce fait, vous recevrez quotidiennement un tableau avec toutes les offres de logements disponibles répondant aux critères définis.

Assane, Djenabou, Mouhamed
