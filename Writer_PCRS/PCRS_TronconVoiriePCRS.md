# PCRS_TronconVoiriePCRS #



**Nom de la classe :**

TronconVoirie

**Titre**

Tronçon de Voie

**Définition**

Le tronçon de voirie du PCRS est un segment d'axe de voie entre deux intersections (qui ne sont pas modélisées dans le PCRS par ailleurs). Il sert essentiellement à identifier en premier lieu les emprises de publication du PCRS qui le concernent. Les noms de voirie, qui nécessitent un positionnement spécifique en dehors de l'espace où figurent les réseaux, et en particulier en zone urbaine dense, sont modélisés par ailleurs en tant que NomVoiriePCRS et ne sont donc pas gérés comme des données attributaires des tronçons de voirie du PCRS. De même, les numéros d'adresse, modélisés par ailleurs en tant que NumeroVoiriePCRS ne sont pas non plus liés aux tronçons de voirie du PCRS.

**Modélisation**

Polyligne <br>
Le tronçon de voirie s'appuie sur les tronçons du filaire des voies entretenu par la collectivité gestionnaire du PCRS, et pouvant s'appuyer sur des référentiels comme la BDUni ou la BD TOPO.

**Contraintes**

Classe accompagnant les métadonnées de publication du PCRS.

**Géométrie**

- Définition : Géométrie de type courbe.

- Type : GM_Curve.

**Paramètres**

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Propriété](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#propriete)

[Référence](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#reference)

[Source](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#source)
