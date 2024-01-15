# Projet Immobilier
Ce dépôt contient plusieurs services liés à la gestion immobilière. Chaque service est conteneurisé et peut être lancé indépendamment ou ensemble en utilisant Docker Compose.

## Services inclus
### 1. API Auto
   La partie backend de l'application immobilière, écrite en PHP. Cette API est accessible à l'adresse http://api.auto.local:2080.

### 2. Base de données Auto
   Un conteneur MySQL utilisé par l'API Auto. Il expose le port 18252 pour accéder à la base de données.

### 3. Adminer
   Un outil d'administration de base de données accessible à l'adresse http://localhost:8080. Utilisez-le pour visualiser et gérer la base de données MySQL.

### 4. Auto.Client
   Une application frontend Vue.js basée sur VITE. Elle est accessible à l'adresse http://localhost:3000.

### 5. Auto.Admin
   Une application frontend React.js basée sur VITE. Elle est accessible à l'adresse http://localhost:3001.

## Prérequis

Assurez-vous d'avoir les outils suivants installés sur votre machine :
- Docker
- Node.js (version 14 ou supérieure)

## Installation et exécution

1. Clonez ce dépôt sur votre machine locale :

```bash
git clone https://github.com/Leonarddoo/Immo/tree/develop
cd projet-immobilier
```

2. Pour lancer tous les services, utilisez la commande Docker Compose suivante :
````bash
docker-compose up --build
````

3. Les différents services seront accessibles aux adresses spécifiées ci-dessus.

## Notes importantes
Assurez-vous que les ports spécifiés dans le fichier docker-compose.yml ne sont pas déjà utilisés sur votre machine.
Chaque service a son propre répertoire avec un fichier Dockerfile pour la construction de l'image Docker.

## Contributors
- DELLINGER Agathe
- POMIN Samuel
