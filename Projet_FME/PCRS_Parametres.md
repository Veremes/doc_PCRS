# Paramètres publiés #

### Angle de rotation ###

- Définition : Utilisé pour l'orientation de l'élément d'habillage, du symbole de poteau (pouvant être étendu pour un poteau ovale pour orienter le symbole) et du symbole d'affleurant, dans le sens horaire par rapport au nord.


- Type : Décimal.


- Valeurs possibles : Valeur angulaire en degrés décimaux.


- Contraintes : 1 valeur non vide.

### Canevas ###

- Définition : Type de canevas auquel appartient le point considéré.


- Type : CharacterString.


- Contraintes : 0..1  Optionnel  : lorsque le point appartient à un canevas donné, il est recommandé de le renseigner.

### Code INSEE ###

- Définition : Code INSEE de la commune.


- Type : CharacterString.


- Contraintes : 1.

### Complément ###

- Définition : Information complémentaire liée au type d'emprise de publication du PCRS, gérée par le gestionnaire  du PCRS et potentiellement à tout utilisateur du PCRS.


- Type : CharacterString.


- Valeurs possibles : Selon le type d'emprise de publication, par exemple :


   - un toponyme pour une emprise de type couloir.

   - le nom de l'opération pour une emprise de concernant une opération donnée,

   - la référence du carreau (si elle n'est pas redondante avec l'identifiant de l'emprise), ou le nom du carroyage pour une emprise de type régulière,

   - le nom ou le type de la limite administrative pur une emprise de type administrative ...


- Contraintes : 0..1 Optionnel : information en complément de l'identifiant d'emprise, et liée au type de l'emprise de publication devant être renseignée si gérée par le gestionnaire du PCRS.

### Date Création ###

- Définition : Date de création ou de mise à jour des données du point de canevas.


- Type : Date au format (aaaa-mm-jj).


- Contraintes : 0..1  Optionnel  : lorsque la date de création ou de mise à jour des données du point de canevas est connue, il est obligatoire de la renseigner.

### Date de Publication ###

- Définition : Date de mise à disposition de l'emprise du PCRS.


- Type : Date au format (aaaa-mm-jj).


- Contraintes : 1.

### Fiche ###

- Définition : Adresse de type URL susceptible de fournir des informations supplémentaires, comme des photographies de repérage,  sur le point de canevas.


- Type : URL.


- Contraintes : 0..1.

### Fournisseur ###

### Gestionnaire ###

1- Emprise d'échange du PCRS

- Définition : Nom de la collectivité gestionnaire du PCRS.


- Type : CharacterString.


- Contraintes : 1.


2- Affleurant du PCRS

- Définition : Nom court, sigle, acronyme de l'opérateur gestionnaire du réseau et fournisseur de la donnée.


- Type : CharacterString.


- Valeurs possibles : Exemple : ENEDIS, GRDF, Lyonnaise des Eaux, ...


- Contraintes : 0..1.

### Horodatage ###

- Définition : Horodatage du point au moment du levé topographique.


- Type : Date.


- Contraintes : 0..1 Optionnel : pour la reprise de données existantes, lorsque l'horodatage du point levé est connu, il est obligatoire de le renseigner.

### Identifiant Affleurant Symbole ###

- Définition : Lien vers une représentation symbolique.


- Type : Classe d'objets AffleurantSymbolePCRS.


- Contraintes 0..1.

### Identifiant Emprise ###

- Définition : Identifiant de l'emprise.


- Type : CharacterString.


- Contraintes : 1.

### Identifiant Habillage ###

- Définition : Identifiant unique de l'habillage.


- Type : CharacterString.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et le cas échéant lié à celui du référentiel dont peut-être issue la donnée.


- Contraintes : 1 Valeur non vide et unique pour un même jeu de données.

### Identifiant Habillage Symbole ###

Identifiant unique de l'habillage symbole.

### Identifiant Objet ###

- Définition : Identifiant unique dans le jeu de données des objets du PCRS.


- Type : CharacterString.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS.


- Contraintes : 1 Valeur unique.

### Identifiant PCRS ###

Les identifiants PCRS sont obligatoirement renseignés. Ils sont calculés par défaut dans le projet FME.

### Identifiant Source ###

- Définition : Identifiant unique de l'affleurants.


- Type : CharacterString.


- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux.


- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Immatriculation ###

- Définition : Référence externe selon la convention d'immatriculation du canevas considéré.


- Type : CharacterString.


- Contraintes : 0..1  Optionnel  : lorsque le matricule du point est connu, il est obligatoire de le renseigner.

### Justification ###

- Définition : Utilisé pour la justification de texte.


- Type : TexteJustificationPCRSType.


- Valeurs possibles :

  - G = Gauche,

  - C = Centré,

  - D = Droite.


- Contraintes : 1.

### Largeur ###

- Définition : Utilisé pour la mise à l'échelle Y du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.


- Type : Décimal.


- Contraintes : 1 Valeur non vide.

### Libellé ###

- Définition : Texte du libellé à utiliser comme habillage du PCRS.


- Type : CharacterString.


- Valeurs possibles : Valeur textuelle. Exemple : 123 m.


- Contraintes : 1.

### Longueur ###

- Définition : Utilisé pour la mise à l'échelle X du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.


- Type : Décimal.


- Contraintes : 1 Valeur non vide.

### Nature ###

- Définition : Nature de l'affleurant.


- Type : NatureAffleurantPCRSType.


- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux


  - 01 = avaloirs,

  - 02 = Boîte, Coffret, Armoire,

  - 03 = Tampon, plaque, chambre,

  - 04 = Branchement, vanne, bouche à clé,

  - 05 = Bouche incendie, Poteau incendie,

  - 06 = poteaux,

  - 07 = Poteau/borne d'éclairage.


- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Nom ###

- Définition : Nom de la commune.


- Type : CharacterString.


- Contraintes : 0..1.

### Nom voirie ###

- Définition : Identifiant unique dans le jeu de données des noms voirie.


- Type : CharacterString.


- Valeurs possibles : Selon La collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.


- Contraintes : 1 Valeur unique.

### Numéro de voirie ###

- Définition : Identifiant unique dans le jeu de données des numéros de voirie.


- Type : CharacterString.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.


- Contraintes : 1 Valeur unique.

### Numéro Point Levé ###

- Définition : Numéro(s) attribué(s) au point(s) levé(s) lors du levé topographique ou de l'intégration au référentiel (séparés par ",").


- Type : CharacterString.


- Valeurs possibles : Un ou plusieurs caractères alpha non accentués préfixant un nombre à valeurs dans une série numérique croissante avec possibilité de saut / valeurs manquantes dans la suite.


- Contraintes : 1 Valeur non vide.

### Positionnement ###

- Définition : Indication quant au positionnement de l'élément d'habillage par rapport à la voirie.


- Type : CategoriePlacementPCRSType.


- Valeurs possibles :


  - 01 = sans repositionnement,

  - 02 = AxeVoirie,

  - 03 = LimiteVoirie,

  - 04 = HorsVoirie,

  - 05 = parcelles.


- Contraintes : 0..1.

### Précision Altimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision altimétrique associée au levé topographique de l'objet.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - 002 = moins de 2 cm,

  - 005 = de 2 à 5 cm,

  - 010 = de 5 à 10 cm,

  - 040 = de 10 à 40 cm,

  - 150 = de 40 à 150 cm,

  - 999 = au delà de 150 cm.


- Contraintes : 0..1.

### Précision Planimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision planimétrique associée au levé topographique de l'objet.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - 002 = moins de 2 cm,

  - 005 = de 2 à 5 cm,

  - 010 = de 5 à 10 cm,

  - 040 = de 10 à 40 cm,

  - 150 = de 40 à 150 cm,

  - 999 = au delà de 150 cm.


- Contraintes : 1.

### Précision XY ###

- Définition : Précision planimétrique exprimée en cm.


- Type : Integer.


- Contraintes : 0..1  Optionnel, à renseigner si disponible.

### Précision Z ###

- Définition : Précision altimétrique exprimée en cm.


- Type : Integer.


- Contraintes : 0..1  Optionnel, à renseigner si disponible (ou pour les saisies nouvelles).

### Producteur ###

- Définition : Producteur de la donnée.


- Type : CharacterString.


- Valeurs possibles : La valeur sera saisie et déterminée par le producteur de façon stable. Cet attribut permettra de filtrer l'ensemble des objets d'un producteur donné.


- Contraintes : 1.

### Propriété ###

- Définition : Distinction d'appartenance  d'un tronçon de voirie à l'espace public ou à l'espace privé.


- Type : ProprieteEspaceType.


- Valeurs possibles :

  - 01 = Espace public,

  - 02 = Espace privé.


- Contraintes : 0..1 Optionnel à renseigner si possible, lorsqu'une superposition avec les données cadastrales n'est pas envisageable.

### Qualité Catégorisation ###

- Définition : Indication du producteur quant à la qualité de la catégorisation. Permet des représentations plus riches pour les migrations / reprises de données.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - 01 = Très fiable / Conforme PCRS,

  - 02 = Moyennement fiable,

  - 03 = Peu fiable.


- Contraintes : 1.

### Référence ###

1- Lien vers un objet « commune »

- Définition : Référence vers une base de données des communes.


- Type : CharacterString.


- Contraintes : 1.


2- Tronçon de Voie

- Définition : Identifiant unique du tronçon dans le référentiel source utilisé.


- Type : CharacterString.


- Valeurs possibles : Selon le fournisseur du référentiel donné.

3- Symbole d'habillage du PCRS

- Définition : Désignation du symbole à utiliser pour la représentation de l'habillage sous forme de symbole.


- Type : CharacterString.


- Contraintes : 1 Valeur non vide.


4- Affleurant du PCRS représenté par un symbole

- Définition : Désignation du symbole à utiliser pour la représentation de l'affleurant.


- Type : CharacterString.


- Contraintes : 1 Valeur non vide.

5- Arbre

- Définition : Désignation du symbole à utiliser pour la représentation de l'arbre.


- Type : CharacterString.


- Valeurs possibles : Permet le cas échéant de faire référence à des essences ou espèces d'arbres différents.


- Contraintes : 1.

### Réseau ###

- Définition : Nature du réseau.


- Type : NatureReseauPCRSType.


- Valeurs possibles :

  - ASSAEU = Eaux usées,

  - ASSARU = Réseau unitaire,

  - 00 = Non défini,

  - ASSA = Assainissement ou pluvial,

  - AEP = Eau potable,

  - ELECECL = Electricité,

  - GAZ = Gaz,

  - MULT = Multi-réseaux,

  - ELECSLT = Signalisation lumineuse tricolore,

  - COM = Télécom,

  - ASSAEP = Eaux pluviales,

  - DECH = déchets,

  - INCE = Incendie,

  - CHIM = Produits chimiques,

  - CHAU = Chauffage et climatisation.


- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Section ###

- Définition : Forme de la section à la base du pilier.


- Type : SectionPilierPCRSType.


- Valeurs possibles :

  - 01 = Pilier carré,

  - 02 = Pilier circulaire,

  - 03 = Pilier rectangulaire,

  - 00 = Pilier à autre forme de section.


- Contraintes : 1 Valeur non vide : l'attribut est utilisé pour différencier les piliers selon leur nature.

### Source ###

1- Tronçon de Voie

- Définition : Acronyme du référentiel utilisé.


- Type : CharacterString.


- Valeurs possibles : Selon le fournisseur du référentiel.


- Contraintes : 1.

2- Affleurant du PCRS

- Définition : Source de données d'affleurant dans le SI du gestionnaire de réseaux.


- Type : CharacterString.


- Valeurs possibles : Nom d'application ou de base de données dans le système d'information du gestionnaire de réseaux.


- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Taille ###

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte.


- Type : Décimal.


- Contraintes : 1.

### Thématique ###

- Définition : La thématique à laquelle est associé chaque objet du PCRS.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - 10 = Affleurant,

  - 00 = A déterminer,

  - 01 = Topographie,

  - 02 = Bâti,

  - 03 = Voirie,

  - 04 = Ferroviaire,

  - 05 = Clôture,

  - 06 = Végétal,

  - 07 = Ouvrage d'art,

  - 08 = Hydrographie,

  - 09 = Orographie,

  - 99 = Non définie.


- Contraintes : 1 en général à valeur unique par classe d'objet dérivé.

### Transparence ###

- Définition : Pourcentage de transparence inversement proportionnelle à l'opacité de la zone.


- Type : Integer.


- Valeurs possibles : de 0 à 100.


- Contraintes : 1.

### Type ###

- Définition : Type d'emprise du PCRS.


- Type : CharacterString.


- Valeurs possibles : Par exemple : Couloir, Opération, Carreau, LimiteAdministrative.


- Contraintes : 0..1.

### Type Mur ###

- Définition : Description des ouvrages de maçonnerie s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces.


- Type : CategorieMurPCRSType.


- Contraintes : 0..1.
