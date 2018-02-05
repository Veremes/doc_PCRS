# FacadePCRS #



**Nom de la classe**

FacadePCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Façade de bâtiment, murs de façade

**Définition**

Classe permettant de décrire les éléments de gros-oeuvre, parfois de second-oeuvre, participant aux faces extérieures d'un bâtiment public ou privé et présentant une importance étendue.

**Modélisation**

Polyligne <br>
La façade est levée au niveau du « nu » du mur principal à la hauteur du soubassement (ou du trottoir en absence de soubassement), en privilégiant autant que possible un levé en entier du bâtiment, formant ainsi une polyligne fermée. Lorsque le bâtiment ne peut être levé en entier en tant que façade, la polyligne résultante est alors une polyligne ouverte.

**Contraintes**

Afin de faciliter les représentations de type DAO, il est recommandé par convention que l’intérieur de la façade se situe à gauche de la polyligne prise dans l’ordre de ses sommets et par conséquent que la région vers l'extérieur associée au sol ou au soubassement se situe à droite.
Toute autre convention ou absence de convention dans l'ordre des sommets devra explicitement être mentionnée dans les métadonnées de publication du PCRS Classe essentielle du PCRS.

 **Critères de sélection**

Concerne aussi bien les bâtiments durs que les bâtiments légers. Ne comprends ni les avant-corps (volumes en avancée) et ni les arrière-corps (volumes en retrait) donnant le relief de façade à compter du « nu » du mur principal.
Ne comprend donc pas le soubassement (partie inférieure, massive, d'une construction, qui surélève celle-ci au niveau du sol ©Larousse) décrit par l'objet "ProeminenceBatiPCRS".
Ne tient pas compte des éventuels décrochements de seuil (seuils de maison, de cave ou de garage), décrits par ailleurs par l'objet SeuilPCRS.

**Géométrie**

- Définition : Géométrie de type de courbe

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
