# Projet-4: EDA & Régressions


## Description du Projet
Bienvenue dans notre projet de Machine Learning basé sur le concours de la ville de Seattle !    
L'objectif de ce projet est de créer un modèle prédictif de la consommation d'énergie et de CO2 des bâtiments publics.     
Le but est d'éviter de réaliser des relevés manuels annuellements en utilisant des modèles prédictifs fiables.    
Les données sont chargées depuis le site de la ville de Seattle : https://data.seattle.gov/dataset/2016-Building-Energy-Benchmarking/2bpz-gwpy

Le jeu de données provient de la ville de Seattle et comprend des informations sur la consommation d'énergie et les émissions de CO2 pour différents bâtiments publics.      
Nous allons diviser le projet en trois scripts distincts pour mieux organiser le flux de travail.

### Notebook 1 : 🛠 Nettoyage & analyses exploratoires des données
Dans le premier script, nous nous concentrerons sur la préparation des données en effectuant les opérations suivantes :

- Chargement des données à partir des fichiers CSV fournis par la ville de Seattle
- Gestion des valeurs nulles
- Analyses univariées
- Consommation d'énergie par type de bâtiment
- Consommation d'énergie par années d'anciennetés
- Consommation d'énergie par type de bâtiment (dispersion)
- Consommation d'énergie en fonction du lieu géographique
- Matrice des corrélations
- Création des DF pour le Machine Learning
- Label Encoder
- Jointure des différentes tables du jeu de données pour créer un ensemble de données cohérent
  
### Notebook 2 : Modélisation - Prédiction de la Consommation d'Énergie
Dans le deuxième script, nous nous concentrerons sur la prédiction de la consommation d'énergie en utilisant plusieurs modèles linéaires et non linéaires en concurrence. Nous effectuerons les étapes suivantes :

- Régression multiple pour créer un modèle linéaire initial
- Régression multiple sur des données centrées et réduites pour améliorer la performance du modèle
- Régression multiple sur des données transformées en log pour gérer les valeurs extrêmes
- Régression logistique pour gérer la classification des données
- Prédiction avec XGBoost pour utiliser un modèle non linéaire avec des hyperparamètres ajustables
    
Nous comparerons les performances et la complexité de chaque modèle pour choisir celui qui convient le mieux à la prédiction de la consommation d'énergie.

### Notebbok 3 : Modélisation - Prédiction des Émissions de CO2
Le troisième script est similaire au deuxième, mais cette fois-ci, nous nous concentrerons sur la prédiction des émissions de CO2 des bâtiments publics.    
Nous utiliserons les mêmes modèles linéaires et non linéaires pour cette tâche de prédiction.

### Prérequis
Nous utilisons un environnement contenant :

Python 3.x     
pandas     
numpy    
pyplotlib    
seaborn    
scikit-learn    
xgboost    

### Structure des Fichiers

├── Data       
│   ├── data1.csv     
│   ├── data2.csv      
├──Modele     
│   ├── Regression.py     
│   ├── EDA.py      
├──Notebooks     
│  ├── Notebook_1_data_preparation.ipynb     
│  ├── Notebook_2_energy_prediction.ipynb      
│  ├──Notebook_3_co2_prediction.ipynb      
├── Seattle_picture.png       
└── README.md     


Le dossier "data" contient les fichiers CSV du jeu de données de la ville de Seattle.      
Les trois scripts sont au format Jupyter Notebook, chacun se concentrant sur une partie spécifique du projet.      
Le fichier README.md est le présent document, fournissant une présentation détaillée du projet.      

### Conclusion
Ce projet de Machine Learning basé sur le concours de la ville de Seattle vise à créer des modèles prédictifs fiables pour la consommation d'énergie et les émissions de CO2 des bâtiments publics.    
En utilisant des modèles linéaires et non linéaires en concurrence, nous chercherons à identifier les meilleurs modèles pour chaque tâche de prédiction.     
La réussite de ce projet nous permettra d'éviter des relevés manuels annuels coûteux en utilisant des modèles prédictifs précis.      

Ce projet fait partie de la formation Data-Scientist de Openclassrooms & Central'Supelec (certificat bac+5).







