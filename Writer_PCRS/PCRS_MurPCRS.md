# MurPCRS #



**Nom de la classe**

MurPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Murs, Murs de soutènement, Murs bahuts avec ou sans clôture, Clôtures sur socle, Parapets.

**Définition**

Classe permettant de décrire les ouvrages de maçonnerie (très souvent en briques ou parpaings) s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces. Certains objets de type socle ou bahut peuvent également être surmontés d'une clôture plus légère comme une grille ou un grillage.

**Modélisation**

Polyligne <br>
Les murs sont levés point par point, au sol, sur chaque côté du domaine public, et complété le cas échéant par un levé point par point, au sol, du côté du domaine privé accessible. Les murs peuvent être indifféremment décrits par leurs côtés sous la forme de polylignes ouvertes, ou par une description plus composite assemblant les polylignes ouvertes et refermant les extrémités pour constituer une unique polyligne fermée.
Le PCRS ne s'attache pas à décrire ni la hauteur du mur ni son épaisseur, ni même le matériau le constituant.
On ne cherchera à modéliser les piliers distribués le long ou aux extrémités de murs seulement lorsque leurs dimensions au sol sont différenciables de la largeur du mur, auquel cas de tels piliers seront décrits par des objets de type "PilierPCRS".

**La classe contient**

- Mur, bahut, gabion

- Mur de soutènement

- Parapet, garde-Corps

- Clôture sur socle ou Bahut avec clôture

- Enrochements

**Contraintes**

Afin de faciliter les représentations de type DAO, il est recommandé par convention que l’intérieur du mur porteur de la matière (briques, parpaings, béton, pierre...) se situe à gauche de la polyligne prise dans l’ordre de ses sommets et par conséquent que la région vers l'extérieur associée au sol se situe à droite.
Toute autre convention ou absence de convention dans l'ordre des sommets devra explicitement être mentionnée dans les métadonnées de publication du PCRS.
Classe essentielle du PCRS.

**Critères de sélection**

Les murs de pierre taillée ou non, ou constitués d'assemblages de bloc sont susceptibles de présenter des irrégularités incompatibles avec les exigences de précision du PCRS : ils ne constituent donc pas à proprement parler des murs du PCRS.
Ils doivent toutefois être décrits en renseignant spécifiquement les précisions planimétriques et/ou altimétriques par des valeurs très supérieures à celles exigées pour le PCRS.

**Géométrie**

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-s-des-point-s-leve-s-separes-par)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)

[Type Mur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#type-mur)
