**Projet de Pipeline de Prétraitement et Modélisation – Campagne Marketing Bancaire**

---

📘 **Contexte**

Ce projet s’inscrit dans le cadre de l'Intelligence Artificielle appliquée au prétraitement des données et vise à développer un pipeline complet d’apprentissage automatique pour prédire si un client souscrira à un dépôt à terme suite à une campagne marketing.
Les données proviennent de la campagne d’une banque et sont accessibles via l’UCI Machine Learning Repository.

❓ **Problématique**

Pourquoi ce projet ?
Les campagnes marketing ciblées sont essentielles pour optimiser les coûts et maximiser les conversions. Cependant, le succès de ces campagnes dépend de la capacité à identifier les clients les plus susceptibles de répondre positivement.

Question centrale :
Comment construire un modèle prédictif fiable pour identifier les clients susceptibles de souscrire à un dépôt à terme, en s’appuyant sur un pipeline structuré de prétraitement, de sélection de caractéristiques et de modélisation ?

🔧 **Méthodologie**

Outils utilisés:

Langage : Python

Environnement : Jupyter Notebook

Bibliothèques principales : pandas, scikit-learn, matplotlib, seaborn

Données : bank-full.csv (entraînement) et bank.csv (test)

Étapes du pipeline:
- Prétraitement des données

- Nettoyage (valeurs manquantes, doublons)

- Encodage des variables catégorielles (One-Hot Encoding, Label Encoding)

- Normalisation/standardisation des variables numériques

- Gestion du déséquilibre des classes (si nécessaire)

- Sélection de caractéristiques

Méthodes étudiées :

- Analyse de corrélation

- Importance des caractéristiques via modèles tree-based (Random Forest)

- Sélection univariée (SelectKBest)

- Justification du choix final

- Modélisation et évaluation

- Choix du modèle : au moins un algorithme supervisé (ex. Random Forest, Logistic Regression, XGBoost)

- Entraînement sur bank-full.csv

- Évaluation sur bank.csv

Métriques utilisées : 

- Accuracy, Precision, Recall, F1-score

- Matrice de confusion

- Courbe ROC / AUC

📊 **Résultats**

Visualisations proposées

- Distribution de la variable cible (y) – histogramme

- Corrélations entre caractéristiques – heatmap

- Importance des caractéristiques – bar plot

- Performances du modèle – matrice de confusion + courbe ROC

Commentaires attendus:
- Interprétation des métriques de performance

- Analyse des caractéristiques les plus discriminantes

- Discussion des limites (ex. déséquilibre des classes, surapprentissage)

✅ **Conclusions et Recommandations**

Implications pour l’entreprise
Un modèle bien calibré permet de :

1- Réduire les coûts de campagne en ciblant les clients les plus réceptifs

2- Augmenter le taux de conversion et la satisfaction client

3- Affiner les stratégies marketing grâce à l’analyse des caractéristiques influentes

Recommandations d’action:

1- Mettre en production le modèle dans un environnement de test avec suivi continu des performances.

2- Intégrer de nouvelles données comportementales (ex. historique des transactions) pour améliorer la prédiction.

3- Automatiser le pipeline de prétraitement pour des mises à jour régulières.

4- Former les équipes marketing à l’utilisation des résultats du modèle pour des campagnes plus personnalisées.

***Ce projet a été réalisé sous la direction du Professeur Nadjate Saïdani.***
