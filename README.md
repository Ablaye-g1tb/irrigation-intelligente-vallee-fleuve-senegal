# Irrigation Intelligente — Vallée du Fleuve Sénégal

> Système de recommandation des doses et fréquences d'irrigation basé sur le Machine Learning,
> combinant télédétection Sentinel-2 et données agro-climatiques NASA POWER.

## Contexte
Les cultures irriguées de la Vallée du Fleuve Sénégal font face à un stress hydrique
chronique (98% du temps selon l'analyse Sentinel-2). Ce projet développe un système
de recommandation d'irrigation basé sur le ML pour aider les agriculteurs à optimiser
leurs pratiques d'irrigation.

## Zone d'étude
4 stations : Saint-Louis, Dagana, Podor, Matam — Période : 2021–2023

## Méthodologie
- **ET0** : Méthode Penman-Monteith FAO-56 (NASA POWER)
- **Indices satellitaires** : NDVI, NDWI, SAVI (Sentinel-2 via Google Earth Engine)
- **Modèle** : XGBoost — accuracy 88%
- **Interprétabilité** : SHAP values + RFECV

## Structure du projet
- `notebooks/` — Collecte des données et modélisation ML
- `data/` — Base de données géospatiale (4 380 observations)
- `models/` — Modèles entraînés (.pkl)
- `figures/` — Visualisations scientifiques

## Stack technique
Python | Google Earth Engine | Sentinel-2 | NASA POWER | XGBoost | SHAP | Pandas

## Auteur
**DIENG Abdoulaye** — Master 2 Modélisation Statistique et Informatique, UCAD
