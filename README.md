# Traitement d'image — Détection de contours par filtre de Sobel

Projet académique réalisé à l'INSA Rouen Normandie pendant mon cycle préparatoire (STPI).

## Description

Ce projet porte sur la détection de contours dans des images à l'aide du filtre de Sobel.

L'algorithme est implémenté en Python et réalise notamment :

* la conversion des images en niveaux de gris ;
* le calcul des gradients horizontal et vertical à l'aide des kernels de Sobel ;
* le calcul de la magnitude du gradient ;
* une étape de suppression des non-maxima afin d'affiner les contours ;
* la génération et la sauvegarde des images obtenues ;
* la mesure des performances de traitement.

Le projet comprend également une analyse des résultats et des performances présentée dans le rapport.

## Technologies

* Python
* NumPy
* Pillow
* Traitement d'image

## Structure du projet

```text
contour-main/
├── output/          # Images générées par les traitements
├── ...              # Code source
├── rapport.pdf      # Rapport du projet
├── requirements.txt
└── README.md
```

## Installation

Installer les dépendances avec :

```bash
pip install -r requirements.txt
```

## Traitement de Sobel

Le fichier `sobel.py` implémente le traitement principal.

Les gradients sont calculés à partir des deux kernels de Sobel :

```text
[-1  0  1]       [-1 -2 -1]
[-2  0  2]       [ 0  0  0]
[-1  0  1]       [ 1  2  1]
```

Les gradients horizontal et vertical sont ensuite combinés afin d'obtenir la magnitude du gradient et ainsi mettre en évidence les contours présents dans l'image.

## Résultats

Les images obtenues lors des différents traitements sont disponibles dans le dossier `output/`.

Le rapport présente en détail la méthode utilisée, les résultats obtenus ainsi que l'analyse des performances.

## Auteurs

Hugo BARROIS
Maissa BEN SETHOUM
Morgan GOOUZOU-HELLOT
Clément LEFEVRE
Maxime MORVANNOU
