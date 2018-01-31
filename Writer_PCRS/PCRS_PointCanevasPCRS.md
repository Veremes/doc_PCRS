# PointCanevasPCRS #



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

**Attributs**

*canevas*

- Définition : Type de canevas auquel appartient le point considéré

- Type : CharacterString

- Contraintes : 0..1  Optionnel  : lorsque le point appartient à un canevas donné, il est recommandé de le renseigner

*dateCreation*

- Définition : Date de création ou de mise à jour des données du point de canevas

- Type : Date

- Contraintes : 0..1  Optionnel  : lorsque la date de création ou de mise à jour des données du point de canevas est connue, il est obligatoire de la renseigner

*fiche*

- Définition : Adresse de type URL susceptible de fournir des informations supplémentaires, comme des photographies de repérage,  sur le point de canevas

- Type : URL

- Contraintes : 0..1

*geometrie*

- Définition : Géométrie du point

- Type : GM_Point

- Contraintes : 1

*immatriculation*

- Définition : Référence externe selon la convention d'immatriculation du canevas considéré

- Type : CharacterString

- Contraintes : 0..1  Optionnel  : lorsque le matricule du point est connu, il est obligatoire de le renseigner

*PrecisionXY*

- Définition : Précision planimétrique exprimée en cm

- Type : Integer

- Contraintes : 0..1  Optionnel, à renseigner si disponible

*PrecisionZ*

- Définition : Précision altimétrique exprimée en cm

- Type : Integer

- Contraintes : 0..1  Optionnel, à renseigner si disponible

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
|Canevas|_PCRS.CANEVAS|
|Date Creation (aaaa-mm-jj)|_PCRS.DATECREATION|
|Fiche|_PCRS.FICHE|
|Immatriculation|_PCRS.IMMATRICULATION|
|Precision XY|_PCRS.PRECISIONXY|
|Precision Z|_PCRS.PRECISIONZ|  
