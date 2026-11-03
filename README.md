# Application Web de Réservation des Ressources d’un Data Center

<p align="center">
  <strong>Projet académique — Développement Web</strong><br>
  Application de gestion, réservation et suivi des ressources informatiques d’un Data Center.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</p>

---

## Présentation du projet

Ce projet consiste à concevoir et développer une application web permettant de gérer les ressources informatiques d’un Data Center et de faciliter leur réservation, leur allocation et leur suivi.

La plateforme centralise les ressources disponibles et permet aux différents utilisateurs d'effectuer des demandes de réservation, de suivre leur état et de gérer les disponibilités.

L'application repose sur une architecture développée avec **Laravel (PHP)** et une base de données relationnelle **MySQL**.

## Objectifs

- Concevoir et gérer une base de données relationnelle.
- Développer une interface web ergonomique, sécurisée et responsive.
- Faciliter la réservation et la gestion des ressources informatiques.
- Vérifier automatiquement les disponibilités et prévenir les conflits.
- Mettre en place un système de gestion des rôles et des permissions.
- Assurer la traçabilité des opérations et le suivi des réservations.
- Fournir des statistiques et des tableaux de bord.

## Types d'utilisateurs

La plateforme prévoit quatre profils avec des responsabilités distinctes.

| Profil | Responsabilités principales |
|---|---|
| Invité | Consulter les ressources disponibles et demander l'ouverture d'un compte. |
| Utilisateur interne | Consulter les ressources, effectuer des réservations et suivre ses demandes. |
| Responsable technique | Gérer les ressources sous sa responsabilité et traiter les demandes associées. |
| Administrateur | Gérer les utilisateurs, les rôles, les ressources, la maintenance et les statistiques globales. |

## Fonctionnalités principales

### 1. Gestion des ressources
- Gestion des serveurs physiques et machines virtuelles.
- Gestion des espaces de stockage et des équipements réseau.
- Consultation des caractéristiques techniques : CPU, RAM, capacité, système d'exploitation et emplacement.
- Gestion de l'état et de la disponibilité des ressources.
- Planification des périodes de maintenance.

### 2. Système de réservation
- Consultation des ressources disponibles.
- Création de demandes avec période, ressources souhaitées et justification.
- Vérification des disponibilités.
- Détection et gestion des conflits de réservation.
- Suivi des demandes selon leurs statuts : En attente, Approuvée, Refusée, Active et Terminée.
- Consultation de l'historique des réservations.

### 3. Gestion des utilisateurs et des permissions
- Authentification des utilisateurs.
- Gestion des profils et des rôles.
- Contrôle des accès selon les responsabilités.
- Activation et désactivation des comptes.

### 4. Notifications et traçabilité
- Notifications relatives aux demandes de réservation.
- Suivi des changements de statut.
- Signalement des incidents techniques.
- Journalisation des opérations importantes.

### 5. Tableaux de bord et statistiques
- Visualisation des statistiques.
- Suivi du taux d'occupation des ressources.
- Consultation des réservations et de leur évolution.

## Technologies et outils

| Domaine | Technologies |
|---|---|
| Backend | PHP, Laravel |
| Base de données | MySQL |
| ORM | Eloquent |
| Frontend | HTML5, CSS3, JavaScript |
| Gestion des routes | Laravel Routing |
| Validation | Laravel Validation |
| Base de données | Migrations Laravel |

**Contrainte de développement frontend :** CSS et JavaScript personnalisés, sans Bootstrap, Tailwind CSS ni jQuery.

## Architecture générale

```text
              Utilisateurs
                   |
                   v
          Interface Web
          HTML / CSS / JS
                   |
                   v
             Laravel
          Application Backend
                   |
       +-----------+-----------+
       |           |           |
       v           v           v
 Gestion des   Réservations  Authentification
 ressources    et suivi      et permissions
       |           |           |
       +-----------+-----------+
                   |
                   v
                MySQL
             Base de données
                   |
                   v
       Statistiques et historique
```

## Installation et exécution

### Prérequis
- PHP
- Composer
- MySQL
- Laravel
- Serveur local (XAMPP, par exemple)

### 1. Cloner le dépôt

```bash
git clone https://github.com/elmaymounizakariae-dotcom/Application-Web-de-R-servation-des-Ressources-d-un-Data-Center.git

cd Application-Web-de-R-servation-des-Ressources-d-un-Data-Center
```

### 2. Installer les dépendances

```bash
composer install
```

### 3. Configurer l'environnement

```bash
cp .env.example .env
```

Configurer ensuite les paramètres de connexion MySQL dans le fichier `.env`.

### 4. Générer la clé de l'application

```bash
php artisan key:generate
```

### 5. Exécuter les migrations

```bash
php artisan migrate
```

### 6. Démarrer le serveur

```bash
php artisan serve
```

L'application sera accessible à l'adresse :

`http://127.0.0.1:8000`

## Dépôt GitHub

**Source code :** [Application Web de Réservation des Ressources d’un Data Center](https://github.com/elmaymounizakariae-dotcom/Application-Web-de-R-servation-des-Ressources-d-un-Data-Center)

---

<p align="center">
  <strong>Projet académique — Développement Web</strong><br>
  PHP · Laravel · MySQL
</p>