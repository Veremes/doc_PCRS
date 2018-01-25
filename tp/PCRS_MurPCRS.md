**Nom de la classe**

MurPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Murs, Murs de soutènement, Murs bahuts avec ou sans clôture, Clôtures sur socle, Parapets.

**Définition**

Classe permettant de décrire les ouvrages de maçonnerie (très souvent en briques ou parpaings) s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces. Certains objets de type socle ou bahut peuvent également être surmontés d'une clôture plus légère comme une grille ou un grillage.

**Modélisation**

Polyligne cf. modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS Les murs sont levés point par point, au sol, sur chaque côté du domaine public, et complété le cas échéant par un levé point par point, au sol, du côté du domaine privé accessible. Les murs peuvent être indifféremment décrits par leurs côtés sous la forme de polylignes ouvertes, ou par une description plus composite assemblant les polylignes ouvertes et refermant les extrémités pour constituer une unique polyligne fermée.
Le PCRS ne s'attache pas à décrire ni la hauteur du mur ni son épaisseur, ni même le matériau le constituant.
On ne cherchera à modéliser les piliers distribués le long ou aux extrémités de murs seulement lorsque leurs dimensions au sol sont différenciables de la largeur du mur, auquel cas de tels piliers seront décrits par des objets de type <PilierPCRS>.

**La classe contient**

Mur, bahut, gabion

**Attributs**

*géométrie*

- Type : GM_Curve

- Contraintes : 1

*typeMur*

- Type : CategorieMurPCRSType

- Contraintes : 0..1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS :|_PCRS.ID|
|Identifiant Objet:|_PCRS.IDOBJET|
|Thématique:|_PCRS.THEMATIQUE|
|Qualité Catégorisation:|_PCRS.QUALITECATEGORISATION|
|Précision Planimetrique:|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique:|_PCRS.PRECISIONALTIMETRIQUE|
|Producteur:|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ","):|_PCRS.NUMEROPOINT|
|Type Mur:|_PCRS.TYPEMUR|
