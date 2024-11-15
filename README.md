# Prédiction du Prix des Maisons

## Contexte du Projet

Dans ce projet, nous simulons une étude d'analyse et de prédiction des prix de maisons dans une région donnée, basée sur divers critères tels que la superficie, le nombre de chambres, le type de quartier, le système de chauffage, et bien d'autres caractéristiques. L'objectif est de construire et d'évaluer un modèle prédictif pour estimer le prix des maisons en fonction de ces attributs.

### Objectifs
1. **Exploration et Analyse des Données (EDA)** : Analyser les données, traiter les valeurs manquantes, et visualiser les distributions des différentes caractéristiques.
2. **Modélisation avec Scikit-Learn** : Utiliser la bibliothèque Scikit-Learn pour entraîner un modèle de régression linéaire sur les données, explorer différents paramètres, et évaluer ses performances.
3. **Implémentation "from scratch"** : Recréer l'algorithme de régression linéaire en Python natif (sans utiliser de bibliothèques de machine learning) pour une compréhension approfondie des calculs et des étapes de l'algorithme.

## Structure du Projet

### Partie 1 : Analyse Graphique des Données (EDA)

Cette partie consiste à explorer les données et à effectuer les étapes suivantes :
- **Chargement des Données** : Chargement des données depuis un fichier CSV.
- **Analyse des Statistiques** : Visualisation des statistiques descriptives pour comprendre les distributions et les caractéristiques des données.
- **Traitement des Valeurs Manquantes** : Identification et traitement des valeurs manquantes pour s'assurer que le jeu de données est complet.
- **Visualisation des Distributions** : Histogrammes pour observer la forme des distributions de chaque variable et détecter les valeurs extrêmes (outliers).
- **Regroupement des Catégories** : Pour les catégories peu représentées, regroupement en une seule catégorie afin de simplifier le modèle.
- **Encodage des Variables Catégorielles** : Conversion des variables catégorielles en format numérique à l’aide du One-Hot Encoding.
- **Détection des Valeurs Extrêmes** : Utilisation de boîtes à moustaches pour détecter et gérer les valeurs extrêmes.
- **Matrice de Corrélation** : Création d’une heatmap pour visualiser les corrélations entre les variables numériques.

### Partie 2 : Modélisation avec Scikit-Learn

Dans cette section, nous construisons un modèle de **régression linéaire** pour prédire le prix des maisons en utilisant les données traitées.
- **Séparation des Données** : Les données sont divisées en ensembles d’entraînement et de test pour évaluer la performance du modèle.
- **Entraînement avec Scikit-Learn** : Un modèle de régression linéaire est entraîné avec Scikit-Learn, en explorant différents paramètres pour optimiser les performances.
- **Évaluation du Modèle** : Les performances du modèle sont évaluées en calculant les métriques MAE (Mean Absolute Error) et R² pour les ensembles d'entraînement et de test. Cela permet de détecter un éventuel sur-apprentissage (overfitting) ou sous-apprentissage (underfitting) et de vérifier la précision des prédictions.

### Partie 3 : Implémentation de la Régression Linéaire "from scratch"

Dans cette dernière partie, l'algorithme de régression linéaire est réimplémenté en Python de manière "from scratch", sans utiliser de bibliothèques de machine learning, pour mieux comprendre son fonctionnement.
- **Initialisation des Paramètres** : Les poids et le biais sont initialisés à zéro.
- **Descente de Gradient** : L'algorithme de descente de gradient est utilisé pour ajuster les paramètres du modèle et minimiser l'erreur entre les prédictions et les valeurs réelles.
- **Évaluation du Modèle** : Les performances de ce modèle "from scratch" sont comparées aux résultats obtenus avec Scikit-Learn pour vérifier la cohérence.

## Structure des Fichiers

- `prix_maisons.csv` : Fichier de données contenant les caractéristiques des maisons et leur prix cible.
- `EDA_Modelisation.ipynb` : Notebook contenant l’analyse graphique (EDA) et la modélisation avec Scikit-Learn.
- `From_Scratch.ipynb` : Notebook contenant l'implémentation "from scratch" de la régression linéaire en Python natif.
- `README.md` : Ce fichier expliquant le contexte, la structure et les étapes pour exécuter le projet.

## Instructions pour Exécuter le Projet

### Prérequis

Assurez-vous d'avoir installé les bibliothèques suivantes :
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Vous pouvez installer ces bibliothèques en exécutant :

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Étapes pour Exécuter

1. Exploration et Modélisation (Parties 1 et 2) : Ouvrez et exécutez le notebook `EDA_Modelisation.ipynb` pour effectuer l'analyse graphique et la modélisation avec Scikit-Learn.
2. Implémentation from Scratch (Partie 3) : Ouvrez et exécutez le notebook `From_Scratch.ipynb` pour l'implémentation manuelle de l'algorithme de régression linéaire.
3. Évaluation des Résultats : Comparez les performances des deux méthodes de modélisation pour observer les différences et analyser les résultats.

## Conclusion

Ce projet illustre les différentes étapes de la construction d'un modèle de machine learning, de la préparation des données jusqu'à l'implémentation de l'algorithme. L’approche "from scratch" offre une compréhension approfondie des mécanismes de la régression linéaire, tandis que l’utilisation de Scikit-Learn permet une modélisation rapide et performante. Ce projet est un bon point de départ pour explorer d’autres algorithmes et pour approfondir l’analyse prédictive dans le domaine de l’immobilier.
