---
title: ""
---

# Travaux Pratiques — Télédétection & Classification d'occupation du sol UGB/LSH/GEO/L3 {.unnumbered .unlisted}

<div align="center">

<img src="images/me.jpg" alt="Photo de profil" width="150"
  style="border-radius: 50%; border: 3px solid #2e86c1; margin-bottom: 1rem;" />

# S. Bassirou DIOP, PhD

**Hydrologie | Machine Learning**

[![ORCID](https://img.shields.io/badge/ORCID-0000--0000--0000--0000-brightgreen?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0000-0000-0000-0000)
[![Email](https://img.shields.io/badge/Email-prenom.nom%40univ.fr-blue?style=flat-square&logo=gmail)](mailto:09.bachir.diop.10@gmail.com)

</div>

---

## Présentation du TP

Ce travail pratique s'inscrit dans le cadre de la **télédétection spatiale appliquée**. Il mobilise des images satellites multibandes pour produire une **carte d'occupation du sol** à partir d'une classification supervisée.

Les données traitées proviennent du capteur **Landsat** (USGS), largement utilisé en sciences de la Terre pour sa couverture temporelle étendue et sa résolution adaptée aux analyses régionales.

---

## Objectifs pédagogiques

À l'issue de ce TP, vous serez en mesure de :

### Comprendre la télédétection
- Maîtriser les fondements physiques de l'acquisition satellite (rayonnement électromagnétique, réponse spectrale des surfaces)
- Distinguer les différentes résolutions : spatiale, spectrale, temporelle, radiométrique
- Identifier les domaines d'application de la télédétection (agriculture, forêt, urbanisme, littoral…)

### Manipuler des images satellites
- Charger et visualiser des images multibandes Landsat
- Réaliser des compositions colorées (RGB naturel, fausses couleurs, infrarouge)
- Calculer des indices spectraux (**NDVI**, **NDWI**, **NDBI**…)

### Réaliser une classification supervisée
- Créer des zones d'entraînement (*training samples*) représentatives
- Appliquer un algorithme de classification (Maximum de vraisemblance, Random Forest…)
- Valider les résultats via une **matrice de confusion** et le **coefficient Kappa**

### Produire une carte d'occupation du sol
- Mettre en page et habiller une carte thématique
- Définir une légende claire et des classes cohérentes
- Exporter le résultat dans un format SIG standard (GeoTIFF, Shapefile)

---

# Zone d'étude

Avant de commencer le TP, téléchargez le GeoPackage contenant la zone d'étude. La région d'étude correspond à une large couverture autour de la ville de Saint-Louis.

<div align="center">

[![Télécharger le GeoPackage](https://img.shields.io/badge/⬇️%20Télécharger-GeoPackage%20(.gpkg)-0078D4?style=for-the-badge&logo=nextcloud&logoColor=white)](https://emma.nl.tabdigital.cloud/s/ksDWbLK9gLrAdz2)

</div>

---

# Outils & environnement

- **QGIS** ou **ArcGIS Pro** — traitement et visualisation des données raster/vecteur
- **Python** (`rasterio`, `scikit-learn`, `numpy`, `matplotlib`) — scripts de traitement automatisé
- **Google Earth Engine** *(optionnel)* — accès et pré-traitement cloud des images Landsat

---

