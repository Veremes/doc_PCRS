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

Un type d'entités source au format DGN nommé "Spits+txt" et correspondant à des points levés est ouvert dans le projet FME.

Voici la représentation d'un point dans le Data Inspector.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/point.PNG)



souhaite relier son type d'entités correspondant aux points levés "Spits+txt" au Transformer "PCRS_PointCanevasPCRS",   

## Paramétrer les Transformers personnalisés ##

## Regroupement des différents Writers PCRS ##

## Validation du fichier GML ##
