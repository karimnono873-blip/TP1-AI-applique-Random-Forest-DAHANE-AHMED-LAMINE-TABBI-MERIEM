# TP N°1 : Classification de Clients avec Random Forest 🌲🛍️

**Auteur :** Dahane Ahmed Lamine  
**Enseignante :** Mme. Fergani  
**Module :** Machine Learning / Data Science  

## 🎯 Objectif du Projet

[cite_start]Ce projet a pour but de classer automatiquement des clients afin d'adapter une stratégie marketing[cite: 208]. [cite_start]Il s'agit d'un problème de classification supervisée utilisant l'algorithme d'Ensemble Learning **Random Forest**[cite: 209]. 

Le rapport principal du projet est fourni sous la forme d'une application web monolithique (un seul fichier HTML interactif avec un thème "Galaxie/Cyberpunk") pour une visualisation claire et professionnelle des concepts et du code.

## 📊 À propos du Dataset

[cite_start]Le jeu de données utilisé est le **Mall Customers Dataset**[cite: 210]. 
* [cite_start]**Description :** C'est un jeu de données synthétique couramment utilisé pour l'apprentissage et la démonstration des techniques de segmentation de la clientèle[cite: 3]. [cite_start]Il contient des informations démographiques et comportementales sur des visiteurs de centre commercial[cite: 4].
* [cite_start]**Taille :** 200 enregistrements, 5 variables[cite: 6].
* [cite_start]**Champs principaux :** `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`[cite: 8].
* [cite_start]**Origine :** Répertorié sur Kaggle et d'autres dépôts open data[cite: 9, 211].

[cite_start]Étant donné que la base de données n'est initialement pas labellisée pour un apprentissage supervisé [cite: 213][cite_start], nous avons créé nos propres labels en catégorisant les consommateurs en 3 classes selon leurs revenus annuels (Faible, Moyen, Élevé)[cite: 214].

## 🧠 Concepts Abordés

* [cite_start]**Random Forest :** Combinaison de plusieurs arbres de décision construits sur des échantillons aléatoires (Bagging) pour obtenir un modèle plus robuste et réduire la variance[cite: 21, 24, 113, 114].
* **Déséquilibre des classes :** Utilisation de la technique **SMOTE** (Synthetic Minority Over-sampling Technique) pour équilibrer la répartition des étiquettes de revenus.
* **Évaluation des performances :** Analyse via la matrice de confusion et le rapport de classification (Précision, Rappel, F1-Score).

## 🛠️ Technologies et Prérequis

Pour exécuter le script d'entraînement localement, vous aurez besoin de Python 3.x et des bibliothèques suivantes :

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
