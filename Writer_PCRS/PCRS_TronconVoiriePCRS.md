# TronconVoiriePCRS #



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

**Attributs**

*geometrie*

- Définition : Géométrie de type courbe

- Type : GM_Curve

- Contraintes : 1

*propriete*

- Définition : Distinction d'appartenance  d'un tronçon de voirie à l'espace public ou à l'espace privé

- Type : ProprieteEspaceType

- Valeurs possibles :

  - 01 = Espace public
  - 02 = Espace privé
  

- Contraintes : 0..1 Optionnel à renseigner si possible, lorsqu'une superposition avec les données cadastrales n'est pas envisageable

*reference*

- Définition : Identifiant unique du tronçon dans le référentiel source utilisé

- Type : CharacterString

- Valeurs possibles : Selon le fournisseur du référentiel donné

*source*

- Définition : Acronyme du référentiel utilisé

- Type : CharacterString

- Valeurs possibles : Selon le fournisseur du référentiel

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS |_PCRS.ID|
|Pcrs.reference|_PCRS.REFERENCE|
|Pcrs.source|_PCRS.SOURCE|
|Pcrs.propriete|_PCRS.PROPRIETE|
