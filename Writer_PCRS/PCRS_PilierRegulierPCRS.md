# PilierRegulierPCRS #



**Nom de la classe**

PilierRegulierPCRS

**Sous-classe de**

PilierPCRS

**Titre**

Pilier circulaire, pilier carré, pilier rectangulaire

**Définition :**

Classe permettant de décrire les constructions en maçonnerie ou en métal, de section circulaire, carrée, rectangulaire érigées dans le but de reprendre ou supporter des charges.

**Modélisation**

 Point

**La classe contient**

Tout type de pilier de forme régulière à section circulaire, carrée ou rectangulaire et quelle que soit la taille de sa section ou la matière le constituant.

**Critères de sélection**

Lorsque le pilier est associé à un socle ou à un mur, ses dimensions au sol doivent le rendre différenciable (aux limites de précision planimétrique) du socle ou du mur attenant.

**Géométrie**

*angleRotation*

- Définition : Utilisé uniquement pur l'orientation du symbole de poteau. Peut être étendu pour un poteau ovale pour orienter le symbole

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1 Valeur non vide

*geometrie*

- Définition : Géométrie de type point

- Type : GM_Point

- Contraintes : 1

*largeur_mm*

- Définition : Utilisé uniquement pour la mise à l'échelle Y du symbole de poteau après rotation

- Type : Décimal

- Contraintes : 1 Valeur non vide

*longueur_mm*

- Définition : Utilisé uniquement pour la mise  l'échelle X du symbole de poteau après rotation

- Type : Décimal

- Contraintes : 1 Valeur non vide

*section*

- Définition : Forme de la section à la base du pilier

- Type : SectionPilierPCRSType

- Valeurs possibles :

  - 01 = Pilier carré
  - 02 = Pilier circulaire
  - 03 = Pilier rectangulaire
  - 00 = Pilier à autre forme de section


- Contraintes : 1 Valeur non vide : l'attribut est utilisé pour différencier les piliers selon leur nature

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|QUALITECATEGORISATION|
|Précision Planimetrique|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|_PCRS.PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
|Angle Rotation|_PCRS.ANGLEROTATION|
|Largeur|_PCRS.LARGEUR|
|Longueur|_PCRS.LONGUEUR|
|Section|_PCRS.SECTION|
