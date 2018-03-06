.. pcrs documentation master file, created by
   sphinx-quickstart on Fri May 12 08:54:22 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Documentation de PCRS pour FME
====================================
Le Plan de Corps de Rue Simplifié constitue un référentiel commun de base décrivant à grande échelle les limites apparentes de la voirie, aussi bien en zones urbaines denses qu’en zones rurales.

Le GML (Geography Markup Language) est le format défini pour l’échange des données relatives au PCRS. Les spécifications du standard sont écrites dans un fichier XSD (schéma d’application du fichier GML) livré par le Conseil National de l'Information Géographique (CNIG). Le XSD constitue alors le standard de référence à respecter pour la validation des données PCRS.

Dans l'optique de faciliter la production de données au format GML, Veremes propose un Writer PCRS pour FME permettant l'écriture de données PCRS dans le format GML en respectant les contraintes du standard XSD proposé par le CNIG.

La documentation est basée sur le fonctionnement du Writer PCRS pour FME de Veremes en accord avec la version 2.0 du standard du PCRS de septembre 2017 présente sur le site internet du CNIG : http://cnig.gouv.fr/wp-content/uploads/2017/12/CNIG_RTGE_PCRS_v2.0.pdf.



.. toctree::
   :maxdepth: 2

   Projet_FME/index.rst
   Writer_PCRS/index.rst
