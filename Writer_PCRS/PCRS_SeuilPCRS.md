# SeuilPCRS #



**Nom de la classe**

SeuilPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Seuil, Ouverture d'un bâtiment ou d'un mur

**Définition**

Classe permettant de décrire l'ensemble des portes, portes cochères, portails, seuils permettant l'entrée ou la sortie dans un bâtiment ou dans une enceinte (AIVF_19_3).

**Modélisation**

Ligne La ligne est définie comme le segment reliant deux points levés (dans le même sens que le levé de façade du bâtiment ou du mur), et de part et d'autre de l'ouverture du bâtiment ou du mur Le point de seuil, déterminé par calcul, est situé à l'axe du seuil, et sert éventuellement à positionner un symbole décrit par un objet SymboleHabillagePCRS.

**La classe contient**
Seuil piéton (ou seuil de maison)  Seuil véhicule (ou seuil de garage) ( © Brest métropole) Seuil d’ouverture
Seuil piéton (ou seuil de maison).

**Critères de sélection**

À l'exclusion de tout seuil de cave.

**Attributs**

*géométrie*

- Définition : Géométrie de type courbe

- Type : GM_Curve

- Contraintes : 1

*symbole*

- Type : Classe d'objets HabillageSymbolePCRS

- Contraintes : 0..1

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
|Identifiant habillage symbole|_PCRS.IDHABILLAGESYMBOLE|
