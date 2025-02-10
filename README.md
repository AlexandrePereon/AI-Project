# Projet IA - Prédiction du Turnover des Employés

## Description
L'entreprise pharmaceutique *HumanForYou*, basée en Inde, emploie environ 4000 personnes et connaît un taux de rotation des employés d'environ 15 % par an. Ce turnover engendre des retards dans les projets, des coûts RH élevés et une perte de productivité. L'objectif de ce projet est d'analyser les facteurs influençant ce turnover et de proposer des modèles prédictifs pour aider l'entreprise à améliorer la rétention de ses employés.

## Données utilisées
Les données fournies par le service RH comprennent :
- Informations générales sur les employés (`general_data.csv`)
- Évaluations des managers (`manager_survey_data.csv`)
- Enquêtes sur la qualité de vie au travail (`employee_survey_data.csv`)
- Horaires de travail (`in_out_time.zip`)

Ces données ont été anonymisées et traitées pour garantir la confidentialité.

## Contenu du Repository
- **AI_Project_Data/** : Contient les fichiers de données.
- **project.ipynb** : Notebook Jupyter incluant l'analyse exploratoire, la modélisation et l'évaluation des modèles.
- **requirements.txt** : Liste des dépendances Python nécessaires.
- **.gitignore** : Fichier définissant les exclusions Git.
- **README.md** : Ce fichier.

## Installation
### Prérequis
- Python 3.10+
- Jupyter Notebook
- Installation des dépendances :
  ```bash
  pip install -r requirements.txt
  ```

### Lancement
1. Clonez le repository :
   ```bash
   git clone https://github.com/AlexandrePereon/AI-Project.git
   ```
2. Accédez au dossier :
   ```bash
   cd AI-Project
   ```
3. Lancez Jupyter Notebook :
   ```bash
   jupyter notebook
   ```
4. Ouvrez le fichier `project.ipynb` pour exécuter l'analyse.

## Déroulement du Projet
### 1. Exploration des Données (EDA)
- Nettoyage et traitement des valeurs manquantes
- Analyse descriptive et visualisation des données
- Identification des corrélations et des facteurs influents

### 2. Modélisation
- Préparation des données (encodage des variables catégorielles, standardisation)
- Test de plusieurs modèles :
  - Régression Logistique
  - SVM (Support Vector Machine)
  - Arbre de Décision
  - Random Forest
- Évaluation avec validation croisée et métriques de performance (Accuracy, F1-score, AUC-ROC)

### 3. Optimisation et Interprétation
- Recherche des meilleurs hyperparamètres avec GridSearchCV
- Analyse des résultats et interprétation des facteurs déterminants
- Recommandations pour améliorer la rétention des employés

## Résultats
- Le modèle **Random Forest** s'est avéré le plus performant avec une AUC-ROC de **0.99**.
- Les principaux facteurs influençant le turnover sont :
  - L'âge des employés
  - La distance entre domicile et lieu de travail
  - Le nombre d'entreprises précédemment travaillées
- Propositions pour l'entreprise :
  - Offrir des formations et perspectives de carrière
  - Améliorer les conditions de travail et l'équilibre vie pro/perso
  - Adapter les politiques RH pour fidéliser les talents

## Livrables
- **Document d'éthique** : Justification des choix réalisés en accord avec les principes éthiques de l'IA.
- **Bibliographie** : Liste des sources académiques et techniques utilisées.
- **Présentation finale** : Résumé des analyses et recommandations.

