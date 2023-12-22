
# Docker NGINX et PHP Application

Ce projet configure un environnement Docker comprenant un serveur web NGINX et une application PHP, gérée à l'aide de Docker Compose.

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
   git clone [URL_DU_DEPOT]
   ```

2. Naviguer dans le répertoire du projet :

   ```
   cd [NOM_DU_REPERTOIRE]
   ```

## Déploiement

Exécuter la commande suivante pour démarrer les services en utilisant Docker Compose :

```
docker-compose up -d
```

## Configuration NGINX

Les configurations NGINX sont stockées dans le dossier `./nginx`. Vous pouvez les modifier selon vos besoins pour gérer la manière dont NGINX traite les requêtes entrantes et les redirige vers l'application PHP.

## Licence

[CHOISIR LA LICENCE APPROPRIÉE]

## Contact

[INFORMATIONS DE CONTACT]
