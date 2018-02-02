# Paramètres publiés #

### Angle de rotation ###

1-
- Définition : Utilisé uniquement pour l'orientation de l'élément d'habillage

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1 valeur non vide

2- Utilisé uniquement pour l'orientation du symbole de poteau. Peut être étendu pour un poteau ovale pour orienter le symbole.

3- Angle utilisé uniquement pour l'orientation du symbole d'affleurant, dans le sens horaire par rapport au nord.


4-
- Définition : Utilisé uniquement pour l'orientation de l'élément d'habillage

- Type : Décimal

- Valeurs possibles : Valeur angulaire en degrés décimaux

- Contraintes : 1
### Canevas ###

Type de canevas auquel appartient le point considéré.

### Code INSEE ###

- Définition : Code INSEE de la commune

- Type : CharacterString

- Contraintes : 1

### Complement ###

- Définition : Information complémentaire liée au type d'emprise de publication du PCRS, gérée par le gestionnaire  du PCRS et potentiellement à tout utilisateur du PCRS

- Type : CharacterString

- Valeurs possibles : Selon le type d'emprise de publication, par exemple :
   - un toponyme pour une emprise de type couloir

   - le nom de l'opération pour une emprise de concernant une opération donnée

   - la référence du carreau (si elle n'est pas redondante avec l'identifiant de l'emprise), ou le nom du carroyage pour une emprise de type régulière

   - le nom ou le type de la limite administrative pur une emprise de type administrative ...

- Contraintes : 0..1 Optionnel : information en complément de l'identifiant d'emprise, et liée au type de l'emprise de publication devant être renseignée si gérée par le gestionnaire du PCRS


### Date Creation (aaaa-mm-jj) ###

Date de création ou de mise à jour des données du point de canevas.

### Date de Publication ###

- Définition : Date de mise à disposition de l'emprise du PCRS

- Type : Date

- Contraintes : 1

### Fiche ###

Adresse de type URL susceptible de fournir des informations supplémentaires, comme des photographies de repérage, sur le point de canevas.

### Fournisseur ###
### Gestionnaire ###

1-

- Définition : Nom de la collectivité gestionnaire du PCRS

- Type : CharacterString

- Contraintes : 1


2-

- Définition : Nom court, sigle, acronyme de l'opérateur gestionnaire du réseau et fournisseur de la donnée

- Type : CharacterString

- Valeurs possibles : Exemple : ENEDIS, GRDF, Lyonnaise des Eaux, etc

- Contraintes : 0..1

### Horodatage ###

Horodatage du point moment du levé topographique.

### Identifiant Affleurant Symbole ###

- Définition : Lien vers une représentation symbolique

- Type : Classe d'objets AffleurantSymbolePCRS

- Contraintes 0..1

### Identifiant Emprise ###

- Définition : Identifiant de l'emprise

- Type : CharacterString

- Contraintes : 1

### Identifiant Habillage ###

Identifiant unique de l'habillage.

### Identifiant habillage symbole ###
### Identifiant Objet ###

### Identifiant PCRS ###

Les identifiants sont obligatoirement renseignés. Ils sont calculés par défaut dans le projet FME.

### Identifiant Source ###

- Définition : Identifiant unique de l'affleurants

- Type : CharacterString

- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux.

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée

### Immatriculation ###

Référence externe selon la convention d'immatriculation du canevas considéré.

### Justification ###

- Définition : Utilisé pour la justification de texte

- Type : TexteJustificationPCRSType

- Valeurs possibles :
  - G = Gauche
  - C = Centré
  - D = Droite

- Contraintes : 1

### Largeur ###

1-
- Définition : Utilisé uniquement pour la mise à l'échelle Y du symbole Habillage

- Type : Décimal

- Contraintes : 1 Valeur non vide

2- Utilisé uniquement pour la mise à l'échelle Y du symbole de poteau après rotation.

3- Utilisé uniquement pour la mise à l'échelle Y du symbole de l'affleurant.

### Libellé ###

- Définition : Texte du libellé à utiliser comme habillage du PCRS

- Type : CharacterString

- Valeurs possibles : Valeur textuelle. Exemple : 123 m

- Contraintes : 1

### Longueur ###

1-
- Définition : Utilisé uniquement pour la mise à l'échelle X du symbole habillage

- Type : Décimal

- Contraintes : 1 Valeur non vide

2- Utilisé uniquement pour la mise à l'échelle X du symbole de poteau après rotation.

3- Utilisé uniquement pour la mise à l'échelle X du symbole de l'affleurant.

### Nature ###

- Définition : Nature de l'affleurant

- Type : NatureAffleurantPCRSType

- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux

  01 = avaloirs

  02 = Boîte, Coffret, Armoire

  03 = Tampon, plaque, chambre

  04 = Branchement, vanne, bouche à clé

  05 = Bouche incendie, Poteau incendie

  06 = poteaux

  07 = Poteau/borne d'éclairage

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée

### Nom ###

- Définition : Nom de la commune

- Type : CharacterString

- Contraintes : 0..1

### Nom voirie ###
### Numero de voirie ###
### Numero(s) des Point(s) Levé(s) (séparés par ",") ###

1- Numéro attribué au point levé lors du levé topographique ou de l’intégration au référentiel selon une ou plusieurs méthodologies à préciser si possible dans les métadonnées.

2- Lien vers les points levés correspondant à l‘objet.

### Positionnement ###

Indication quant au positionnement de l'élément d'habillage par rapport à la voirie.

### Précision Altimétrique ###

Intervalle de précision dans lequel s'exprime en cm la précision altimétrique associée au levé topographique de l'objet.

### Précision Planimétrique ###

Intervalle de précision dans lequel s'exprime en cm la précision planimétrique associée au levé topographique de l'objet.

### Precision XY ###

Précision planimétrique exprimée en cm.

### Precision Z ###

Précision altimétrique exprimée en cm.

### Producteur ###

Producteur de la donnée.

### Propriete ###

Distinction d'appartenance d'un tronçon de voirie à l'espace public ou à l'espace privé.

### Qualité Catégorisation ###

Indication du producteur quant à la qualité de la catégorisation. Permet des représentations plus riches pour les migrations / reprises de données.

### Reference ###

1-

- Définition : Référence vers une base de données des communes

- Type : CharacterString

- Contraintes : 1

2- Identifiant unique du tronçon dans le référentiel source utilisé.

3-
- Définition : Désignation du symbole à utiliser pour la représentation de l'habillage sous forme de symbole

- Type : CharacterString

- Contraintes : 1 Valeur non vide

4- Désignation du symbole à utiliser pour la représentation de l'affleurant.

5-
- Définition : Désignation du symbole à utiliser pour la représentation de l'arbre.

- Type : CharacterString

- Valeurs possibles : Permet le cas échéant de faire référence à des essences ou espèces d'arbres différents

- Contraintes : 1

### Reseau ###

- Définition : Nature du réseau

- Type : NatureReseauPCRSType

- Valeurs possibles :

  ASSAEU = Eaux usées

  ASSARU = Réseau unitaire

  00 = Non défini

  ASSA = Assainissement ou pluvial

  AEP = Eau potable

  ELECECL = Electricité

  GAZ = Gaz

  MULT = Multi-réseaux

  ELECSLT = Signalisation lumineuse tricolore

  COM = Télécom

  ASSAEP = Eaux pluviales

  DECH = déchets

  INCE = Incendie

  CHIM = Produits chimiques

  CHAU = Chauffage et climatisation

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée


### Section ###

Forme de la section à la base du pilier.

### Source ###

1- Acronyme du référentiel utilisé.

2-

- Définition : Source de données d'affleurant dans le SI du gestionnaire de réseaux

- Type : CharacterString

- Valeurs possibles : Nom d'application ou de base de données dans le système d'information du gestionnaire de réseaux

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée

### Taille ###

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte

- Type : Décimal

- Contraintes : 1

### Thématique ###

1- La thématique à laquelle est associé l'élément d'habillage du PCRS.

2- La thématique à laquelle est associé chaque objet du PCRS.

### Transparence ###
### Type ###

- Définition : Type d'emprise du PCRS

- Type : CharacterString

- Valeurs possibles : Par exemple : Couloir, Opération, Carreau, LimiteAdministrative

- Contraintes : 0..1

### Type Mur ###

Description des ouvrages de maçonnerie s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces.
