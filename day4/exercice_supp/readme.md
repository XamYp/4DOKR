Consignes :
1) Créer un dockerfile pour créer une image nginx.
2) Dans le dockerfile exposé le port 80 et copier le fichier de configuration nginx au bon emplacement dans votre image.

Votre docker compose devra contenir :
4 services :
- weather-app1
- weather-app2
- weather-app3
- nginx

2 réseaux :
- frontend
- weather_app (interne)

Vous devrez construire les images weather-app à partir du dockerfile contenu dans le dossier weather-app et l'image nginx à partir du dockerfile que vous aurez créé dans le dossier nginx.
L'image construire de weather-app devra contenir l'argument "VERSION=v2.0"
Chaque service weather-app devra avoir comme variable d'environnement "NODE_ENV=production" et avoir le réseau "weather_app".
Le service nginx devra avoir le "tty" d'activé.
