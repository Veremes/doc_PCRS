# PCRS_PointCanevasPCRS #



**Nom de la classe**

PointCanevasPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Points de canevas topographique

**Définition**

Un canevas topographique est constitué d'un ensemble de points matérialisés sur le terrain, repérés en coordonnées XY et Z dans les référentiels géographiques planimétriques et altimétriques en vigueur, facilitant ainsi la production de séries de données géographiques cohérentes et homogènes lors des levés topographiques réalisés par les géomètres. Ils disposent d'une immatriculation spécifique au canevas utilisé et sont en général documentés par une fiche signalétique accessible au public.

**Modélisation**

Point <br>Lorsque l'altimétrie du point de canevas est disponible, il est obligatoire de la fournir sous forme de coordonnée Z.

**La classe contient**

Tout point précédemment déterminé et matérialisé sur le terrain et répondant à la précision attendue.   

**Contraintes**

La modélisation conceptuelle des points de canevas est uniquement topographique, et ne se substitue pas à la logique de gestion de ceux ci et pour laquelle un des principaux cas d'utilisation correspond à l'information du public, avec adresse de localisation, photographie, URL, etc... Les gestionnaires des différents canevas entretiennent pour cela d'autres séries de données pour lesquelles l'immatriculation d'un point de canevas associée au type de canevas concerné permettent le cas échéant de mettre en relation les données du PCRS avec les données sources d'immatriculation et de gestion des points de canevas.

**Critères de sélection**

Les points de canevas dont la précision ne serait pas au moins égale à celle attendue lors du levé topographique des objets du PCRS sont exclus de cette classe d'objets.

**Géométrie**

- Définition : Géométrie du point.

- Type : GM_Point.

**Paramètres**

[Canevas](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#canevas)

[Date Création](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#date-creation)

[Fiche](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#fiche)

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Immatriculation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#immatriculation)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Précision XY](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-xy)

[Précision Z](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-z)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
