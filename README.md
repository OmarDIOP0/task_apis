# Projet de Gestion de Tâches NestJS

Ce projet est une application NestJS qui gère des tâches avec une API CRUD. Elle utilise SQLite comme base de données. Le projet possède deux branches :
- `main` : Expose une API CRUD pour les tâches.
- `with-auth` : Ajoute des fonctionnalités d'authentification, y compris l'inscription, la connexion, la mise à jour du profil, et nécessite une authentification pour effectuer les opérations CRUD sur les tâches.

# Comment Exécuter le Projet en Local
## Prérequis
- Node.js (>=14.x)
- npm (>=6.x)
- SQLite
- Installation

## 1. Clonez le dépôt :

## 2. Installez les dépendances :
```bash
npm install
```

## 3. Créez et configurez la base de données SQLite :
- Assurez-vous que SQLite est installé.
- Configurez le fichier config/config.json avec les paramètres appropriés.

## 4. Exécutez les migrations :
```bash
npx sequelize-cli db:migrate
```

# Exécution du Projet
1. Démarrez le serveur NestJS :
```bash
npm run start
```

2. Le serveur devrait maintenant être en cours d'exécution à `http://localhost:3000`.

3. Le projet utilise Swagger pour la documentation de l'API. Après avoir démarré le serveur, vous pouvez accéder à la documentation de l'API à `http://localhost:3000/api-docs`

# Branches

## Branche `main`

La branche `main` expose une API CRUD pour les tâches. Vous pouvez utiliser cette branche pour gérer les tâches sans authentification.

## Branche `with-auth`

La branche `with-auth` inclut des fonctionnalités d'authentification. Elle ajoute les points de terminaison suivants :

- `/auths/register`
- `/auths/login`
- `/auths/profils`

Elle nécessite également une authentification pour les opérations CRUD sur les tâches.

Pour passer à la branche with-auth, utilisez :

```bash
git checkout with-auth
```
