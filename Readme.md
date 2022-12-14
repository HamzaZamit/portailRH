#
## _Portail RH :_



[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master#)](https://travis-ci.org/joemccann/dillinger)

Le portail RH est une plateforme web qui offre aux collaborateurs, managers et
services RH, un outil puissant mettant à leur disposition de nombreuses
fonctionnalités, des indicateurs et un moyen de faciliter l’accès aux données RH.


## Features
un compte salarié qui pourra exécuter les tâches suivantes :
- Demander et télécharger une attestation de travail, attestation de salaire => le
  téléchargement de l’attestation passe par la validation de la RH tout en gardant
  l’historique des documents envoyés avec la date d’envoie et la date de la
  demande.
- Avoir une idée sur les compétences des autres collaborateurs :
- Accéder à Udemy (lien, login , formations disponibles par catégorie)
- Partager les connaissances entre les collaborateurs (des articles intéressants ,
  des trucs dans plusieurs domaines )
- Lors du son départ ( récupération des matériels ) : il peut passer quiz

Le service Rh peut  :
- Recevoir des demandes spécifiques de chaque collaborateur tout en gardant
  une traçabilité de ces échanges.
- Recevoir des alertes sur les événements concernant les salariés. Par exemple,
  la fin de période d’essai ou de contrat, les dates de visites médicales, les
  formations à prévoir, etc..).
- récupérer l'historique de génération des documents par date ou client .

Le manager peut :
- Gérer les demandes d’absence, de formation, prendre connaissance des
  entretiens professionnels.
- Préparation des templates compte rendu des entretiens annuels (interne)
- Gérer les demandes d’absence, de formation, prendre connaissance des
  entretiens professionnels.



## Tech

Le portail RH utilise un certain nombre de projets open source pour fonctionner correctement :

- [Java 11 ] - En tant que langage de programmation Backend
- [Springboot ] - En tant que Framework de programmation Backend
- [PostgreSQL] - En tant que système de gestion de base de données relationnelle
- [Angular] - En tant que Framework de programmation Frontend
- [Swagger] - utilisé pour partager la documentation entre les chefs de produit, les testeurs et les développeurs


## Installation
Premiere Etape :
Installer les Node modules
```sh
npm install
```
Deuxième Etape :
Lancer les contenuers du Back-End , Front-End et de la base des données
```sh
sudo docker-compose up  --build -d
```

## Tester l'Application

Vous voulez tester ? Génial !

Ouvrez votre navigateur et lancez

```sh
http://localhost:8080
```

Pour tester vos REST APIs , Ouvrez Postman et exécutez
```sh
http://localhost:8091/login
```
Génial : Vous disposez d'un jeton d'accès (ACEESS_TOKEN)
Vous pouvez maintenant tester tous vos APIs  sur Postman (Authorization Type : Bearer token)
NB : Le localhost peut être remplacé par L'URL et le port de votre environnement PROD .

Si vous voulez tester vos APIs REST grace à l'outil de test Swagger , Ouvrez votre navigateur et lancez :
```sh
http://localhost:8091/swagger-ui.html#/
```

Cliquez sur Autoriser et mettez dans la case appelée "Value"
Bearer [ACEESS_TOKEN]
NB : L'ACEESS_TOKEN doit etre remplacé par l'acess token obtenu a travers postman .
Cliquez ensuite sur le bouton "Authorize"

Félicitations, vous avez maintenant toutes vos API prêtes à être exécutées

NB : les coordonnées de la base des données sont indiqué dans le docker-compose File .
## Supervisé par
RedLean Services
## Contact
alaa.mzoughi@redlean.io

  
