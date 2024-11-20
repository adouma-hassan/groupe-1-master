Nom1:ADOUMA Hassan
Nom2:Melas Kotin

num_etu1:21901741
num_etu2:22211719


Gestion des Animaux - Projet Web (université de caen normandie)
Description

Ce projet est une application web conçue pour gérer une base de données d'animaux. L'application propose des fonctionnalités de création, de modification, de suppression, et de visualisation des informations des animaux. Elle est développée en PHP en suivant une architecture claire et modulaire qui inclut un routeur, un contrôleur, et des vues (HTML et JSON).
Fonctionnalités principales

    Affichage d'informations sur les animaux :
        Visualiser les informations d'un animal spécifique.
        Voir une liste de tous les animaux enregistrés.

    Création d'animaux :
        Ajouter un nouvel animal à la base via un formulaire.

    Modification des informations des animaux :
        Mettre à jour les informations d'un animal existant.

    Suppression des animaux :
        Supprimer un animal après confirmation.

    Support JSON :
        Fournir les données d'un animal au format JSON pour une intégration ou utilisation externe.

    Navigation dynamique :
        Une page d'accueil intuitive.
        Génération d'URL spécifiques pour chaque action (affichage, modification, suppression, etc.).

Architecture

    Routeur (Router) :
        Gère les URL et détermine quelle action doit être exécutée en fonction des paramètres.
        Fournit des méthodes pour générer des URL pour toutes les actions disponibles.

    Contrôleur (Controller) :
        Contient la logique métier de l'application.
        Permet de gérer les actions comme l'ajout, la mise à jour, ou la suppression d'animaux.
        Interagit avec les modèles et les vues.

    Vues :
        HTML (View) : Génère des pages HTML pour l'utilisateur.
        JSON (ViewJSON) : Fournit des réponses au format JSON pour des usages programmatiques.

    Stockage des données (AnimalStorage) :
        Interface ou classe simulant un stockage persistant des informations des animaux.

Routage

Le routeur est le point central de l'application. Selon les paramètres fournis dans l'URL, il :

    Affiche une liste d'animaux (?liste).
    Affiche les informations détaillées d'un animal spécifique (?action=afficher&id={id}).
    Gère les formulaires de création et de modification d'animaux.
    Fournit des réponses JSON pour une utilisation externe (?action=json&id={id}).

Exemple d'URLs

    Page d'accueil : /site.php
    Liste des animaux : /site.php?liste
    Création d'un nouvel animal : /site.php?action=nouveau
    Modification d'un animal : /site.php?action=modifier&id=1
    Suppression d'un animal : /site.php?action=supprimer&id=1
    Récupération des données en JSON : /site.php?action=json&id=1

Technologies utilisées

    Langage : PHP
    Front-End : HTML/CSS généré dynamiquement.
    Back-End : Architecture MVC en PHP.

Usage

Pour utiliser ce projet, il suffit d'héberger les fichiers PHP sur un serveur local ou en ligne (comme Apache via XAMPP). Assurez-vous que PHP est configuré correctement pour gérer les sessions.
