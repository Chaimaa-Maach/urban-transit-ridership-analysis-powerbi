# 🚆 Urban Transit Analysis – Chicago vs Philadelphia

<img width="1024" height="1024" alt="Gemini_Generated_Image_2y29wq2y29wq2y29" src="https://github.com/user-attachments/assets/bf5a22fa-8a98-4272-959f-64186fe40f8b" />


## 📌 Présentation du projet
Ce projet vise à analyser et comparer la **mobilité urbaine** dans deux grandes villes américaines — **Chicago** et **Philadelphie** — à partir des **données de fréquentation des transports publics**.

L’analyse est réalisée selon deux axes principaux :
- 📍 **Par lignes (routes)**
- 🚍 **Par modes de transport (Bus & Rail)**

L’objectif est de mettre en évidence les **tendances temporelles**, les **différences structurelles** entre les villes et les **comportements de fréquentation**, afin de fournir des indicateurs utiles à la prise de décision en matière de mobilité urbaine.

---

## 🎯 Objectifs
- Comparer la fréquentation des transports urbains entre Chicago et Philadelphie  
- Identifier les lignes et modes de transport les plus utilisés  
- Analyser l’évolution mensuelle et annuelle de la fréquentation  
- Mettre en évidence les impacts conjoncturels (ex. : période post-2019)  
- Construire un **dashboard Power BI interactif** basé sur une **modélisation en étoile**

---

## 🗂️ Sources de données
Les données utilisées proviennent de jeux de données publics sur la fréquentation des transports urbains :
- Données de fréquentation **par ligne**
- Données de fréquentation **par mode de transport**
- Période couverte : **2019 à 2025**

Les données ont été nettoyées, harmonisées et agrégées avant intégration dans Power BI.

---

## 🧹 Préparation & Nettoyage des données
Les principales étapes de traitement incluent :
- Filtrage des données à partir de **2019** pour assurer la comparabilité
- Agrégation des données journalières en **données mensuelles**
- Harmonisation des noms de colonnes et des formats numériques
- Standardisation des modes de transport (Bus / Rail)
- Séparation claire entre données **brutes (raw)** et **données nettoyées (clean)**

---

## 🧱 Modélisation des données
Le modèle repose sur une **architecture en étoile (Star Schema)** optimisée pour l’analyse Power BI.

### Tables de faits
- **FACT_ROUTE** : fréquentation par ligne, ville et date  
- **FACT_MODE** : fréquentation par mode de transport, ville et date  

### Tables de dimensions
- **DIM_DATE** : année, mois, libellé temporel
- **DIM_CITY** : villes (Chicago, Philadelphie)
- **DIM_ROUTE** : lignes de transport
- **DIM_MODE** : modes de transport (Bus, Rail)

Cette modélisation permet :
- une navigation fluide entre dimensions
- des performances optimisées
- une grande flexibilité analytique

---

## 📊 Dashboards Power BI

### 1️⃣ Analyse par lignes (Routes)
- KPI : Total Rides, Moyenne mensuelle, Min / Max observés
- Top 10 des lignes les plus fréquentées
- Comparaison inter-villes
- Évolution mensuelle de la fréquentation

### 2️⃣ Analyse par modes de transport
- KPI : Total Ridership, Moyenne mensuelle, Nombre de modes actifs
- Comparaison Bus vs Rail par ville
- Évolution mensuelle par mode
- Analyse de la croissance Month-over-Month (MoM)

🎛️ Les dashboards sont entièrement **interactifs** grâce aux filtres par :
- Année
- Ville
- Mode de transport

---

## 🔍 Principaux enseignements
- Chicago affiche globalement une **fréquentation plus élevée** que Philadelphie
- Le **bus** est le mode de transport dominant dans les deux villes
- Le **rail** joue un rôle plus important à Chicago
- Des variations saisonnières et conjoncturelles sont clairement observables

---

## 🛠️ Outils & Technologies
- **Python** (préparation et nettoyage des données)
- **Power BI**
  - Power Query (M)
  - Modélisation en étoile
  - DAX (mesures analytiques)
- **Git & GitHub** (versioning et documentation)

---

## 👤 Auteur
**Chaimaa**  

