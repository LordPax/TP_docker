
# Docker - TP3 : Création d'un environnement Docker-Compose 
> **Objectifs du TP** :
>- Manipulation avancée de Docker-Compose
>

## 1 - Créer un environnement de développement

Vous trouverez un dossier `application` qui comporte une API Rest Express - PostgreSQL. 

- Création d'un docker-compose.yaml afin de servir l'application.
- Pensez à utiliser le concept de Networks tel que vu précédemment.

## 2 - Créer un environnement de production 

- Créez l'(es) image(s) Dockerfile permettant de préparer l'environnement de Production.
- Pushez sur un repo public DockerHub les images créées.
- Lancez en local la commande `docker container run` en utilisant l'(es) image(s) que vous avez créées.

## 3 - Optimiser l'environnement de production 

Maintenant que vous avez une application fonctionnelle, vous allez devoir optimiser l'image Dockerfile de l' `api`.

- Pour en faire l'optimisation rappelez-vous de tout ce qu'on a vu ensemble sur les différents Concepts autour de Dockerfile.

**L'étudiant ayant l'image `api` la plus petite (et fonctionnelle) se verra attribuer +1 point supplémentaire sur sa note de partiel.**
