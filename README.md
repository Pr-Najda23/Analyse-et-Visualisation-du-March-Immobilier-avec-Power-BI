🏠 Darkom.ma — Data Engineering & BI Pipeline

Pipeline décisionnel complet pour l’analyse du marché immobilier marocain à partir des annonces Darkom.ma.

📊 Aperçu du Projet

Ce projet consiste à construire une architecture BI complète permettant de transformer des données immobilières brutes en dashboards interactifs Power BI.

Architecture utilisée :

CSV Source
    ↓
Staging Layer
    ↓
Clean Layer
    ↓
Data Warehouse (Star Schema)
    ↓
Power BI Dashboards
🎯 Objectifs du Projet

Le projet permet de :

Construire un pipeline ETL industriel
Nettoyer et transformer les données immobilières
Concevoir un Data Warehouse optimisé
Créer des KPIs métiers avancés
Développer des dashboards interactifs Power BI
Analyser le marché immobilier marocain
🧱 Architecture du Projet
darkom_project/
│
├── data/
│   ├── raw/
│   ├── clean/
│
├── logs/
│
├── scripts/
│   ├── staging/
│   ├── cleaning/
│   ├── warehouse/
│
├── sql/
│
├── dashboards/
│
├── README.md
│
└── requirements.txt
🗄️ Technologies Utilisées
Technologie	Rôle
Python	ETL & Data Cleaning
PostgreSQL	Data Warehouse
SQLAlchemy	Connexion DB
Pandas	Manipulation des données
Power BI	Visualisation
Power Query	Préparation BI
DAX	Mesures avancées
📥 Source des Données

Fichier source :

darkom_annonces.csv
Colonnes disponibles
Colonne	Description
annonce_id	Identifiant unique
date_publication	Date de publication
titre	Titre annonce
ville	Ville
quartier	Quartier
type_bien	Appartement, Villa...
transaction	Vente / Location
prix	Prix en MAD
surface	Surface m²
nb_chambres	Nombre chambres
nb_salles_bain	Nombre salles de bain
etage	Numéro étage
annee_construction	Année construction
⚙️ Pipeline ETL
1️⃣ Staging Layer

Objectif :

Import brut du CSV
Vérification du chargement
Gestion des logs
Zone temporaire avant transformation

Actions réalisées :

✔ Import PostgreSQL
✔ Contrôle d’intégrité
✔ Logging ETL
✔ Validation des colonnes

🧹 2️⃣ Clean Layer
Nettoyage des données
Suppression des doublons
Gestion des valeurs manquantes
Correction des types
Standardisation des villes
Harmonisation des transactions
Traitement des valeurs aberrantes
Variables créées
Feature Engineering	Description
prix_m2	Prix par m²
age_bien	Âge estimé
categorie_prix	Économique / Luxe
categorie_surface	Petit / Moyen / Grand
annee_publication	Dimension temporelle
trimestre_publication	Analyse saisonnière
🏛️ 3️⃣ Data Warehouse

Le Data Warehouse est construit dans :

bi_schema
Modèle utilisé

⭐ Star Schema

Tables de dimensions
dim_date
dim_localisation
dim_bien
dim_transaction
Table de faits
fact_annonces
🔗 Relations du Modèle
dim_date --------|
                  |
dim_localisation -|---- fact_annonces
                  |
dim_bien ---------|
                  |
dim_transaction --|
📈 KPIs Développés
KPI	Description
Nombre total d'annonces	Volume global
Prix moyen	Prix moyen marché
Prix moyen par m²	Valeur immobilière
Surface moyenne	Taille moyenne
Croissance annonces	Évolution temporelle
Répartition des biens	Analyse catégories
📊 Dashboards Power BI
🌍 Dashboard 1 — Vue Globale
Nombre total d'annonces
Prix moyen marché
Surface moyenne
Répartition par ville
KPIs interactifs
Répartition Vente vs Location
💰 Dashboard 2 — Analyse des Prix
Distribution des prix
Prix moyen par m²
Segments immobiliers
Analyse par catégorie
Comparaison des types de biens
📍 Dashboard 3 — Analyse Géographique
Carte géographique
Classement des villes
Top quartiers
Zones les plus chères
Répartition régionale
📉 Dashboard 4 — Analyse des Tendances
Évolution des prix
Volume des annonces
Analyse saisonnière
Comparaison N vs N-1
Tendances marché immobilier
🎛️ Filtres Dynamiques

Tous les dashboards contiennent des slicers interactifs :

Ville
Type de bien
Transaction
Surface
Prix
Période
🔍 Validation des Données

Contrôles effectués :

✔ Cohérence du warehouse
✔ Intégrité des relations
✔ Validation des types
✔ Contrôle qualité
✔ Vérification Power BI

📊 Résultat Final

Le projet produit :

✅ Pipeline ETL complet
✅ Data Warehouse optimisé
✅ Dashboards Power BI interactifs
✅ Analyse complète du marché immobilier marocain
