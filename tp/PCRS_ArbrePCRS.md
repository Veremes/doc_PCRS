# ArbrePCRS #



**Nom de la classe**

ArbrePCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Arbre

**Définition**

Classe permettant de décrire les arbres régulièrement entretenus de la voirie du domaine public.  

**Modélisation**

 Point (GM_Point) L'arbre est modélisé par un point levé en axe du tronc, à hauteur du terrain naturel hors éventuel monticule au pied.

Les autres aspects de la modélisation géométrique sont propres à ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS.

**La classe contient**

 Selon toutes essences et espèces d'arbres.

 **Attributs**

*géométrie*

 - Type : GM_Point

 - Contraintes : 1

*référence*

 - Définition : Désignation du symbole à utiliser pour la représentation de l'arbre.

 - Type : CharacterString

 - Valeurs possibles : Permet le cas échéant de faire référence à des essences ou espèces d'arbres différents

 - Contraintes : 1

 **Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|_PCRS.QUALITECATEGORISATION|
|Précision Planimetrique|PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
|Reference:|_PCRS.REFERENCE|