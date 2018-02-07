# Conception du projet FME #
Le projet Writers PCRS permettant l'écriture des données PCRS dans le format GML, nécessite un minimum de connaissances dans l'utilisation du logiciel FME.

Chaque Transformers personnalisés dans FME est associé à une classe du standard PCRS.

la structure des données en sortie correspondant aux spécifications du standard.

Le produit Writers PCRS contient 31 formats personnalisés.

## Prérequis ##

**Version FME**

La version minimale de FME à utiliser est la 2016.1.

**Installation des Transformers personnalisés**

- Clique-droit sur les Transformers personnalisés > "Install".

- Ou bien, déplacer l'ensemble des Transformers personnalisés dans le répertoire : \Documents\FME\Transformers.

## Lien entre les données source et les Writers PCRS ##

La première étape consiste à lire le jeu de données source PCRS dans un projet FME selon le format d'origine des données.

Les Transformers personnalisés sont ensuite intégrés au projet FME au besoin. En effet, si les données source ne contiennent pas toutes les classes, inutile d'ajouter les Transformers relatifs aux classes manquantes.

L'objectif est d'établir le lien entre les données sources et les Transformers personnalisés.

**Exemple**

La classe "ArbrePCRS" est associée au Transformer personnalisé "PCRS_ArbrePCRS". L'utilisateur va alors relier dans FME son type d'entités source correspondant aux arbres au Transformer "PCRS_ArbrePCRS".

C'est le même principe pour l'ensemble des classes comme l'illustre la figure ci-dessous.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/donnees_sources.PNG)

## Prétraitements des données ##

Parfois, les données ne sont pas exploitables directement et nécessitent un prétraitement.

C'est à l'utilisateur de gérer cette partie en retravaillant les données pour les rendre conformes aux spécifications des Transformers.

**Exemple**

Un type d'entités source au format DGN nommé "Spits+txt" et correspondant à des points du canevas est ouvert dans le projet FME. L'idée est de connecter ce type d'entités source au Transformer correspondant nommé "PCRS_PointCanevasPCRS".

Voici la représentation d'un point de la classe d'origine "Spits+txt" dans le Data Inspector. En terme de géométrie, il ne s'agit pas d'un seul point, mais de plusieurs éléments (lignes, point, annotation).

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/point.PNG)

Le Transformer "PCRS_PointCanevasPCRS" attend un entrée une géométrie ponctuelle. Le type d'entités source ne peut donc pas être relié directement au Transformer, il nécessite un prétraitement.

L'objectif est alors de convertir chaque point d'origine composé de lignes, d'un point et d'une annotation en un seul point.

Les géométries initiales constituant le point sont définies par un numéro et un nom de cellule identique. Un regroupement peut alors être effectué sur ce critère avec le Transformer nommé "Aggregator".

En sortant de ce Transformer l'ensemble des géométries d'un point d'origine ne forment plus qu'un seul objet. L'étape suivante consiste alors à remplacer chaque objet par un point avec le Transformer "VertexCreator".

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/points_canevas.PNG)

## Paramétrer les Transformers personnalisés ##

## Regroupement des différents Writers PCRS ##

## Validation du fichier GML ##
