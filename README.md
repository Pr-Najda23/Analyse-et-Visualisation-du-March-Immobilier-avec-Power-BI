🏠 Darkom.ma — Data Engineering & BI Pipeline

📊 Pipeline décisionnel complet pour l’analyse du marché immobilier marocain

📚 Aperçu du Projet

Ce projet consiste à concevoir une architecture BI complète permettant de transformer des données immobilières brutes issues de Darkom.ma en tableaux de bord interactifs avec Power BI.

L’objectif principal est de construire un pipeline ETL industriel allant du chargement des données jusqu’à la visualisation décisionnelle.

🏗️ Architecture du Pipeline
       Source CSV
            ↓
     Staging Layer
            ↓
      Clean Layer
            ↓
 Data Warehouse (BI)
            ↓
      Power BI
🎯 Objectifs du Projet

✔ Construire un pipeline ETL complet
✔ Nettoyer et transformer les données immobilières
✔ Concevoir un Data Warehouse optimisé
✔ Développer des KPIs métiers avancés
✔ Créer des dashboards interactifs Power BI
✔ Analyser le marché immobilier marocain

🧱 Structure du Projet
darkom_project/
│
├── data/
│   ├── raw/
│   └── clean/
│
├── logs/
│
├── scripts/
│   ├── staging/
│   ├── cleaning/
│   └── warehouse/
│
├── sql/
│
├── dashboards/
│
├── README.md
└── requirements.txt
🛠️ Technologies Utilisées
Technologie	Utilisation
Python	Pipeline ETL
Pandas	Nettoyage des données
PostgreSQL	Data Warehouse
SQLAlchemy	Connexion PostgreSQL
Power BI	Data Visualisation
Power Query	Préparation des données
DAX	KPIs & Mesures
📥 Source des Données
Fichier utilisé
darkom_annonces.csv
Colonnes disponibles
Colonne	Description
annonce_id	Identifiant unique
date_publication	Date de publication
titre	Titre annonce
ville	Ville
quartier	Quartier
type_bien	Appartement, Villa, Terrain...
transaction	Vente / Location
prix	Prix en MAD
surface	Surface en m²
nb_chambres	Nombre de chambres
nb_salles_bain	Nombre de salles de bain
etage	Numéro d’étage
annee_construction	Année de construction
⚙️ Pipeline ETL
1️⃣ Staging Layer

Cette couche sert de zone temporaire pour le chargement brut des données.

Actions réalisées
Import du fichier CSV vers PostgreSQL
Vérification du chargement
Gestion des logs ETL
Contrôle d’intégrité des colonnes
🧹 2️⃣ Clean Layer

Cette étape permet de nettoyer et standardiser les données.

Nettoyage effectué
✔ Suppression des doublons
✔ Gestion des valeurs manquantes
quartier
nb_chambres
nb_salles_bain
etage
annee_construction
✔ Standardisation des données
Uniformisation des villes
Harmonisation des transactions
Normalisation des types de biens
✔ Traitement des valeurs aberrantes
prix
surface
nb_chambres
✔ Correction des types de données
Conversion DATE
Types numériques
Contrôle cohérence
🧠 Feature Engineering

Création de nouvelles variables analytiques :

Feature	Description
prix_m2	Prix par m²
age_bien	Âge du bien
categorie_prix	Économique / Luxe
categorie_surface	Petit / Moyen / Grand
annee_publication	Analyse temporelle
trimestre_publication	Analyse saisonnière
🏛️ Data Warehouse

Le Data Warehouse est stocké dans :

bi_schema
⭐ Modèle utilisé : Star Schema
Tables de dimensions
dim_date
dim_localisation
dim_bien
dim_transaction
Table de faits
fact_annonces
🔗 Modèle Relationnel
dim_date --------|
                  |
dim_localisation -|---- fact_annonces
                  |
dim_bien ---------|
                  |
dim_transaction --|
📈 KPIs Développés
KPI	Description
Nombre total d’annonces	Volume global
Prix moyen	Prix moyen du marché
Prix moyen par m²	Valeur immobilière
Surface moyenne	Taille moyenne
Croissance des annonces	Évolution temporelle
Répartition des biens	Analyse des catégories
📊 Dashboards Power BI
🌍 Dashboard 1 — Vue Globale
Nombre total d’annonces
Prix moyen du marché
Surface moyenne
Répartition par ville
KPIs interactifs
Répartition Vente vs Location
💰 Dashboard 2 — Analyse des Prix
Distribution des prix
Prix moyen par m²
Analyse des segments immobiliers
Prix par type de bien
Analyse par catégorie de prix
📍 Dashboard 3 — Analyse Géographique
Répartition géographique
Carte des prix immobiliers
Top villes les plus chères
Analyse des quartiers
Classement des zones
📉 Dashboard 4 — Analyse des Tendances
Évolution des prix
Volume des annonces
Analyse saisonnière
Comparaison N vs N-1
Tendances du marché
🎛️ Filtres Dynamiques

Les dashboards intègrent des slicers interactifs :

Ville
Type de bien
Transaction
Surface
Prix
Période
🔍 Validation des Données

Contrôles réalisés :

✔ Cohérence du Data Warehouse
✔ Validation des relations
✔ Contrôle qualité des données
✔ Vérification des types
✔ Validation Power BI

🚀 Résultat Final

Le projet permet d’obtenir :

✅ Pipeline ETL industriel
✅ Data Warehouse optimisé
✅ Dashboards Power BI interactifs
✅ Analyse complète du marché immobilier marocain
