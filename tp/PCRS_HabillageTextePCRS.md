**Nom de la classe**

HabillageTextePCRS

**Sous-classe de**

HabillagePCRS

**Titre**

Texte d'habillage du PCRS

**Définition**

Classe spécialisée de la classe abstraite HabillagePCRS permettant de décrire tous les éléments d'habillage de type texte utiles à la compréhension du PCRS.

**Modélisation**

Point (propriété de la classe généralisée HabillagePCRS) Libellé de type texte positionné de façon ponctuelle, avec possibilité de spécifier une orientation spécifique.

**La classe contient**

- les toponymes,
- les coordonnées planimétriques,
- les altimétries,
...

**Contraintes**

Contraintes de positionnement en dehors de la voirie, en particulier en zone dense ou très dense.

**Attributs**

*angleRotation*

- Définition : Utilisé uniquement pour l'orientation de l'élément d'habillage

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1

*géométrie*

- Définition : Géométrie de type point

- Type : GM_Point

- Contraintes : 1

*justification*

- Définition : Utilisé pour la justification de texte

- Type : TexteJustificationPCRSType

- Valeurs possibles :
+-  - C = centré
  - D = droite

- Contraintes : 1

*Taille*

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte

- Type : Décimal

- Contraintes : 1

**Pramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS :|_PCRS.ID|
|Identifiant Habillage:|_PCRS.IDHABILLAGE|
|_PCRS.IDHABILLAGE|_PCRS.THEMATIQUE|
|Libelle:|_PCRS.LIBELLE|
|Angle de rotation:|_PCRS_ANGLEROTATION|
|Justification:|_PCRS.JUSTIFICATION|
|Taille:|_PCRS.TAILLE|
