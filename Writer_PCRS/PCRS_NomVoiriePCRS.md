# NomVoiriePCRS #



**Nom de la classe**

NomVoiriePCRS

**Sous-classe de**

HabillageTextePCRS

**Titre :**

Nom de voirie, Nom de voie

**Définition**

Noms de voirie associés aux voies modélisées par tronçons. Ils sont liés à un référentiel donné, et servent de données d'habillage du PCRS. Les noms de voirie du PCRS doivent si possible être placés hors espace public (sur les parcelles privées) de façon à ne pas empiéter en zone dense ou très dense sur les espaces liés à la représentation des réseaux (non modélisés dans le PCRS) de façon à permettre un affichage ne se superposant pas (pour des plans au 1/200ème) aux numéros de voirie du PCRS.

**Modélisation**

Point (propriété de la classe généralisée HabillageTextePCRS) <br>Libellé de type texte positionnant de façon ponctuelle le nom de voirie avec une orientation liée au tronçon de voirie le plus proche de la voie associée à l'adresse.

**Contraintes**

Contraintes de positionnement en dehors de l'espace public de la voirie, en particulier en zone dense ou très dense, à préciser localement.


**Attributs**

*idNomVoirie*

- Définition : Identifiant unique dans le jeu de données des noms voirie

- Type : CharacterString

- Valeurs possibles : Selon La collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée

- Contraintes : 1 Valeur unique

*positionnement*

- Définition : Indication quant au positionnement de l'élément d'habillage par rapport à la voirie

- Type : CategoriePlacementPCRSType

- Valeurs possibles :

  - 01 = sans repositionnement
  - 02 = AxeVoirie
  - 03 = LimiteVoirie
  - 04 = HorsVoirie
  - 05 = parcelles


- Contraintes : 0..1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Habillage|_PCRS.IDHABILLAGE|
|Libelle|_PCRS.LIBELLE|
|Libelle|_PCRS.LIBELLE|
|Angle de rotation|_PCRS_ANGLEROTATION|
|Justification|_PCRS.JUSTIFICATION|
|Taille|_PCRS.TAILLE|
|Nom voirie|_PCRS.IDNOMVOIRIE|
|_PCRS.IDNOMVOIRIE|_PCRS.POSITIONNEMENT|
