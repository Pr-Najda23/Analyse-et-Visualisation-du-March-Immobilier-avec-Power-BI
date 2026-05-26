🏠 Projet BI — Analyse Immobilière (Power BI)
📌 Présentation

Ce projet consiste à développer des tableaux de bord interactifs sous Power BI afin d’analyser le marché immobilier marocain à partir de données extraites de Avito.ma.

Le Data Warehouse est organisé en deux schémas :

bi_schema → utilisé pour la Business Intelligence (ce projet)
ml_schema → destiné au Machine Learning (non utilisé ici)

👉 Seul le schéma bi_schema est exploité pour l’analyse et le reporting.

🎯 Objectifs
Connexion de Power BI au Data Warehouse
Importation des données depuis bi_schema
Nettoyage et transformation via Power Query
Création de KPI avec DAX
Conception de dashboards interactifs pour l’analyse du marché immobilier
📊 Tableaux de bord
1️⃣ Vue globale du marché
Nombre total d’annonces
Prix moyen
Répartition des annonces par ville
Évolution du marché dans le temps
2️⃣ Analyse des prix
Distribution des prix
Prix moyen au m²
Comparaison par segment
3️⃣ Analyse géographique
Répartition des annonces par ville
Visualisation sur carte
Zones les plus chères
4️⃣ Analyse des tendances
Évolution des prix
Évolution du volume d’annonces
Tendances saisonnières
🎛️ Filtres disponibles
Ville
Type de bien
Fourchette de prix
Surface
Date

👉 Tous les visuels sont interactifs et dynamiques.

🛠️ Technologies utilisées
Power BI
Power Query
DAX (Data Analysis Expressions)
SQL (PostgreSQL)
Python (ETL & Data Pipeline)
🔁 Pipeline du projet

Données → ETL (Python) → Data Warehouse → Power BI → Dashboards
