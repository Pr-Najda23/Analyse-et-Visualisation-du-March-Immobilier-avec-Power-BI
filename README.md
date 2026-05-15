# 🏠 Avito Maroc — Analyse du Marché Immobilier

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Terminé-brightgreen?style=for-the-badge)
![Langue](https://img.shields.io/badge/Langue-Français-blue?style=for-the-badge)

> Tableau de bord Power BI interactif pour l'analyse et la visualisation du marché immobilier marocain à partir des annonces Avito.

---

## 📊 Aperçu du Projet

Ce projet propose une analyse complète des annonces immobilières publiées sur **Avito Maroc**, structurée en **3 pages interactives** dans un fichier Power BI (`.pbix`).

### KPIs Principaux
| Indicateur | Valeur |
|---|---|
| Nombre total d'annonces | **306** |
| Prix moyen | **1,50 MDH** |
| Prix moyen par m² | **49,05 KDH** |

---

## 📁 Structure du Rapport

### 1. 🌍 Vue Globale
Vue d'ensemble du marché avec :
- Nombre total d'annonces par ville (histogramme)
- Répartition des annonces par ville (graphique en anneau)
- Nombre d'annonces et prix moyen par segment (moyen / luxe / économique)
- Carte géographique — Prix moyen par ville

### 2. 💰 Analyse des Prix
Analyse approfondie des prix avec :
- Treemap — Prix moyen par m² par ville
- Histogramme de distribution des prix (compartiments)
- Comparaison annonces & prix moyen par segment

### 3. 📍 Analyse Géographique
Focus territorial avec :
- Carte interactive — Prix moyen par ville
- Graphique en anneau — Répartition des annonces par ville
- Tableau détaillé — Prix moyen par m² pour chaque ville

---

## 🎛️ Filtres Disponibles

Le rapport propose des filtres dynamiques applicables sur toutes les pages :

- **Ville** (`city`) — sélection multiple
- **Segment** — `économique` / `luxe` / `moyen`
- **Prix** — curseur de plage (115 000 DH → 60 000 000 DH)
- **Surface** (`surface_m2`) — curseur de plage (1 m² → 270 m²)

---

## 🗺️ Villes Couvertes

Le dataset inclut des annonces pour les principales villes marocaines, notamment :

`Kénitra` · `Casablanca` · `Essaouira` · `Agadir` · `Tanger` · `Dakhla` · `Ouislane` · `Marrakech` · `Fès` · `Meknès` · `Oujda` · `Rabat` · `Salé` · `Béni Mellal` · `Temara` · et bien d'autres.

---

## 🚀 Prise en Main

### Prérequis
- [Microsoft Power BI Desktop](https://powerbi.microsoft.com/fr-fr/desktop/) (gratuit)

### Ouverture du fichier
```bash
# Cloner le dépôt
git clone https://github.com/<votre-username>/avito-maroc-powerbi.git

# Naviguer dans le dossier Power BI
cd avito-maroc-powerbi/Power\ bi/
# Double-cliquer sur avito.pbix ou l'ouvrir via Power BI Desktop
```

### Navigation dans le rapport
1. Ouvrir `avito.pbix` dans Power BI Desktop
2. Utiliser les onglets en bas : **Vue Globale** → **Analyse des prix** → **Analyse Géographique**
3. Appliquer les filtres dans le panneau gauche pour affiner l'analyse

---

## 📂 Fichiers du Projet

```
ANALYSE ET VISUALISATION D.../
│
├── 📁 Dashboard screenshoots/
│   ├── 🖼️ Dashboard_1.png       # Vue Globale
│   ├── 🖼️ Dashboard_2.png       # Analyse des Prix
│   └── 🖼️ dashboard_3.png       # Analyse Géographique
│
├── 📁 Power bi/
│   └── 📊 avito.pbix            # Fichier Power BI principal
│
└── 📄 README.md                 # Documentation du projet
```

---

## 💡 Insights Clés

- **Kénitra** domine avec **23,53%** des annonces totales
- **Tanger** et **Agadir** affichent les prix au m² les plus élevés
- Le segment **luxe** présente le prix moyen le plus haut, mais le **segment moyen** concentre la majorité des annonces
- **Essaouira** se distingue avec un prix moyen par m² de **87 395,81 DH**
- **Agadir** enregistre le prix moyen par m² le plus élevé : **129 778,80 DH**

---

## 🛠️ Technologies Utilisées

- **Power BI Desktop** — Modélisation des données & visualisations
- **DAX** — Mesures et calculs (prix moyen, KPIs)
- **Bing Maps** — Cartes géographiques intégrées
- **Source des données** — Annonces immobilières Avito Maroc

---

## 👤 Auteur

Projet réalisé dans le cadre d'une analyse du marché immobilier marocain.

---

## 📄 Licence

Ce projet est à usage personnel et éducatif.