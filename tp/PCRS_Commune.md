**Nom de la classe**

Commune

**Titre**

Lien vers un objet « commune »

**Définition**

Cette classe permet de référencer une commune présente dans un référentiel externe.

**Modélisation**

 Multi Polygone (GM_MultiPolygon) Les communes sont modélisées par un ensemble de polygones. La géométrie est indicative et la précision géométrique accordée importe peu.

**Critères de sélection**

Seuls sont considérés les objets « commune » d'un jeu de données de référence, défini par le gestionnaire du PCRS.

**Attributs**

*Code INSEE*

- Définition : Code INSEE de la commune

- Type : CharacterString

- Contraintes : 1

*géométrie*

- Définition : Géométrie de la commune

- Type : GM_MultiSurface

- Contraintes : 1

*nom*

- Définition : Nom de la commune

- Type : CharacterString

- Contraintes : 0..1

*référence*

- Définition : Référence vers une base de données des communes

- Type : CharacterString

- Contraintes : 1

**Paramètres**


| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS (calculé par défaut):|_PCRS.ID|
|Code INSEE:|_PCRS.COMMUNE_CODEINSEE|
|Nom:|_PCRS.COMMUNE_NOM|
|Reference:|_PCRS.REFERENCE|
