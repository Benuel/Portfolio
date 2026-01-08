# Estimation du nombre de festivaliers

> **Entreprise :** Couleur Café <br>
> **Projet :** Estimation du nombre de festivaliers <br>
> **Rôle :** Co-Auteur / Développeur <br>
> **Statut :** Actif <br>
> **Chronologie :** 2025 <br>
> **Stack Technique :** Python, Flask, SocketIO, JS, Tailwind CSS, PyTorch, OpenCV

> [🇬🇧 Read in English](./README.md)

## Vue d'ensemble

**Estimation du nombre de festivaliers** est une application web en temps réel conçue pour visualiser la densité de foule sur plusieurs lieux d'un festival. Optimisée pour un affichage sur grand écran dans les salles de contrôle, elle aide les équipes de sécurité à surveiller les flux de festivaliers.


## Fonctionnalités

![Screenshot](assets/Screenshot.png)

*   **Données en Direct :** Affiche le nombre total de personnes et la densité (personnes/m²) pour plusieurs scènes.
*   **Vérification Visuelle :** Affiche l'image traitée correspondante pour une confirmation visuelle instantanée.
*   **Alertes Intelligentes :** Utilise des seuils de couleur configurables (Vert/Orange/Rouge) pour signaler immédiatement les zones surpeuplées.
*   **Navigation Temporelle :** Permet aux opérateurs de parcourir l'historique et de revoir les états passés de la foule.
*   **Mode Direct :** Se met à jour automatiquement dès que de nouvelles analyses sont disponibles.

---

## Architecture Technique

Le système fonctionne sous forme de pipeline :
1.  **Ingestion :** Extrait les flux vidéo RTSP des caméras de sécurité.
2.  **Analyse :** Un modèle IA en Python (utilisant le projet pré-entraîné **APGCC**) traite les images pour détecter les personnes et estimer la densité.
3.  **Distribution :** Un backend Flask diffuse les mises à jour via WebSockets (Flask-SocketIO).
4.  **Affichage :** Un tableau de bord réactif en HTML5 et Tailwind CSS présente les données.

---

## Confidentialité

> **Note :** Le code source complet, les configurations détaillées des modèles IA et les scripts de déploiement ne sont pas disponibles publiquement. Ce dépôt sert uniquement de vitrine pour présenter le produit et ses capacités.
