## 🌺 Dataset - Flowers Recognition 🌺
## Table des Matières

- [Description du Projet et ressources](#description-du-projet-et-ressources)
- [Technologies Utilisées](#technologies-utilisées)
- [Étapes du Projet](#étapes-principales-du-projet)
  - [Partie 1 : Extraction et exploration des données](#partie-1--extraction-et-exploration-des-données)
  - [Partie 2 : Prétraitement des images](#partie-2--prétraitement-des-images)
  - [Partie 3 : Construction modèle CNN](#partie-3--Construction-modèle-CNN)
  - [Partie 3 : Optimisation paramètres et évaluation](#partie-3--Optimisation-paramètres-et-évaluation)
- [Auteur](#auteur)

## Description du Projet et ressources

Ce dataset contient environ 4 300 images de fleurs réparties en cinq classes : chamomile, tulip, rose, sunflower, dandelion. Les images ont été collectées à partir de Flickr, Google Images et Yandex Images, chaque classe comprend environ 800 photos en couleur, avec une résolution moyenne de 320×240 pixels. Les images ne sont pas redimensionnées à une taille unique et présentent des proportions variables. Ce projet a pour objectif le traitement et l’optimisation d’images en vue de construire deux modèles de classification par réseau de neurones convolutifs (CNN) : un modèle simple et un modèle optimisé.📷

📌 Télécharger via Kaggle ou API ((https://www.kaggle.com/datasets/alxmamaev/flowers-recognition) 📌

📥 Telecharger le Dataset via Google Drive (https://drive.google.com/drive/folders/1J8oiO7iYouf9KdJ5Ja1Qjs9t7CwvUG_f) 📥

## Technologies Utilisées : 

- Python dans un environnement Google Collab,
- OpenCV,
- Pandas, NumPy, Matplotlib,
- TensorFlow, Keras,
- Scikit-image, ImageDataGenerator, Scikit-learn,

## 🕜 Etapes principales du projet 🕜

📂 ### Partie 1 : Extraction et exploration des données 📂

- Chargement des données réparties en 5 dossiers étiquettés (Roses, Tulip, Sunflower..).
  
- Décompte du nombre d'images pour voir la répartition par catégories.

🖼️ ### Partie 2 : Prétraitement des images 🖼️

- Redimensionnement de toutes les images pour les uniformiser en 128*128

- Conversion des images en tableaux numériques pour le traitement

- Normalisation des pixels dans la plage [0,1] et encodage des étiquettes

🤖  ### Partie 3 : Construction modèle CNN 🤖

- Modèle 'Sequential' en Keras avec 3 couches de Conv2D + MaxPooling2D + 1 couche Flatten +  1 couche Dense avec 128 neuronnes +  Dropout de 50% + couche de sortie 'Dense' avec Softmax 5 classes, compilation avec optimiseur 'Adam un learning rate = 0.001, perte 'sparse_categorical_crossentropy' et accuracy comme mètrique, entraînement sur 12 epochs batch_size = 32

- Evaluation de la performance avec une courbe de précision et une courbe de pertes. ** Accuracy 65% **

🚀 ### Partie 4 : Optimisation paramètres et évaluation 🚀

- Utilisation de 'DataImageGenerator' pour augmenter artificiellement le jeu d'entrainement avec données variées

- Entrainement du deuxiemes modèles sur 10 epochs avec data augmentées. ** Accuracy 72% **

## Auteur 
Étudiant en Data Science
damien.lauger.edu@groupe-gema.com

