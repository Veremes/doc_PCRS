# Paramètres publiés #

### Angle de rotation ###

- Définition : Utilisé pour l'orientation de l'élément d'habillage, du symbole de poteau (pouvant être étendu pour un poteau ovale pour orienter le symbole) et du symbole d'affleurant, dans le sens horaire par rapport au nord.<br>

- Type : Décimal.<br>

- Valeurs possibles : Valeur angulaire en degrés décimaux.<br>

- Contraintes : 1 valeur non vide.

### Canevas ###

- Définition : Type de canevas auquel appartient le point considéré.<br>

- Type : CharacterString.<br>

- Contraintes : 0..1  Optionnel  : lorsque le point appartient à un canevas donné, il est recommandé de le renseigner.

### Code INSEE ###

- Définition : Code INSEE de la commune.<br>

- Type : CharacterString.<br>

- Contraintes : 1.

### Complément ###

- Définition : Information complémentaire liée au type d'emprise de publication du PCRS, gérée par le gestionnaire  du PCRS et potentiellement à tout utilisateur du PCRS.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon le type d'emprise de publication, par exemple :<br>

   - un toponyme pour une emprise de type couloir.
   - le nom de l'opération pour une emprise de concernant une opération donnée,
   - la référence du carreau (si elle n'est pas redondante avec l'identifiant de l'emprise), ou le nom du carroyage pour une emprise de type régulière,
   - le nom ou le type de la limite administrative pur une emprise de type administrative ...<br>

- Contraintes : 0..1 Optionnel : information en complément de l'identifiant d'emprise, et liée au type de l'emprise de publication devant être renseignée si gérée par le gestionnaire du PCRS.

### Date Création ###

- Définition : Date de création ou de mise à jour des données du point de canevas.<br>

- Type : Date au format (aaaa-mm-jj).<br>

- Contraintes : 0..1  Optionnel  : lorsque la date de création ou de mise à jour des données du point de canevas est connue, il est obligatoire de la renseigner.

### Date de Publication ###

- Définition : Date de mise à disposition de l'emprise du PCRS.<br>

- Type : Date au format (aaaa-mm-jj).<br>

- Contraintes : 1.

### Fiche ###

- Définition : Adresse de type URL susceptible de fournir des informations supplémentaires, comme des photographies de repérage,  sur le point de canevas.<br>

- Type : URL.<br>

- Contraintes : 0..1.

### Fournisseur ###

### Gestionnaire ###

1) Emprise d'échange du PCRS<br>

- Définition : Nom de la collectivité gestionnaire du PCRS.<br>

- Type : CharacterString.<br>

- Contraintes : 1.


2) Affleurant du PCRS

- Définition : Nom court, sigle, acronyme de l'opérateur gestionnaire du réseau et fournisseur de la donnée.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Exemple : ENEDIS, GRDF, Lyonnaise des Eaux, ...<br>

- Contraintes : 0..1.

### Horodatage ###

- Définition : Horodatage du point au moment du levé topographique.<br>

- Type : Date.<br>

- Contraintes : 0..1 Optionnel : pour la reprise de données existantes, lorsque l'horodatage du point levé est connu, il est obligatoire de le renseigner.

### Identifiant Affleurant Symbole ###

- Définition : Lien vers une représentation symbolique.<br>

- Type : Classe d'objets AffleurantSymbolePCRS.<br>

- Contraintes 0..1.

### Identifiant Emprise ###

- Définition : Identifiant de l'emprise.<br>

- Type : CharacterString.<br>

- Contraintes : 1.

### Identifiant Habillage ###

- Définition : Identifiant unique de l'habillage.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et le cas échéant lié à celui du référentiel dont peut-être issue la donnée.<br>

- Contraintes : 1 Valeur non vide et unique pour un même jeu de données.

### Identifiant Habillage Symbole ###

Identifiant unique de l'habillage symbole.

### Identifiant Objet ###

- Définition : Identifiant unique dans le jeu de données des objets du PCRS.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon la collectivité gestionnaire du PCRS.<br>

- Contraintes : 1 Valeur unique.

### Identifiant PCRS ###

Les identifiants PCRS sont obligatoirement renseignés. Ils sont calculés par défaut dans le projet FME.

### Identifiant Source ###

- Définition : Identifiant unique de l'affleurants.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux.<br>

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Immatriculation ###

- Définition : Référence externe selon la convention d'immatriculation du canevas considéré.<br>

- Type : CharacterString.<br>

- Contraintes : 0..1  Optionnel  : lorsque le matricule du point est connu, il est obligatoire de le renseigner.

### Justification ###

- Définition : Utilisé pour la justification de texte.<br>

- Type : TexteJustificationPCRSType.<br>

- Valeurs possibles :<br>
  - G = Gauche,
  - C = Centré,
  - D = Droite.<br>

- Contraintes : 1.

### Largeur ###

- Définition : Utilisé pour la mise à l'échelle Y du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.<br>

- Type : Décimal.<br>

- Contraintes : 1 Valeur non vide.

### Libellé ###

- Définition : Texte du libellé à utiliser comme habillage du PCRS.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Valeur textuelle. Exemple : 123 m.<br>

- Contraintes : 1.

### Longueur ###

- Définition : Utilisé pour la mise à l'échelle X du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.<br>

- Type : Décimal.<br>

- Contraintes : 1 Valeur non vide.

### Nature ###

- Définition : Nature de l'affleurant.<br>

- Type : NatureAffleurantPCRSType.<br>

- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux<br>

  - 01 = avaloirs,
  - 02 = Boîte, Coffret, Armoire,
  - 03 = Tampon, plaque, chambre,
  - 04 = Branchement, vanne, bouche à clé,
  - 05 = Bouche incendie, Poteau incendie,
  - 06 = poteaux,
  - 07 = Poteau/borne d'éclairage.<br>

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Nom ###

- Définition : Nom de la commune.<br>

- Type : CharacterString.<br>

- Contraintes : 0..1.

### Nom voirie ###

- Définition : Identifiant unique dans le jeu de données des noms voirie.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon La collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.<br>

- Contraintes : 1 Valeur unique.

### Numéro de voirie ###

- Définition : Identifiant unique dans le jeu de données des numéros de voirie.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.<br>

- Contraintes : 1 Valeur unique.

### Numéro Point Levé ###

- Définition : Numéro(s) attribué(s) au point(s) levé(s) lors du levé topographique ou de l'intégration au référentiel (séparés par ",").<br>

- Type : CharacterString.<br>

- Valeurs possibles : Un ou plusieurs caractères alpha non accentués préfixant un nombre à valeurs dans une série numérique croissante avec possibilité de saut / valeurs manquantes dans la suite.<br>

- Contraintes : 1 Valeur non vide.

### Positionnement ###

- Définition : Indication quant au positionnement de l'élément d'habillage par rapport à la voirie.<br>

- Type : CategoriePlacementPCRSType.<br>

- Valeurs possibles :<br>

  - 01 = sans repositionnement,
  - 02 = AxeVoirie,
  - 03 = LimiteVoirie,
  - 04 = HorsVoirie,
  - 05 = parcelles.<br>

- Contraintes : 0..1.

### Précision Altimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision altimétrique associée au levé topographique de l'objet.<br>

- Type : Domaine de valeurs.<br>

- Valeurs possibles :<br>

  - 002 = moins de 2 cm,
  - 005 = de 2 à 5 cm,
  - 010 = de 5 à 10 cm,
  - 040 = de 10 à 40 cm,
  - 150 = de 40 à 150 cm,
  - 999 = au delà de 150 cm.<br>

- Contraintes : 0..1.

### Précision Planimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision planimétrique associée au levé topographique de l'objet.<br>

- Type : Domaine de valeurs.<br>

- Valeurs possibles :<br>

  - 002 = moins de 2 cm,
  - 005 = de 2 à 5 cm,
  - 010 = de 5 à 10 cm,
  - 040 = de 10 à 40 cm,
  - 150 = de 40 à 150 cm,
  - 999 = au delà de 150 cm.<br>

- Contraintes : 1.

### Précision XY ###

- Définition : Précision planimétrique exprimée en cm.<br>

- Type : Integer.<br>

- Contraintes : 0..1  Optionnel, à renseigner si disponible.

### Précision Z ###

- Définition : Précision altimétrique exprimée en cm.<br>

- Type : Integer.<br>

- Contraintes : 0..1  Optionnel, à renseigner si disponible (ou pour les saisies nouvelles).

### Producteur ###

- Définition : Producteur de la donnée.<br>

- Type : CharacterString.<br>

- Valeurs possibles : La valeur sera saisie et déterminée par le producteur de façon stable. Cet attribut permettra de filtrer l'ensemble des objets d'un producteur donné.<br>

- Contraintes : 1.

### Propriété ###

- Définition : Distinction d'appartenance  d'un tronçon de voirie à l'espace public ou à l'espace privé.<br>

- Type : ProprieteEspaceType.<br>

- Valeurs possibles :<br>

  - 01 = Espace public,
  - 02 = Espace privé.<br>

- Contraintes : 0..1 Optionnel à renseigner si possible, lorsqu'une superposition avec les données cadastrales n'est pas envisageable.<br>

### Qualité Catégorisation ###

- Définition : Indication du producteur quant à la qualité de la catégorisation. Permet des représentations plus riches pour les migrations / reprises de données.<br>

- Type : Domaine de valeurs.<br>

- Valeurs possibles :<br>

  - 01 = Très fiable / Conforme PCRS,
  - 02 = Moyennement fiable,
  - 03 = Peu fiable.<br>

- Contraintes : 1.

### Référence ###

1) Lien vers un objet « commune »<br>

- Définition : Référence vers une base de données des communes.<br>

- Type : CharacterString.<br>

- Contraintes : 1.<br>

2) Tronçon de Voie

- Définition : Identifiant unique du tronçon dans le référentiel source utilisé.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon le fournisseur du référentiel donné.

3) Symbole d'habillage du PCRS

- Définition : Désignation du symbole à utiliser pour la représentation de l'habillage sous forme de symbole.<br>

- Type : CharacterString.<br>

- Contraintes : 1 Valeur non vide.

4) Affleurant du PCRS représenté par un symbole

- Définition : Désignation du symbole à utiliser pour la représentation de l'affleurant.<br>

- Type : CharacterString.<br>

- Contraintes : 1 Valeur non vide.

5) Arbre

- Définition : Désignation du symbole à utiliser pour la représentation de l'arbre.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Permet le cas échéant de faire référence à des essences ou espèces d'arbres différents.<br>

- Contraintes : 1.

### Réseau ###

- Définition : Nature du réseau.<br>

- Type : NatureReseauPCRSType.<br>

- Valeurs possibles :<br>

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
  - CHAU = Chauffage et climatisation.<br>

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Section ###

- Définition : Forme de la section à la base du pilier.<br>

- Type : SectionPilierPCRSType.<br>

- Valeurs possibles :<br>

  - 01 = Pilier carré,
  - 02 = Pilier circulaire,
  - 03 = Pilier rectangulaire,
  - 00 = Pilier à autre forme de section.<br>

- Contraintes : 1 Valeur non vide : l'attribut est utilisé pour différencier les piliers selon leur nature.<br>

### Source ###

1) Tronçon de Voie

- Définition : Acronyme du référentiel utilisé.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Selon le fournisseur du référentiel.<br>

- Contraintes : 1.

2) Affleurant du PCRS

- Définition : Source de données d'affleurant dans le SI du gestionnaire de réseaux.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Nom d'application ou de base de données dans le système d'information du gestionnaire de réseaux.<br>

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée.

### Taille ###

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte.<br>

- Type : Décimal.<br>

- Contraintes : 1.

### Thématique ###

- Définition : La thématique à laquelle est associé chaque objet du PCRS.<br>

- Type : Domaine de valeurs.<br>

- Valeurs possibles :<br>

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
  - 99 = Non définie.<br>

- Contraintes : 1 en général à valeur unique par classe d'objet dérivé.

### Transparence ###

- Définition : Pourcentage de transparence inversement proportionnelle à l'opacité de la zone.<br>

- Type : Integer.<br>

- Valeurs possibles : de 0 à 100.<br>

- Contraintes : 1.

### Type ###

- Définition : Type d'emprise du PCRS.<br>

- Type : CharacterString.<br>

- Valeurs possibles : Par exemple : Couloir, Opération, Carreau, LimiteAdministrative.<br>

- Contraintes : 0..1.

### Type Mur ###

- Définition : Description des ouvrages de maçonnerie s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces.<br>

- Type : CategorieMurPCRSType.<br>

- Contraintes : 0..1.
