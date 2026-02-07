**Projet :** 

Prédiction de Souscription à un Dépôt Bancaire (Classification avec Random Forest)

**Description :** 

Ce projet utilise l'apprentissage automatique pour prédire si un client souscrira à un dépôt à terme après une campagne marketing téléphonique, en se basant sur des données démographiques et comportementales.

🎯 **Objectif / Contexte**

Problème à résoudre :

Les banques effectuent régulièrement des campagnes marketing pour proposer des produits financiers (comme des dépôts à terme). Ces campagnes ont un coût, et contacter tous les clients est inefficace.
L'objectif est de construire un modèle prédictif qui identifie les clients les plus susceptibles de souscrire, afin d'optimiser les efforts marketing et d'améliorer le taux de conversion.

Pourquoi c'est intéressant :

- Réduction des coûts marketing

- Amélioration de l'expérience client (moins de sollicitations inutiles)

- Cas pratique typique de classification binaire en machine learning

📊 **Données**

Source : UCI Machine Learning Repository - Bank Marketing Dataset

Taille :

bank-full.csv : 45 211 lignes (entraînement)

bank.csv : 4 521 lignes (test)

Variables principales (17 colonnes) :

Catégorie	Variables	Description

Démographiques	age, job, marital, education	Âge, profession, situation familiale, niveau d'étude
Financières	default, balance, housing, loan	Défaut de crédit, solde, prêt immobilier, prêt personnel
Campagne	contact, day, month, duration, campaign	Type de contact, jour/mois, durée d'appel, nombre de contacts
Historique	pdays, previous, poutcome	Jours depuis dernier contact, contacts précédents, résultat passé
Cible	y	Souscription au dépôt (yes/no)

🛠️ **Méthodologie / Analyse**

Le projet suit un pipeline structuré :

1. Prétraitement des données
Chargement et inspection des données (pandas, .info(), .describe())

Détection des valeurs manquantes et des valeurs aberrantes

Visualisation des distributions et outliers via boxplots

2. Ingénierie des features
Pipeline de traitement :

Variables numériques : imputation par la moyenne + standardisation (StandardScaler)

Variables catégorielles : encodage one-hot (OneHotEncoder)

Utilisation de ColumnTransformer pour appliquer différents traitements par type de variable

3. Modélisation
Modèle choisi : RandomForestClassifier (forêt aléatoire)

Pipeline complet : prétraitement + modèle

Métriques d'évaluation : accuracy_score, classification_report

4. Évaluation et interprétation
Prédictions sur le jeu de test

Analyse des performances et des features importantes

📈 **Résultats clés**

Insights principaux :
Variables influentes : La durée de l'appel (duration) et le résultat de la campagne précédente (poutcome) sont des prédicteurs forts.

Impact de l'historique : Les clients contactés récemment (pdays) et ayant déjà souscrit répondent mieux.

Profil type du souscripteur : Clients plus âgés, avec un solde élevé et sans prêt en cours.

Limite du modèle : La variable duration est très prédictive, mais n'est connue qu'après l'appel → à utiliser avec précaution pour de nouvelles campagnes.


🖥️ **Technologies utilisées**

Langage : Python 3

Bibliothèques principales :

pandas, numpy : manipulation des données

matplotlib, seaborn : visualisations

scikit-learn : préprocessing, modélisation, évaluation

jupyter : environnement interactif

Modèle : RandomForestClassifier (classification)

👨‍💻 **Auteur**

KOUDA KYLIAN
Étudiant en Data Science / Analyste Data

GitHub : 

LinkedIn : https://www.linkedin.com/feed/

Contact : kyliankk22@gmail.com


**Ce mini projet a été réalisé dans le cadre d'un apprentissage en machine learning et data analysis.**

