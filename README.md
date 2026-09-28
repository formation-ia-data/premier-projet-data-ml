# Ton premier projet Data & ML en Python

Code et données de la vidéo YouTube **« Ton premier projet Data & ML en Python — projet
complet 35 min (débutant, avec code) »**.

On y estime la consommation d'une voiture (en L/100 km) à partir de son poids, avec une
régression linéaire, de bout en bout : chargement, nettoyage, exploration, prétraitement,
modélisation et interprétation.

## Lancer le notebook : rien à installer

[![Ouvrir dans Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/formation-ia-data/premier-projet-data-ml/blob/main/premier_projet_data_ml.ipynb)

Cliquez sur le bouton : le notebook s'ouvre dans **Google Colab**, directement dans le
navigateur. Il suffit d'un compte Google. Ni Python ni Anaconda à installer.

Exécutez ensuite les cellules une à une, de haut en bas (`Maj + Entrée`).

## Contenu

| Fichier | Rôle |
|---|---|
| `premier_projet_data_ml.ipynb` | Le notebook de la vidéo |
| `data/mpg.csv` | Le jeu de données : 398 voitures, 9 colonnes |

Le notebook lit le CSV depuis le tag **`v1`** de ce dépôt. Le fichier servi reste donc
identique à celui de la vidéo, même si le dépôt évolue.

## ⚠️ Limites du modèle

Les données portent sur des voitures commercialisées **entre 1970 et 1982**, pesant de
732 à 2 331 kg. Le modèle décrit une **association** dans cet échantillon ancien. Il ne
dit rien des voitures d'aujourd'hui, et il ne prouve pas que le poids soit la seule cause
de la consommation.

## Données et licence

**Données :** *Auto MPG*, UCI Machine Learning Repository —
Quinlan, R. (1993). Auto MPG [Dataset]. <https://doi.org/10.24432/C5859H>

**Licence des données :** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

**Modifications :** le fichier `data/mpg.csv` est la copie redistribuée par le dépôt
d'exemples de seaborn (<https://github.com/mwaskom/seaborn-data>), sans modification.
Le notebook y ajoute deux colonnes métriques : `conso_l_100km` (`235,214583 / mpg`) et
`poids_kg` (`weight × 0,45359237`). Aucune ligne n'est supprimée.
