# Sky-Explorer

## Description

Sky Explorer est une école d'aviation située à Aix les Milles, qui offre des formations pour devenir pilote professionnel ainsi que des activités de loisirs liées à l'aviation. Le projet consiste en le développement d'une plateforme composée de deux outils principaux : un pour la gestion des plannings et de la facturation, et un autre pour le suivi pédagogique des étudiants. Le premier outil est destiné à l'usage exclusif des collaborateurs, tandis que le second est accessible aux collaborateurs et aux étudiants.

## Fonctionnalités

- **Gestion des plannings :** Interface pour gérer les plannings des cours et des activités de loisirs, avec des vues par jour, semaine et mois.
- **Filtrage des plannings :** Possibilité de filtrer les activités affichées (ex : vols de loisir, leçons, etc.).
- **Système de facturation :** Intégration d'un système pour suivre et gérer les paiements des cours et des vols.
- **Suivi financier et statistiques :** Tableaux de bord présentant des bilans financiers et statistiques (temps de vol, nombre de leçons, etc.).
- **Suivi pédagogique :** Interface pour suivre la progression individuelle des étudiants, incluant performances, compétences acquises et objectifs.
- **Communication :** Fonctionnalités de communication pour faciliter les échanges entre collaborateurs et étudiants.
- **Accès sécurisé pour les étudiants :** Permet aux étudiants de consulter leur progression et de recevoir des feedbacks sur leurs performances.
- **Multiplateforme :** Accessible sur desktop, tablette et smartphone.
- **Sécurité et confidentialité :** Mise en œuvre de mesures pour garantir la sécurité et la confidentialité des données.

## Technologies utilisées

- **API :** PHP 8.2 avec Composer et PostgreSQL
- **Front-end :** React

### Prérequis

- PHP 8.2 (avec les extentions activer sodium et pdo_pgsql)
- PostgreSQL
- Node.js pour React
- Composer

### Étapes d'installation du projet

1. **Cloner le dépôt :**
   ```bash
   git clone --recursive hhttps://github.com/qboitel/sky-explorer.git
    ```

### installation sky-explorer-api

#### Prérequis
- PHP 8.2
- Composer
- PostgreSQL

#### Étapes d'installation pour l'API

1. **Placer dans le dossier de l'API, en partant de la racine du projet**
   ```bash
   cd ./sky-explorer-api
   ```

2. **Utiliser les commandes pour initialiser la base de données**
    ```bash
    # Création de la base de données
    php bin/console doctrine:database:create
    # Création des tables de la base de données
    php bin/console doctrine:migrations:migrate
    ```
3. **Création d'un utilisateur**
    ```bash
    php bin/console app:user:create
    # Liste des roles disponibles : ROLE_SUPER_ADMIN, ROLE_ADMIN, ROLE_FORMATEUR, ROLE_USER
    ```
4. **Lancement du serveur**
    ```bash
    php -S 127.0.0.1:8000 -t public/
    ```

### installation sky-explorer-front

#### Prérequis
- Node.js

#### Étapes d'installation pour le front

1. **Placer dans le dossier du front, en partant de la racine du projet**
   ```bash
   cd ./sky-explorer-front
   ```
2. **Installer les dépendances du projet**
    ```bash
    npm install
    ```
3. **Lancement de l'application**
    ```bash
        npm run dev
    ```

## Auteurs

- [crodrigues-dotcom](https://github.com/crodrigues-dotcom)
- [qboitel](https://github.com/qboitel)