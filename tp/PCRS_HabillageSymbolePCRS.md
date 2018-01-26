# HabillageSymbolePCRS #



**Nom de la classe**

HabillageSymbolePCRS

**Sous-classe de**

HabillagePCRS

**Titre**

Symbole d'habillage du PCRS

**Définition**

Classe spécialisée de la classe abstraite HabillagePCRS permettant de décrire tous les éléments d'habillage de type symbole utiles à la compréhension du PCRS.

**Modélisation**

Point (propriété de la classe généralisée HabillagePCRS) Point de référence au centre du symbole, dont on précisera la référence, les dimensions inscrites dans un rectangle (longueur, largeur), et l'orientation spécifique.

**Contraintes**

Contraintes de positionnement en dehors de la voirie, en particulier en zone dense ou très dense.

**Attributs**

*angleRotation*

- Définition : Utilisé uniquement pour l'orientation de l'élément d'habillage

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1 valeur non vide

*géométrie*

- Définition : Géométrie de type ponctuel .

- Type : GM_Point

- Contraintes : 1

*largeur_mm*

- Définition : Utilisé uniquement pour la mise à l'échelle Y du symbole Habillage

- Type : Décimal

- Contraintes : 1 Valeur non vide

*longueur_mm*

- Définition : Utilisé uniquement pour la mise à l'échelle X du symbole habillage

- Type : Décimal

- Contraintes : 1 Valeur non vide

*référence*

- Définition : Désignation du symbole à utiliser pour la représentation de l'habillage sous forme de symbole .

- Type : CharacterString

- Contraintes : 1 Valeur non vide

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Habillage|_PCRS.IDHABILLAGE|
|Thematique|_PCRS.THEMATIQUE|
|Reference|_PCRS_REFERENCE|
|Angle de rotation|_PCRS_ANGLEROTATION|
|Longueur en mm|_PCRS_LONGUEUR_MM|
|Largeur en mm|_PCRS.LARGEUR_MM|
