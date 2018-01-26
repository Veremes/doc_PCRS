# PilePontPCRS #



**Nom de la classe**

PilePontPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Pile ou culée de pont du PCRS

**Définition**

Classe permettant de décrire les appuis massifs et permanents supportant les tabliers des ponts

**Modélisation**

Polyligne ouverte ou fermée (GM_Curve) Les piles de pont sont levées le long de la limite apparente avec le revêtement voisin, point à point et au niveau du sol (fil d'eau). Les autres aspects de la modélisation géométrique sont propres à  ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS

**La classe contient**

Pile (appuis intermédiaires) ou culées (appuis d'extrémité)

**Critère de sélection**

Appuis massifs et permanents supportant le tablier d'un pont

**Attributs**

*géométrie*

- Définition : Géométrie de type polygone .

- Type : GM_Polygon

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|QUALITECATEGORISATION|
|Précision Planimetrique|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
