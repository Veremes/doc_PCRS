**Nom de la classe**

MasqueOpacitePCRS

**Sous-classe de**

HabillagePCRS

**Titre**

Masque d'opacité du PCRS

**Définition**

Lorsqu'une image est disponible, un masque d'opacité correspond à la définition d'une zone surfacique pouvant s'étendre partiellement sur une ou plusieurs orthophotographies et pour laquelle localement les objets vecteur viennent compléter l’image. Afin de pouvoir visualiser le vecteur en superposition à l'image sur cette zone, un masque blanc, partiellement transparent est superposé à l'image.  

**Modélisation**

Surface

**Contraintes**

Classe essentielle pour l’utilisation d’orthophotoplans.

**Attributs**

*géométrie*

- Définition : Géométrie de type surfacique représentant la zone masquée .

- Type : GM_Surface  

- Contraintes : 1

*raster*

- Type : Classe d'objets RasterPCRS

- Contraintes : 1..*

*transparence*

- Définition : Pourcentage de transparence inversement proportionnelle à l'opacité de la zone .

- Type : Integer

- Valeurs possibles : de 0 à 100

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS :|_PCRS.ID
|Identifiant Habillage:|_PCRS.IDHABILLAGE|
|Thematique:|_PCRS.THEMATIQUE|
|Transparence:|_PCRS.TRANSPARENCE|
