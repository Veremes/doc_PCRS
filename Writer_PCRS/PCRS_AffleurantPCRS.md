# AffleurantPCRS #



**Nom de la classe**

AffleurantPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Affleurant du PCRS

**Définition**

Classe permettant de décrire une partie d'un réseau existant visible depuis la surface.
IMPORTANT : un affleurant de réseau correspond à un objet métier géré non pas par la collectivité gestionnaire du PCRS mais par l'opérateur gestionnaire du réseau. Il figure toutefois dans la liste des objets échangés dans un PCRS de façon à partager la localisation précise de tous les objets d'un réseau visibles depuis la surface. Chaque gestionnaire reste responsable de ses affleurants.

**Modélisation**

Selon les classes d'affleurant spécialisées, et représentées (de préférence) par une représentation exhaustive et intéropérable comme le polygone AffleurantEnveloppePCRS, éventuellement complété par un habillage de type HabillageLignesPCRS, néanmoins d'autres modélisation géométriques sont offertes afin de ne pas perdre d'informations. La modélisation géométrique est propre à chacune des classes d'affleurant spécialisées AffleurantXXXPCRS du PCRS.

**La classe contient**

Bouches, avaloirs, regards, plaques, poteaux, coffrets...

**Contraintes**

Classe essentielle du PCRS.

**Attributs**

*gestionnaire*

- Définition : Nom court, sigle, acronyme de l'opérateur gestionnaire du réseau et fournisseur de la donnée

- Type : CharacterString

- Valeurs possibles : Exemple : ENEDIS, GRDF, Lyonnaise des Eaux, etc

- Contraintes : 0..1

*idSource*

- Définition : Identifiant unique de l'affleurants

- Type : CharacterString

- Valeurs possibles : Selon le système d'information du gestionnaire de réseaux.

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée

*nature*

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

*reseau*

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


*source*

- Définition : Source de données d'affleurant dans le SI du gestionnaire de réseaux

- Type : CharacterString

- Valeurs possibles : Nom d'application ou de base de données dans le système d'information du gestionnaire de réseaux

- Contraintes : 0..1 Optionnel : selon les données entretenues par le gestionnaire de réseau concerné, cette valeur doit si possible être renseignée

*symbolisation*

- Définition : Lien vers une représentation symbolique

- Type : Classe d'objets AffleurantSymbolePCRS

- Contraintes 0..1

*representations*

- Définition : Liens vers une représentation de type géométrique

- Type : Classe d'objets AffleurantGeometriquePCRS

- Contraintes : 1 Il est nécessaire de fournir au moins un type de représentation géométrique

**Paramètres**

![Identifiant PCRS](Parametres.html#Identifiant PCRS_PCRS.ID)

![Identifiant Objet](Parametres.html#Identifiant Objet_PCRS.IDOBJET)

![Thématique](Parametres.html#Thématique_PCRS.THEMATIQUE)

![Qualité Catégorisation](Parametres.html#Qualité Catégorisation_PCRS.QUALITECATEGORISATION)

![Précision Planimetrique](Parametres.html#Précision Planimetrique PRECISIONPLANIMETRIQUE)   

![Précision Altimétrique](Parametres.html#Précision Altimétrique_PCRS.PRECISIONALTIMETRIQUE)

![Producteur](Parametres.html#Producteur_PCRS.PRODUCTEUR)

![Numero(s) des Point(s) Levé(s) (séparés par ",")](Parametres.html#Numero(s) des Point(s) Levé(s) (séparés par ",")_PCRS.NUMEROPOINT)

![Gestionnaire](Parametres.html#Gestionnaire_PCRS.GESTIONNAIRE)

![Identifiant Source](Parametres.html#Identifiant Source_PCRS.IDSOURCE)

![Nature](Parametres.html#Nature_PCRS.NATURE)

![Reseau](Parametres.html#Reseau_PCRS.RESEAU)

![Source](Parametres.html#Source_PCRS.SOURCE)

![Identifiant Affleurant Symbole](Parametres.html#Identifiant Affleurant Symbole_PCRS.IDAFFLEURANTSYMBOLE)