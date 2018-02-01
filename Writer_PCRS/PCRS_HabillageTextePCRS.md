# HabillageTextePCRS #



**Nom de la classe**

HabillageTextePCRS

**Sous-classe de**

HabillagePCRS

**Titre**

Texte d'habillage du PCRS

**Définition**

Classe spécialisée de la classe abstraite HabillagePCRS permettant de décrire tous les éléments d'habillage de type texte utiles à la compréhension du PCRS.

**Modélisation**

Point (propriété de la classe généralisée HabillagePCRS) <br>Libellé de type texte positionné de façon ponctuelle, avec possibilité de spécifier une orientation spécifique.

**La classe contient**

- les toponymes
- les coordonnées planimétriques
- les altimétries ...

**Contraintes**

Contraintes de positionnement en dehors de la voirie, en particulier en zone dense ou très dense.

**Géométrie**

*angleRotation*

- Définition : Utilisé uniquement pour l'orientation de l'élément d'habillage

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1

*geometrie*

- Définition : Géométrie de type point

- Type : GM_Point

- Contraintes : 1

*justification*

- Définition : Utilisé pour la justification de texte

- Type : TexteJustificationPCRSType

- Valeurs possibles :
  - G = Gauche
  - C = Centré
  - D = Droite


- Contraintes : 1

*libelle*

- Définition : Texte du libellé à utiliser comme habillage du PCRS

- Type : CharacterString

- Valeurs possibles : Valeur textuelle. Exemple : 123 m

- Contraintes : 1

*Taille*

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte

- Type : Décimal

- Contraintes : 1

**Pramètres**

![Identifiant PCRS](Parametres.html#Identifiant PCRS_PCRS.ID)

![Identifiant Habillage](Parametres.html#Identifiant Habillage_PCRS.IDHABILLAGE)

![_PCRS.IDHABILLAGE](Parametres.html#_PCRS.IDHABILLAGE_PCRS.THEMATIQUE)

![Libelle](Parametres.html#Libelle_PCRS.LIBELLE)
