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
