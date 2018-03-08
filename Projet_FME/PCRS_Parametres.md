# Paramètres des Transformers #

### Angle de rotation ###

- Définition : Utilisé pour l'orientation de l'élément d'habillage, du symbole de poteau (pouvant être étendu pour un poteau ovale pour orienter le symbole) et du symbole d'affleurant, dans le sens horaire par rapport au nord.


- Type : Décimal.


- Valeurs possibles : Valeur angulaire en degrés décimaux.

### Canevas ###

- Définition : Type de canevas auquel appartient le point considéré.


- Type : Chaîne de caractères.


- Paramètre optionnel.

### Code INSEE ###

- Définition : Code INSEE de la commune.


- Type : Chaîne de caractères.

### Complément ###

- Définition : Information complémentaire liée au type d'emprise de publication du PCRS, gérée par le gestionnaire  du PCRS et potentiellement à tout utilisateur du PCRS.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon le type d'emprise de publication, par exemple :


   - un toponyme pour une emprise de type couloir.

   - le nom de l'opération pour une emprise de concernant une opération donnée,

   - la référence du carreau (si elle n'est pas redondante avec l'identifiant de l'emprise), ou le nom du carroyage pour une emprise de type régulière,

   - le nom ou le type de la limite administrative pur une emprise de type administrative ...


- Paramètre optionnel.

### Date Création ###

- Définition : Date de création ou de mise à jour des données du point de canevas.


- Type : Date au format (aaaa-mm-jj).


- Paramètre optionnel.

### Date de Publication ###

- Définition : Date de mise à disposition de l'emprise du PCRS.


- Type : Date au format (aaaa-mm-jj).

### Emplacement du schéma PCRS ###

- Définition : Emplacement du schéma d'application de l'espace de nommage http://cnig.gouv.fr/pcrs. 
Cette valeur est utilisée pour alimenter l'attribut xsi:schemaLocation dans l'entête du fichier GML généré. L'emplacement du schéma d'application est utilisé pour assurer la validation du jeu de données. 

Il peut être défini par une uri (http://schemas.veremes.net/pcrs/CNIG_PCRS_v2.0.xsd), un emplacement local absolu ("file:///c:/xsd/CNIG_PCRS_v2.0.xsd") ou relatif (./xsd/CNIG_PCRS_v2.0.xsd). 

Le CNIG n'ayant pas défini d'emplacement officiel pour le schéma d'application PCRS, Veremes propose l'uri http://schemas.veremes.net/pcrs/CNIG_PCRS_v2.0.xsd.


- Type : Domaine de valeurs ou chaîne de caractères


- Valeurs proposées :

  - http://schemas.veremes.net/pcrs/CNIG_PCRS_v2.0.xsd,

  - CNIG_PCRS_v2.0.xsd.

### Fiche ###

- Définition : Adresse de type URL susceptible de fournir des informations supplémentaires, comme des photographies de repérage,  sur le point de canevas.


- Type : URL.


- Paramètre optionnel.

### Fournisseur ###

- Définition : Nom de la collectivité gestionnaire du PCRS.


- Type : Chaîne de caractères.

### Gestionnaire ###

- Définition : Nom court, sigle, acronyme de l'opérateur gestionnaire du réseau et fournisseur de la donnée.


- Type : Chaîne de caractères.


- Valeurs possibles : Exemple : ENEDIS, GRDF, Lyonnaise des Eaux, ...


- Paramètre optionnel.

### Horodatage ###

- Définition : Horodatage du point au moment du levé topographique.


- Type : Date.


- Paramètre optionnel.

### Identifiant Affleurant Symbole ###

- Définition : Lien vers une représentation symbolique.


- Type : Chaîne de caractères.


- Paramètre optionnel.

### Identifiant Emprise ###

- Définition : Identifiant de l'emprise.


- Type : Chaîne de caractères.

### Identifiant Habillage ###

- Définition : Identifiant unique de l'habillage.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et le cas échéant lié à celui du référentiel dont peut-être issue la donnée.

### Identifiant Objet ###

- Définition : Identifiant unique dans le jeu de données des objets du PCRS.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS.

### Identifiant PCRS ###

Les identifiants PCRS sont obligatoirement renseignés. Ils sont calculés par défaut dans le projet FME.

### Identifiant Source ###

- Définition : Identifiant unique de l'affleurant.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux.


- Paramètre optionnel.

### Immatriculation ###

- Définition : Référence externe selon la convention d'immatriculation du canevas considéré.


- Type : Chaîne de caractères.


- Paramètre optionnel.

### Justification ###

- Définition : Utilisé pour la justification de texte.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Gauche,

  - Centré,

  - Droite.

### Largeur ###

- Définition : Utilisé pour la mise à l'échelle Y du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.


- Type : Décimal.

### Libellé ###

- Définition : Texte du libellé à utiliser comme habillage du PCRS.


- Type : Chaîne de caractères.


- Valeurs possibles : Valeur textuelle. Exemple : 123 m.

### Longueur ###

- Définition : Utilisé pour la mise à l'échelle X du symbole habillage, du symbole de l'affleurant et du symbole de poteau après rotation.


- Type : Décimal.

### Nature ###

- Définition : Nature de l'affleurant.


- Type : Domaine de Valeurs.


- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux

  - Avaloirs,

  - Boîte, Coffret, Armoire,

  - Tampon, Plaque, Chambre,

  - Branchement, Vanne, Bouche à clé,

  - Bouche incendie, Poteau incendie,

  - Poteau,

  - Poteau d'éclairage.


- Paramètre optionnel.

### Nom ###

- Définition : Nom de la commune.


- Type : Chaîne de caractères.

### Nom voirie ###

- Définition : Identifiant unique dans le jeu de données des noms voirie.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon La collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.

### Numéro de voirie ###

- Définition : Identifiant unique dans le jeu de données des numéros de voirie.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon la collectivité gestionnaire du PCRS, et si possible identique à celui du référentiel dont est issu la donnée.

### Numéro Point Levé ###

- Définition : Numéro(s) attribué(s) au point(s) levé(s) lors du levé topographique ou de l'intégration au référentiel (séparés par ",").


- Type : Chaîne de caractères.


- Valeurs possibles : Un ou plusieurs caractères alpha non accentués préfixant un nombre à valeurs dans une série numérique croissante avec possibilité de saut / valeurs manquantes dans la suite.

### Positionnement ###

- Définition : Indication quant au positionnement de l'élément d'habillage par rapport à la voirie.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Sans repositionnement,

  - Axe voirie,

  - Limite voirie,

  - Hors voirie,

  - Parcelle.


- Paramètre optionnel.

### Précision Altimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision altimétrique associée au levé topographique de l'objet.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Moins de 2 cm,

  - De 2 à 5 cm,

  - De 5 à 10 cm,

  - De 10 à 40 cm,

  - De 40 à 150 cm,

  - Au delà de 150 cm.


- Paramètre optionnel.

### Précision Planimétrique ###

- Définition : Intervalle de précision dans lequel s'exprime en cm la précision planimétrique associée au levé topographique de l'objet.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Moins de 2 cm,

  - De 2 à 5 cm,

  - De 5 à 10 cm,

  - De 10 à 40 cm,

  - De 40 à 150 cm,

  - Au delà de 150 cm.

### Précision XY ###

- Définition : Précision planimétrique exprimée en cm.


- Type : Entier.


- Paramètre optionnel.

### Précision Z ###

- Définition : Précision altimétrique exprimée en cm.


- Type : Entier.


- Paramètre optionnel.

### Producteur ###

- Définition : Producteur de la donnée.


- Type : Chaîne de caractères.


- Valeurs possibles : La valeur sera saisie et déterminée par le producteur de façon stable. Cet attribut permettra de filtrer l'ensemble des objets d'un producteur donné.

### Propriété ###

- Définition : Distinction d'appartenance  d'un tronçon de voirie à l'espace public ou à l'espace privé.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Espace Public,

  - Espace Privé.


- Paramètre optionnel.

### Qualité Catégorisation ###

- Définition : Indication du producteur quant à la qualité de la catégorisation. Permet des représentations plus riches pour les migrations / reprises de données.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Très fiable / Conforme PCRS,

  - Moyennement fiable,

  - Peu fiable.

### Référence ###

1- Lien vers un objet « commune »

- Définition : Référence vers une base de données des communes.


- Type : Chaîne de caractères.


2- Tronçon de Voie

- Définition : Identifiant unique du tronçon dans le référentiel source utilisé.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon le fournisseur du référentiel donné.


3- Symbole d'habillage du PCRS

- Définition : Désignation du symbole à utiliser pour la représentation de l'habillage sous forme de symbole.


- Type : Chaîne de caractères.


4- Affleurant du PCRS représenté par un symbole

- Définition : Désignation du symbole à utiliser pour la représentation de l'affleurant.


- Type : Chaîne de caractères.


5- Arbre

- Définition : Désignation du symbole à utiliser pour la représentation de l'arbre.


- Type : Chaîne de caractères.


- Valeurs possibles : Permet le cas échéant de faire référence à des essences ou espèces d'arbres différents.

### Réseau ###

- Définition : Nature du réseau.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Eaux usées,

  - Réseau unitaire,

  - Non défini,

  - Assainissement et pluvial,

  - Eau potable,

  - Electricité,

  - Eclairage public,

  - Signalisation lumineuse tricolore,

  - Electricité basse tension,

  - Electricité haute tension,

  - Gaz,

  - Multi-réseaux,

  - ELECSLT = Signalisation lumineuse tricolore,

  - Télécom,

  - Eaux pluviales,

  - Déchets,

  - Incendie,

  - Produits chimiques,

  - Chauffage et climatisation.


- Paramètre optionnel.

### Section ###

- Définition : Forme de la section à la base du pilier.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Pilier carré,

  - Pilier circulaire,

  - Pilier rectangulaire,

  - Pilier à autre forme de section.

### Source ###

1- Tronçon de Voie

- Définition : Acronyme du référentiel utilisé.


- Type : Chaîne de caractères.


- Valeurs possibles : Selon le fournisseur du référentiel.

2- Affleurant du PCRS

- Définition : Source de données d'affleurant dans le SI du gestionnaire de réseaux.


- Type : Chaîne de caractères.


- Valeurs possibles : Nom d'application ou de base de données dans le système d'information du gestionnaire de réseaux.


- Paramètre optionnel.

### Taille ###

- Définition : Facteur de taille permettant le cas échéant aux utilisateurs de pondérer la taille du Texte.


- Type : Décimal.

### Thématique ###

- Définition : La thématique à laquelle est associé chaque objet du PCRS.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Affleurant,

  - A déterminer,

  - Topo,

  - Bâti,

  - Voirie,

  - Ferroviaire,

  - Clôture,

  - Végétal,

  - Ouvrage d'art,

  - Hydrographie,

  - Orographie,

  - Raster,

  - Non définie.

### Transparence ###

- Définition : Pourcentage de transparence inversement proportionnelle à l'opacité de la zone.


- Type : Entier.


- Valeurs possibles : de 0 à 100.

### Type ###

- Définition : Type d'emprise du PCRS.


- Type : Chaîne de caractères.


- Valeurs possibles : Par exemple : Couloir, Opération, Carreau, LimiteAdministrative.


- Paramètre optionnel.

### Type Mur ###

- Définition : Description des ouvrages de maçonnerie s'élevant en hauteur et servant à enclore, séparer ou délimiter des espaces.


- Type : Domaine de valeurs.


- Valeurs possibles :

  - Mur,

  - Mur de soutènement,

  - Mur bahut,

  - Mur bahut avec cloture,

  - Parapet,

  - Enrochement.

### XML Fragments ###

- Définition : Fragments XML à fusionner dans un attribut.


- Valeur par défaut : _pcrs.xml_formatted.
