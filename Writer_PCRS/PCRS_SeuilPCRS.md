# PCRS_SeuilPCRS #



**Nom de la classe**

SeuilPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Seuil, Ouverture d'un bâtiment ou d'un mur

**Définition**

Classe permettant de décrire l'ensemble des portes, portes cochères, portails, seuils permettant l'entrée ou la sortie dans un bâtiment ou dans une enceinte (AIVF_19_3).

**Modélisation**

Ligne <br>
La ligne est définie comme le segment reliant deux points levés (dans le même sens que le levé de façade du bâtiment ou du mur), et de part et d'autre de l'ouverture du bâtiment ou du mur Le point de seuil, déterminé par calcul, est situé à l'axe du seuil, et sert éventuellement à positionner un symbole décrit par un objet SymboleHabillagePCRS.

**La classe contient**

- Seuil piéton (ou seuil de maison)  

- Seuil véhicule (ou seuil de garage)

- Seuil d’ouverture

**Critères de sélection**

À l'exclusion de tout seuil de cave.

**Géométrie**

- Définition : Géométrie de type courbe.

- Type : GM_Curve.

**Paramètres**

[Identifiant Habillage Symbole](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-habillage-symbole)

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
