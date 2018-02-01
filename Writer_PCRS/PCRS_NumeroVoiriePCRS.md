# NumeroVoiriePCRS #



**Nom de la classe**

NumeroVoiriePCRS

**Sous-classe de**

HabillageTextePCRS

**Titre**

Numéro d'adresse

**Définition**

Numéros de voirie de type adresse, liés à un référentiel donné, servant de données d'habillage du PCRS.
Les numéros de voirie du PCRS doivent être positionnés de façon à permettre un affichage à l'intérieur des parcelles (non modélisées dans le PCRS), et ne se superposant pas (pour des plans au 1/200ème) aux noms de voirie du PCRS, de façon à ne pas empiéter en zone dense ou très dense sur les espaces liés à la représentation des réseaux (non modélisés dans le PCRS).

**Modélisation**

Point (propriété de la classe généralisée HabillageTextePCRS) <br>
Libellé de type texte positionnant de façon ponctuelle le numéro d'adresse.

**Contraintes**

Contraintes de positionnement en dehors de l'espace public de la voirie, en particulier en zone dense ou très dense.

**Géométrie**

*idNumeroVoirie*

- Définition : Identifiant unique dans le jeu de données des numéros de voirie

- Type : CharacterString

- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée

- Contraintes : 1 Valeur unique

*positionnement*

- Définition : Indication quant au positionnement de l'élément d'habillage par rapport à la voirie

- Type : CategoriePlacementPCRSType

- Valeurs possibles :
  - 01 = Sans repositionnement
  - 02 = Axe Voirie
  - 03 = LimiteVoirie
  - 04 = HorsVoirie
  - 05 = Parcelle


- Contraintes : 0..1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Habillage|_PCRS.IDHABILLAGE|
|Thematique|_PCRS.THEMATIQUE|
|Libelle|_PCRS.LIBELLE|
|Angle de rotation|_PCRS_ANGLEROTATION|
|Justification|_PCRS.JUSTIFICATION|
|Taille|_PCRS.TAILLE|
|Numero de voirie|_PCRS.IDNUMEROVOIRIE|
|Positionnement|_PCRS.POSITIONNEMENT
