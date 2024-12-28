
API d'apprentissage automatique avec Flask et CNTK

Description

Ce projet met en œuvre une API d'apprentissage automatique basée sur Flask et CNTK (Microsoft Cognitive Toolkit). Il permet de déployer et de consommer des modèles de machine learning dans le cloud avec une interface 

simplifiée.


Structure du projet

templates/ : Contient les fichiers HTML pour l'interface web Flask.

Intro_to_Cloud_ML_with_Flask_and_CNTK.ipynb : Notebook Jupyter expliquant l'intégration de CNTK et Flask.

cntk_api.py : Fichier principal définissant l'API Flask pour l'utilisation des modèles.

config.py : Configuration des paramètres de l'application et des chemins.

conda.yaml : Fichier YAML pour configurer l'environnement Conda.

neko.jpg : Exemple d'image pour la démonstration du modèle.

synsets.txt : Fichier contenant les classes cibles pour la classification.

README.md : Ce fichier, détaillant le projet.

Fonctionnalités clés

Déploiement d’un modèle d’apprentissage automatique avec Flask.

Utilisation de CNTK pour l’entraînement et l’inférence des modèles.

API REST pour consommer les modèles via des requêtes HTTP.

Visualisation des résultats à l’aide de l’interface web Flask.

Prise en charge de la classification d’images avec un modèle pré-entraîné.

Installation


Clonez ce dépôt :



bash

Copier le code

git clone https://github.com/ton_profil/API-d-apprentissage-automatique.git

cd API-d-apprentissage-automatique

Configurez l’environnement Conda :



bash

Copier le code

conda env create -f conda.yaml

conda activate cntk_env

Lancez l’application Flask :



bash

Copier le code

python cntk_api.py

Accédez à l'interface utilisateur via :


http://127.0.0.1:5000 dans votre navigateur.

Utilisation

Chargez une image via l'interface web pour obtenir des prédictions du modèle.

Envoyez une requête POST à l'API pour une classification programmatique.

Exemple de requête POST :


bash

Copier le code

curl -X POST -F "file=@neko.jpg" http://127.0.0.1:5000/predict

Technologies utilisées

Frameworks : Flask, CNTK.

Langage : Python.

Outils : Jupyter Notebook, Conda.

Auteur
SALAH BEY ABDELDJALIL
