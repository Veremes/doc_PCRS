# Conception du projet FME #

Le projet Writers PCRS permettant l'écriture des données PCRS dans le format GML, nécessite un minimum de connaissances dans l'utilisation du logiciel FME. 

Le produit Writers PCRS correspond dans FME à 31 Transformers personnalisés. A l'exception de quelques Transformers de fonctionnement, chaque Transformers personnalisés est associé à une classe du standard PCRS.

## Prérequis ##

**Version FME**

La version minimale de FME à utiliser est la 2016.1.3.2.

**Installation de l'extension PCRS pour FME**

Suite à l'installation de l'extension PCRS pour FME, vous disposerez d'un trentaine de transformers supplémentaires correspondant aux classes du PCRS (PCRS_MarcheEscalierPCRS, PCRS_AffleurantPCRS...) et à des fonctions utilitaires (PCRS_MergePCRSObjects...).

Ces transformers sont regroupés dans la catégorie PCRS de la galerie des Transformers de FME et commencent tous par le préfixe PCRS_. Il vous suffit donc de taper ces lettres dans l'espace de travail de FME Workbench pour en obtenir la liste et pouvoir sélectionner le Transformer de votre choix.

**Licence PCRS pour FME**

L'extension PCRS pour FME est protégée par un fichier de licence.
Vous pouvez effectuer une demande de licence auprès de codes@veremes.com en fournissant votre code machine/registration key (n° à 10 chiffres visible dans l'utilitaire FME Licensing Assistant).

En l'absence de fichier de licence, les Transformers fonctionnent correctement mais ne laissent passer que 20 entités par classe et 500 au total.

**Limitations**

Actuellement seules les données vectorielles sont supportées par PCRS pour FME et il n'est possible de générer qu'une emprise par document GML. Le support du raster est prévu avant la fin de l'année 2018.

## Lien entre les données source et les Writers PCRS ##

La première étape consiste à lire le jeu de données source PCRS dans un projet FME selon le format d'origine des données. Le système de coordonnées doit obligatoirement être renseigné dans le jeu de données source.

Les Transformers personnalisés sont ensuite intégrés au projet FME au besoin. En effet, si les données source ne contiennent pas toutes les classes, inutile d'ajouter les Transformers relatifs aux classes manquantes.

L'objectif est d'établir le lien entre les données sources et les Transformers personnalisés.

**Exemple**

La classe "ArbrePCRS" est associée au Transformer personnalisé "PCRS_ArbrePCRS". L'utilisateur va alors relier dans FME son type d'entités source correspondant aux arbres au Transformer "PCRS_ArbrePCRS".

C'est le même principe pour l'ensemble des classes comme l'illustre la figure ci-dessous.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/donnees_sources.PNG)

## Prétraitements des données ##

Parfois, les données ne sont pas exploitables directement et nécessitent un prétraitement.

C'est à l'utilisateur de gérer cette partie en retravaillant les données pour les rendre conformes aux prérequis des Transformers.

**Exemple**

Un type d'entités source au format DGN nommé "Spits+txt" et correspondant à des points du canevas est ouvert dans le projet FME. L'idée est de connecter ce type d'entités source au Transformer associé nommé "PCRS_PointCanevasPCRS".

Voici la représentation d'un point de la classe d'origine "Spits+txt" dans le Data Inspector. En terme de géométrie, il ne s'agit pas d'un seul point, mais de plusieurs éléments (lignes, point, annotation).

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/point.PNG)

Le Transformer "PCRS_PointCanevasPCRS" attend un entrée une géométrie ponctuelle. Le type d'entités source ne peut donc pas être relié directement au Transformer, il nécessite un prétraitement.

L'objectif est alors de convertir chaque point d'origine composé de lignes, d'un point et d'une annotation en un seul point.

Les géométries initiales constituant le point sont définies par un numéro et un nom de cellule identique. Un regroupement peut alors être effectué sur ce critère avec le Transformer nommé "Aggregator".

En sortant de ce Transformer l'ensemble des géométries d'un point d'origine ne forment plus qu'un seul objet. L'étape suivante consiste alors à remplacer chaque objet par un point avec le Transformer "VertexCreator".

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/points_canevas.PNG)

La nécessité des traitements en amont sur les types d'entités dépend de la qualité des données source.

## Paramétrer les Transformers personnalisés ##

Lorsque la données source est connectée au Transformer personnalisé, le paramétrage de ce dernier peut alors être réalisé.

A l'ouverture d'un Transformer personnalisé, plusieurs éléments sont proposés. Les champs obligatoires sont visibles en rouge et les champs optionnels en blanc.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/transformer_facade.PNG)

La rubrique [Description du Writer PCRS pour FME](http://doc-pcrs.readthedocs.io/fr/latest/Writer_PCRS/index.html#description-du-writer-pcrs-pour-fme) donne des informations sur les classes du PCRS et liste les paramètres par Transformers, et la page [Paramètres publiés](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#PCRS_Parametres) explique tous les paramétrages des Transformers correspondant à des paramètres publiés pour FME.

## Regroupement des différents Transformers personnalisés ##

Les Transformers personnalisés doivent rejoindre le Transformer nommé "PCRS_EmpriseEchangePCRS". En effet, les différents objets du PCRS sont liés à l'emprise.

Le Transformer "PCRS_MergePCRSObjects" va quant-à lui regrouper l'emprise et l'ensemble des objets associés en fusionnant les éléments de XML des données entrantes.

A ce stade, un attribut dans FME contient l'ensemble du XML.

## Validation du fichier GML ##

Le Transformer "XMLValidator" peut être intégré pour valider le contenu de l'attribut XML en fonction des impératifs du XSD du standard.

Suite à la validation, l'attribut est renommé pour être exporté dans un fichier texte au format GML.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/regroupement.PNG)
