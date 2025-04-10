# docker-citation-app

TP_DOCKER_Marwan_GHRAIRI

Description
L'application consiste en une API backend Node.js et une interface frontend React. L'API retourne une citation aléatoire parmi une liste de trois citations statiques. Le frontend consomme cette API pour afficher la citation du jour sur une interface web simple.

Fonctionnalités :
- Backend Node.js expose une route "/quotes" pour retourner une citation aléatoire en format JSON.
- Frontend React récupère la citation via une requête HTTP et l'affiche à l'utilisateur.

Prérequis
Avant de démarrer le projet, assurez-vous d'avoir installé Docker et Docker Compose sur votre machine.

Lancer l'application avec Docker

1 Cloner ce dépôt

git clone https://github.com/votre-utilisateur/citation-app.git
cd citation-app

2 Lancer Docker Compose

Dans le répertoire racine de votre projet, exécutez la commande suivante pour construire et démarrer les conteneurs Docker :

docker-compose up --build

    --build : Cette option force Docker Compose à reconstruire les images avant de démarrer les conteneurs.

3 Accéder à l'application

    Backend (API) : L'API backend sera disponible sur http://localhost:5000/quotes.

    Frontend (UI) : L'interface frontend sera disponible sur http://localhost:3000.

4 Arrêter les conteneurs

Pour arrêter les conteneurs Docker en cours d'exécution, utilisez :

docker-compose down

Structure du Projet

/citation-app
├── /backend            # Code de l'API backend (Node.js)
├── /backend/Dockerfile # Dockerfile pour le backend
├── /frontend           # Code du frontend (React)
├── /frontend/Dockerfile # Dockerfile pour le frontend
├── docker-compose.yml  # Configuration Docker Compose
└── README.md           # Ce fichier
