# test-technique-datascience

Il s'agit du test technique la data science chez Folhomee. Il consiste en 5 questions et un petit challenge. Pour chacune vous devez implémenter une solution en utilisant si besoin le langage de votre choix. Pour les questions plus ouvertes, merci d'y répondre dans un fichier markdown

Votre rendu consitera en un repo github **privé** auquel vous inviterez notre CTO [Matthieu Rondeau](https://github.com/milanito).

Une fois que vous aurez fini, vous devrez envoyer [un email](mailto:matthieu@folhomee.fr) à notre CTO en indiquant que vous avez fini et en donnant vos disponibilités pour le debrief.

Si vous avez des questions ou des remarques, vous pouvez évidemment envoyer un mail.

Bonne chance !

## Question #1

Comment expliquer un test A/B à un ingénieur qui n'a aucune formation en statistiques ?

## Question #2

Comment s'assurer que vous n'analysez pas quelque chose qui finit par ne plus avoir de sens ?

## Question #3

Comment suggérer à un franchisé où ouvrir un nouveau magasin ?

## Question #4

Vous appelez 2 Uber et 3 Chauffeur Privé. Si le temps que chacun d'eux met pour vous rejoindre est identique, quelle est la probabilité que tous les Chauffeur Privé arrivent en premier ? Quelle est la probabilité que tous les Uber arrivent en premier ?

## Question #5

Étant donné un tableau d'entiers, renvoyer les indices des deux nombres tels que leur somme atteigne une cible spécifique.

Vous pouvez supposer que chaque entrée a exactement une solution, et vous ne pouvez pas utiliser deux fois le même élément.

Exemple :

```
Étant donné nums = [2, 7, 11, 15], cible = 18,
nums[1] + nums[2] = 7 + 11 = 18, retour [1, 2].
```

## Challenge

Vous êtes libre d'utiliser internet et toute autre bibliothèque.

Fichier de données : [data/cruise_ship_info.csv](./data/cruise_ship_info.csv)

### Objectif

Construire un régresseur qui recommande la taille de "l'équipage" pour les acheteurs potentiels de navires. Veuillez suivre les étapes suivantes

- Lire le fichier et afficher les colonnes.
- Calculez les statistiques de base des données (nombre, moyenne, std, etc.), examinez les données et énoncez vos observations.
- Sélectionnez les colonnes qui seront probablement importantes pour prédire la taille de l'"équipage".
- Si vous avez supprimé des colonnes, expliquez pourquoi vous les avez supprimées.
- Utilisez un *one-hot encoding* pour les caractéristiques catégorielles.
- Créez des ensembles d'entraînement et de test (utilisez 60 % des données pour l'entraînement et le rappel pour le test).
- Construisez un modèle d'apprentissage automatique pour prédire la taille de l'" équipage ".
- Calculez le coefficient de corrélation de Pearson pour l'ensemble de formation et les ensembles de données de test.
- Décrivez les hyperparamètres de votre modèle et comment vous les modifieriez pour améliorer les performances du modèle.
- Qu'est-ce que la régularisation ? Quel est le paramètre de régularisation de votre modèle ?
- Tracez la valeur du paramètre de régularisation en fonction de la corrélation de Pearson pour les ensembles de test et d'apprentissage, et voyez si votre modèle présente un problème de biais ou de variance.
