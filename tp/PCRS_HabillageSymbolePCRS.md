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

![Identifiant PCRS](Parametres.html#Identifiant PCRS_PCRS.ID)

![Identifiant Habillage](Parametres.html#Identifiant Habillage_PCRS.IDHABILLAGE)

![Thematique](Parametres.html#Thematique_PCRS.THEMATIQUE)

![Reference](Parametres.html#Reference_PCRS_REFERENCE)

![Angle de rotation](Parametres.html#Angle de rotation_PCRS_ANGLEROTATION)

![Longueur en mm](Parametres.html#Longueur en mm_PCRS_LONGUEUR_MM)