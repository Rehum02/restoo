
## Restoo 
  Restoo. Vos plats preférés proches de vous. Commandez, vous êtes livrés
  
  

## Introduction
Restoo est une plateforme mettant en relation des restaurants et des clients.
Restoo est actuellement opérationnelle.
C'est une plateforme test servant juste d'échantillon comme demandé  au terme de l'entretien, en prelude au projet proprement dit.

## Apercu 
Vous pouvez voir des images de la plateforme dans le dossier restoo_screen_shot.

## Fonctionnalités

Technolgies utilisées 

- Front-End : Vue 2.6.11
- Back-End : Nodejs 14.17.4
- Base de données : MongoDB 

Note: Ne disposant pas de serveur en ligne pouvant heberger une base de données MongoDB, l'application n'a pu être deployée en ligne.
Pour deployer sur un serveur en ligne, vous pouvez vous referer à la section "Deploiement en ligne" ou me communiquer les coordonnées de votre serveur pour que je puisse effectuer le deploiement.

## Fonctionnalités

- Possibilité pour un restaurant et un client de s'inscrire
- Possibilité pour un restaurant de definir ses plats 
- Possibilité pour un restaurant et un client de voir leurs differentes commandes
- Possibilité pour un restaurant de voir sa balance 
- Possibilité pour un client d'editer ses données personnelles
- Possibilité pour un client de faire une commande 

 
## Procedure Installation locale 
* INSTALLATION DE MONGODB
        - Télécharger MongoDB sur le site officiel
        - Installer MongoDB  et l'executer
        (Vous pouvez voir les differents documents,les collections, la db avec MongoDBCompass)

* INSTALLATION DU BACKEND 
        - Aller dans le dossier restoo_backend
        - Telecharger le dossier
        - Se mettre dans le dossier, ouvrir l'invite de commande  et faire  ```  npm install ```
        - Dans le dossier Backend , Aller à assets/custom_scripts . Dans ce dossier, ouvrir le  fichier app.const.js Editer les propriétes du serveur SMTP pour l'envoi d'email essentiellement de la propriété CONST_BASE_MAIL_ENCODING  à CONST_BASE_MAIL_PORT 
        - Connexion à la base de données, toujours dans le dossier custom_scripts, ouvrir le fichier mongodb.scheme.js . Mettre le lien de la connexion à la bd mongodb locale . Par default c'est mongodb://localhost:27017. Vous pouvez laisser si c'est identique
        - Faire  ```npm run script ``` pour demarrer le serveur


* INSTALLATION DU FRONTEND  
        - Aller dans le dossier restoo_frontend__source
        - Telecharger le dossier
        - Se mettre dans le dossier et faire npm install
        - Faire  ```npm run script ``` pour demarrer lancer l'app


## Procedure deploiement en ligne 
 * MONGODB
        - Verifier la presence de Mongodb

 * INSTALLATION DU BACKEND 
        - Installer NodeJS sur le serveur . Le Backend peut etre à un url sous-domaine ou un domaine. 
        - Aller dans le dossier restoo_backend
        - Uploader tout le contenu du dossier à la racine du serveur 
        - Faire  ``` npm install  ``` ou cliquer sur le bouton d'execution du fichier package.json


 * INSTALLATION DU FRONTEND  
        - Aller dans le dossier restoo_frontend__online
        - Mettre la valeur url du backend dans la propriété  CONST_BACKEND_ROOT_PATH
        - Uploader tout le contenu du dossier à la racine du serveur
        - lancer l'app

## Credit 
Miché KOKORA.
Je reste disponible au besoin.
