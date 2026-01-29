# NimblePhysics Setup pour PhysioEvaLab

Configuration et fichiers pour le déploiement de NimblePhysics sur le serveur.

## Fichiers

- `nginx-nimble.conf` : Configuration nginx pour /nimble/ et /nimble-ws
- `bundle.js` : Client web patché (WebSocket via nginx)
- `wiki-page.txt` : Page wiki DokuWiki
- `README.md` : Ce fichier

## Utilisation

Voir la page wiki : https://192.168.0.56/dokuwiki/doku.php?id=apps:nimblephysics

## Architecture

- Frontend : /var/www/nimble/
- WebSocket proxy : nginx /nimble-ws -> localhost:8070
- Docker image : nimblephysics:working
- Kernel Jupyter : nimblephysics-docker

