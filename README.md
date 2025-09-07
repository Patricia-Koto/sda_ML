-----

# Analyse et prédiction de la solvabilité des prêts

## Contexte

Les institutions financières font face au défi d'évaluer le risque de défaut de paiement des prêts. Ce projet utilise les données historiques des demandeurs de prêt pour créer un modèle d'apprentissage automatique capable de prédire les défauts de paiement, ce qui permet des décisions plus éclairées et une atténuation des risques.

## Objectifs du projet

  * **Créer un modèle prédictif :** Construire un modèle qui peut prévoir si un prêt sera en défaut en se basant sur les informations fournies par le demandeur.
  * **Identifier les facteurs clés :** Déterminer les variables les plus influentes qui contribuent au risque de défaut de paiement.
  * **Formuler des recommandations :** Proposer des stratégies pour réduire les risques de défaut.

## Technologies et bibliothèques

Le projet est développé en Python et utilise plusieurs bibliothèques de science des données et d'apprentissage automatique.

  * `pandas` et `numpy` pour la manipulation des données.
  * `matplotlib.pyplot` et `seaborn` pour la visualisation des données.
  * `scikit-learn` pour le prétraitement, la modélisation et l'évaluation du modèle.

## Structure du jeu de données

Le jeu de données `loan_default_data.csv` est utilisé, contenant 255 347 lignes et 18 colonnes. Il inclut des variables numériques et catégorielles telles que :

  * **Variables numériques :** `Age`, `Income`, `LoanAmount`, `CreditScore`, `MonthsEmployed`, `NumCreditLines`, `InterestRate`, `LoanTerm`, et `DTIRatio`.
  * **Variables catégorielles :** `Education`, `EmploymentType`, `MaritalStatus`, `HasMortgage`, `HasDependents`, `LoanPurpose`, et `HasCoSigner`.

## Étapes de l'analyse

1.  **Exploration des données :** Le notebook commence par une exploration détaillée des données, incluant des statistiques descriptives et une vérification des valeurs uniques pour chaque variable.
2.  **Visualisation des données :** Des graphiques en secteurs sont générés pour visualiser la distribution des variables catégorielles par rapport à la variable cible (`Default`).
3.  **Préparation des données :** Les données sont nettoyées et préparées pour la modélisation.
4.  **Modélisation :** Plusieurs modèles de classification sont testés à l'aide d'une validation croisée (K-Fold) pour prédire le défaut de paiement.
5.  **Évaluation et résultats :** Les performances des modèles sont évaluées en utilisant une métrique d'exactitude (accuracy).

-----

### Comment utiliser ce projet ?

1.  **Clonez le référentiel** sur votre machine locale.
2.  **Installez les dépendances :** Assurez-vous d'avoir Python et toutes les bibliothèques requises installées (utiliser le ficher "requirements.txt").
3.  **Exécutez le notebook :** Ouvrez le fichier `loan_credit.ipynb` dans un environnement Jupyter (comme Jupyter Notebook ou JupyterLab) et exécutez les cellules une par une.
