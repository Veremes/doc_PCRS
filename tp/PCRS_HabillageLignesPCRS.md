# HabillageLignesPCRS #



**Nom de la classe**

HabillageLignesPCRS

**Sous-classe de**

HabillagePCRS

**Titre**

Lignes d’habillage

**Définition**

Classe spécialisée de la classe abstraite <HabillagePCRS> permettant de décrire tous les éléments d'habillage de type lignes utiles à la compréhension du PCRS.

**Modélisation**

Multilignes

**La classe contient**

- les orographies,
- les dessins d'affleurants,
- les changements de revêtement non représentés comme des objets du PCRS
- les fondations
- les limites de haies, d’espace vert, etc.
-  largeur des ouvertures
...

**Attributs**

*géométrie*

- Définition : géométrie de type multi-courbe.

- Type : GM_MultiCurve

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Habillage|_PCRS.IDHABILLAGE|
|Thematique|_PCRS.THEMATIQUE|
