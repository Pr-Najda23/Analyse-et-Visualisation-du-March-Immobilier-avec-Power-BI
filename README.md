🏠 Real Estate BI Analytics — Power BI Project
📌 Contexte

Ce projet a pour objectif d’analyser le marché immobilier marocain à partir de données issues de Avito.ma, en construisant des tableaux de bord interactifs avec Power BI.

Le Data Warehouse est organisé en deux schémas :

bi_schema → utilisé pour la Business Intelligence (ce projet)
ml_schema → destiné au Machine Learning (non exploité ici)

👉 L’analyse et les dashboards reposent uniquement sur bi_schema.

🎯 Objectifs du projet

Connecter Power BI au Data Warehouse (PostgreSQL)
Importer les données depuis bi_schema
Nettoyer et transformer les données avec Power Query
Créer des indicateurs clés de performance (KPI) avec DAX
Développer des dashboards interactifs pour l’analyse du marché

📊 Dashboards développés

1️⃣ Vue globale du marché
Nombre total d’annonces
Prix moyen du marché
Répartition des annonces par ville
Évolution temporelle des listings

2️⃣ Analyse des prix
Distribution des prix
Prix moyen au m²
Comparaison des segments immobiliers


3️⃣ Analyse géographique
Répartition des annonces par ville
Visualisation cartographique
Identification des zones les plus chères


4️⃣ Analyse des tendances
Évolution des prix dans le temps
Variation du volume des annonces
Analyse des tendances saisonnières


🎛️ Filtres interactifs
Ville
Type de bien (appartement, maison, etc.)
Fourchette de prix
Surface
Période temporelle

👉 Tous les visuels sont dynamiques et filtrables.

🛠️ Stack technique
Power BI → Visualisation et dashboards
Power Query → Transformation des données
DAX → Calcul des KPI
PostgreSQL → Data Warehouse
Python → ETL et ingestion des données

🔁 Architecture du projet

Scraping / Data Source → ETL (Python) → Data Warehouse (bi_schema) → Power BI → Dashboards
