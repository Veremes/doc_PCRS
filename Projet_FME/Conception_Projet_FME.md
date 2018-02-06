# Conception du projet FME #

Le projet Writers PCRS permettant l'écriture des données PCRS dans le format GML, nécessite un minimum de connaissances dans l'utilisation du logiciel FME. En effet, il faut établir manuellement le lien entre les données sources et la structure des données en sortie correspondant aux spécifications du standard.

La version minimale de FME à utiliser est la 2016.1.

Chaque Writer est associé à une classe du standard PCRS et les classes correspondent à des Transformers personnalisés dans FME. Par exemple, pour la classe "ArbrePCRS" issue de la sous-classe "ObjetVecteurPCRS", le Transformer personnalisé "PCRS_ArbrePCRS" va être utilisé.

![TEST](/Images/TP.jpg)
