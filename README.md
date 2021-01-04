# test-technique-datascience

Il s'agit du test technique la data science chez Folhomee. Il est conçu pour tester vos compétences en conception d'API, en scraping Web, en architecture cloud et en apprentissage automatique en général.

Nous allons chercher à analyser les données fournies par velib

## Livrables

Les livrables minimum sont les suivants :

- Un repo github privé auquel vous aurez donné accès au CTO de Folhomee (username github : milanito)
- Un ensemble de dossiers/fichiers selon une nomenclature claires

Pour le reste, vous êtes libre de vos choix technique (base de donnée, etc ...) quand il n'est pas explicitement dit dans l'exercice le choix à faire. Soyez prêt à expliquer votre code et pourquoi vous avez pris certaines des décisions que vous avez prises.

## Récupération des flux

La liste des flux est disponible ici :

- https://velib-metropole-opendata.smoove.pro/opendata/Velib_Metropole/gbfs.json

Les deux qui nous intéressent sont ceux sur les informations des stations et sur le status de ces dernières :

- https://velib-metropole-opendata.smoove.pro/opendata/Velib_Metropole/station_information.json
- https://velib-metropole-opendata.smoove.pro/opendata/Velib_Metropole/station_status.json

## Exercice

### Récupération des données

Concevez un système pour :
- Lire les données de tous les flux (en temps réel ?)
- Stocker dans une base de données

Il vous sera demandé une description de la conception qui doit inclure :

- La stack technologique
- La méthode de collecte et de traitement des données
- L'infrastructure cloud utilisée (si c'est le cas)

Les composants à développer sont le scraping et le stockage Web, ainsi qu'un point de terminaison / hotspots d'API qui accepte les paramètres

> Soyez simple sur la réalisation, le but n'est pas de prendre trop de temps mais de comprendre votre manière de faire

### Détermination des points chauds

Déterminez les points chauds : les stations les plus encombrées de vélos

> indice: vous devez diviser la carte en hexagones égaux de 75 mètres pour regrouper les coordonnées

## API de lecture

Ecrivez une API (simple) pour pouvoir récupérer les données qui comprend une route qui accepte comme parametre une date

Un exemple de réponse pour ce point final pourrait être une liste de centres hexagonaux (lat / long) et leur poids (par rapport aux autres) en termes de degré d'encombrement pour le jour donné.

> Soyez simple sur cette partie
