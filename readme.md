4. Accéder à l'application :
    - Frontend : [http://frontend.local](http://frontend.local)
    - Backend API : [http://backend.local](http://backend.local)

## Structure du Projet :

- **bank-service/** : Contient le code source de l'application Spring Boot et le Dockerfile pour construire l'image Docker.
- **bank-web/** : Contient le code source de l'application Angular et le Dockerfile pour construire l'image Docker avec Apache2.
- **traefik/** : Contient les fichiers de configuration pour Traefik.
- **docker-compose.yml** : Fichier de configuration Docker Compose pour orchestrer les services.
- **README.md** : Instructions pour exécuter le projet.

## Points Importants :

- **Traefik v3** est configuré comme reverse proxy pour router les requêtes vers les services Angular et Spring Boot.
- **Labels Docker** sont utilisés pour le routage dynamique avec Traefik.
- **Health checks** sont configurés pour chaque service dans les Dockerfiles respectifs.

## Ressources Utiles :

- [Documentation Officielle de Docker](https://docs.docker.com/)
- [Documentation Officielle de Traefik v3](https://doc.traefik.io/traefik/)