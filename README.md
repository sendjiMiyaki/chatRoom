# ChatRoom

ChatRoom est une application de chat en ligne permettant à plusieurs utilisateurs de se connecter à des **rooms** (salles de discussion) en temps réel. Chaque room peut accueillir jusqu'à **10 utilisateurs** et offre la possibilité de discuter de manière sécurisée (HTTPS).

## Fonctionnalités

- **Créer une room** : Permet à un utilisateur de créer une room avec un **id unique** et un **mot de passe (optionnel)**.
- **Rejoindre une room** : Les utilisateurs peuvent rejoindre une room en utilisant l'**id** de la room et, si nécessaire, le mot de passe.
- **Gestion des utilisateurs** : Chaque utilisateur peut choisir un **username unique pour chaque room** ou utiliser un **même username pour toutes les rooms**.
- **Messages en temps réel** : Les messages sont échangés en temps réel dans chaque room.
- **Sécurité** : Le site fonctionne en **HTTPS** et l'accès aux rooms privées est protégé par mot de passe.
- **Limitation** : Chaque room peut accueillir jusqu'à **10 utilisateurs maximum**.

## Technologies utilisées

- **Frontend** : React.js (pour l'interface utilisateur dynamique)
- **Backend** : Node.js avec Express.js (pour gérer les routes API)
- **Base de données** : MongoDB (stockage des rooms, utilisateurs et messages)
- **Communication en temps réel** : Socket.io (pour la messagerie en temps réel)
- **Sécurité** : HTTPS, JWT pour l'authentification des utilisateurs

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les éléments suivants :

- **Node.js** (version 14.x ou supérieure)
- **MongoDB** (ou utiliser MongoDB Atlas)
- **npm** (ou yarn)

## Installation

### Clonez ce repository :

```bash
git clone https://github.com/sendjiMiyaki/chatRoom.git
cd chatRoom
```

### Installation des dépendances

1. **Backend** :
   - Allez dans le dossier du backend : `cd backend`
   - Installez les dépendances :

   ```bash
   npm install
   ```

2. **Frontend** :
   - Allez dans le dossier du frontend : `cd frontend`
   - Installez les dépendances :

   ```bash
   npm install
   ```

### Configuration

1. **Backend** : Créez un fichier `.env` à la racine du dossier `backend` et ajoutez vos variables d'environnement :
   
   ```
   MONGO_URI=<votre-uri-mongodb>
   JWT_SECRET=<votre-clé-secrète-pour-JWT>
   ```

2. **Frontend** : Aucune configuration spécifique pour l'instant, mais vous pouvez modifier les appels API dans le code frontend pour correspondre à l'URL de votre serveur backend si nécessaire.

### Démarrage de l'application

1. **Backend** :
   - Dans le dossier `backend`, lancez le serveur :

   ```bash
   npm start
   ```

2. **Frontend** :
   - Dans le dossier `frontend`, lancez l'application React :

   ```bash
   npm start
   ```

   L'application sera accessible sur [http://localhost:3000](http://localhost:3000).

## Utilisation

1. **Créer une room** : Cliquez sur "Créer une room" et donnez-lui un nom. Vous pouvez choisir d'ajouter un mot de passe pour rendre la room privée.
2. **Rejoindre une room** : Entrez l'**id de la room** et, si nécessaire, le **mot de passe**.
3. **Envoyer des messages** : Tapez votre message dans la zone de chat et appuyez sur "Envoyer". Les messages seront envoyés en temps réel à tous les utilisateurs connectés dans la room.
4. **Quitter une room** : Vous pouvez quitter la room à tout moment en cliquant sur "Quitter la room".

## Contribuer

Les contributions sont les bienvenues ! Si vous avez des idées ou des améliorations à proposer, n'hésitez pas à ouvrir une **issue** ou à soumettre une **pull request**.

### Étapes pour contribuer :

1. Fork ce repository.
2. Créez une nouvelle branche (`git checkout -b feature-nouvelle-fonctionnalité`).
3. Faites vos changements.
4. Commitez vos changements (`git commit -m 'Ajout d'une nouvelle fonctionnalité'`).
5. Poussez sur votre fork (`git push origin feature-nouvelle-fonctionnalité`).
6. Ouvrez une pull request pour que nous puissions revoir vos changements.

## License

Ce projet est sous la **MIT License**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
