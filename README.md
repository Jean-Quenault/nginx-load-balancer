# Nginx load balancer

Ce projet configure un environnement Docker comprenant un serveur web NGINX et une application PHP en quatres replicas avec Docker Compose.

## Prérequis

- Docker
- Docker Compose

## Configuration

Le fichier `docker-compose.yml` inclut deux services :

1. `webserver` : Un serveur web NGINX configuré pour écouter sur le port 80. Il utilise des configurations personnalisées situées dans le dossier `./nginx`.
2. `app` : Une application PHP exécutée avec Apache, accessible via le serveur NGINX. Ce service est configuré pour démarrer avec 4 réplicas.

## Installation

1. Cloner le dépôt :

   ```
   git clone https://github.com/Jean-Quenault/nginx-load-balancer/tree/main
   ```

2. Naviguer dans le répertoire du projet :

   ```
   cd nginx-load-balancer/
   ```

## Déploiement

Exécuter la commande suivante pour démarrer les services en utilisant Docker Compose :

```
docker-compose up -d
```

L'application affiche ensuite l'id du conteneur solicité (par le load balancer).

## Configuration NGINX

Les configurations NGINX sont stockées dans le dossier `./nginx`. Vous pouvez les modifier selon vos besoins pour gérer la manière dont NGINX traite les requêtes entrantes et les redirige vers l'application PHP.

