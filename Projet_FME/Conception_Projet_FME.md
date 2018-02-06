# Conception du projet FME #
Le projet Writers PCRS permettant l'écriture des données PCRS dans le format GML, nécessite un minimum de connaissances dans l'utilisation du logiciel FME.
![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/TP.PNG)

## Prérequis ##

**Version FME**

La version minimale de FME à utiliser est la 2016.1.

**Installation des Transformers personnalisés**

- Clique-droit sur les Transformers personnalisés > "Install".

- Ou bien, déplacer l'ensemble des Transformers personnalisés dans le répertoire : \Documents\FME\Transformers.

## Lien entre les données sources et les Writers PCRS ##

La première étape consiste à lire le jeu de données sources PCRS dans FME selon le format d'origine des données.

Chaque Writer PCRS est associé à une classe du standard PCRS et les classes correspondent à des Transformers personnalisés dans FME.

L'objectif est d'établir le lien entre les données sources et les Transformers personnalisés.

![](https://raw.githubusercontent.com/Veremes/doc_PCRS/master/Images/donnees_sources.PNG)

Par exemple, la classe "ArbrePCRS" issue de la sous-classe "ObjetVecteurPCRS" est associée au Transformer personnalisé "PCRS_ArbrePCRS".

L'objectif est d'établir le lien entre les données sources relatives aux arbres et le Transformer personnalisé "PCRS_ArbrePCRS".

la structure des données en sortie correspondant aux spécifications du standard.




Le produit Writers PCRS contient 31 formats personnalisés.
## Regroupement des différents Writers PCRS ##

## Validation du fichier GML ##
