# PilierParticulierPCRS #



**Nom de la classe**

PilierParticulierPCRS

**Sous-classe de**

PilierPCRS

**Titre**

Pilier polygonal

**Définition**

Classe permettant de décrire les constructions en maçonnerie ou en métal, de section polygonale érigées dans le but de reprendre ou supporter des charges

**Modélisation**

Polyligne fermée Le pilier est levé point par point au niveau du sol et au sens de l'emprise maximum.  
N.B. La hauteur du pilier ne fait pas partie des informations levées dans le cadre du PCRS

**La classe contient**

Tout type de pilier à section de forme polygonale

**Contraintes**

Il est décidé par convention que l’intérieur du pilier mur porteur de la matière se situe à gauche de la polyligne prise dans l’ordre de ses sommets et par conséquent que la région vers l'extérieur associée au sol se situe à droite. Les singularités liées au cheminement polygonal, et en particulier la singularité dite « en papillon » doivent être évitées

**Critères de sélection**

Lorsque le pilier est attenant à un socle ou à un mur, ses dimensions au sol doivent le rendre différenciable (aux limites de précision planimétrique) du socle ou du mur attenant

**Attributs**

*géométrie*

- Définition : Géométrie de type courbe

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|_PCRS.QUALITECATEGORISATION|
|Précision Planimetrique|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
