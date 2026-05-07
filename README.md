Contexte du Projet
L'entreprise pharmaceutique HumanForYou, basée en Inde, fait face à un taux de rotation (turnover) de 15%. Ce phénomène engendre des retards sur les projets, des coûts de recrutement élevés et une perte de savoir-faire critique.

Objectif : Identifier les facteurs d'influence de l'attrition et proposer un modèle de Machine Learning capable de prédire les départs pour permettre à la direction RH de mettre en place des actions de rétention ciblées.

 Données Utilisées
L'analyse repose sur la fusion de quatre sources de données (fichiers CSV) anonymisées par EmployeeID :

Données RH (general_data.csv) : Informations démographiques, salaires, ancienneté et formation.

Évaluation Manager (manager_survey_data.csv) : Implication et performance perçues par la hiérarchie.

Enquête Salariés (employee_survey_data.csv) : Satisfaction environnementale, satisfaction au travail et équilibre vie pro/vie perso.

Horaires de travail (in_out_time.csv) : Données de badgeuses permettant de calculer le temps de travail effectif moyen et les heures supplémentaires.

 Stack Technique
Langage : Python 3.13.7

Librairies Data : Pandas (manipulation), NumPy (calcul)

Visualisation : Matplotlib, Seaborn

Machine Learning : Scikit-Learn (Prétraitement, Modélisation, Évaluation)

 Méthodologie & Pipeline
Data Cleaning & Feature Engineering :

Gestion des valeurs manquantes (imputation des notes d'enquêtes).

Calcul de la durée moyenne de travail journalière à partir des badgeuses.

Encodage des variables catégorielles (LabelEncoding / One-Hot Encoding).

Analyse Exploratoire (EDA) :

Mise en évidence des corrélations (ex: lien entre le salaire et le départ).

Analyse de la distribution de l'âge et de la distance domicile-travail.

Modélisation :

Entraînement de plusieurs modèles : Régression Logistique, Random Forest, et Decision Tree.

Gestion de l'imbalance des classes (l'attrition ne concerne que 15% du dataset).

Évaluation : Utilisation de la Matrice de Confusion, du F1-Score et de la courbe ROC-AUC.

 Résultats Clés 
Facteurs Majeurs :  la charge de travail, à la satisfaction et à l’ancienneté  des variables pivots.

Performance : le Random Forest optimisé apparaît comme le meilleur modèle pour prédire l’attrition dans ce contexte.
