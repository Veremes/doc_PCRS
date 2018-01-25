**Nom de la classe**

PointLevePCRS

**Titre**

Point levé du PCRS

**Définition**

Point géoréférencé en planimétrie, ou planimétrie et altimétrie du PCRS

**Modélisation**

Point La modélisation géométrique par point(s) est propre à chacun des objets du PCRS, elle sera donc décrite dans la partie du catalogue propre à chacun des objets dérivés de la classe ObjetVecteurPCRS (paragraphes B.3.17 à B.3.31)

**La classe contient**

De façon non limitative, tout point situé le long ou sur le pourtour d'un objet du PCRS peut être décrit par cette classe d'objet, par exemple :
- Point le long d'un fil d'eau  
- Point d'une limite apparente  
- Point d'amorce de bâti  
- Point de seuil  
- Point de rupture de pente  
- Point le long d'un rail  
- Point associé à un dénivelé d'escalier ou de marche d'escalier  
- Par extension, tout point utile issu d'un lever Mobile Mapping (nuages de points LIDAR, vues immersives...).  

**Contraintes**

Un point levé doit être topologiquement inclus dans l'emprise du levé topographique. Les points peu précis n'ont pas à figurer dans les données échangées du PCRS.

**Critères de sélection**

Tout point servant à qualifier un objet du PCRS en tant que support pour une cotation des réseaux en classe A (planimétrie et altimétrie) ou en classe AP (planimétrie seulement) au sens DT-DICT.

**Attributs**

*géométrie*

- Définition : Géométrie de type ponctuel

- Type : GM_Point

- Contraintes : 1

*horodatage*

- Définition : Horodatage du point au moment du levé topographique

- Type : Date

- Contraintes : 0..1 Optionnel : pour la reprise de données existantes, lorsque l'horodatage du point levé est connu, il est obligatoire de le renseigner

*numeroPoint*

- Définition : Numéro attribué au point levé lors du levé topographique ou de l' intégration au référentiel selon une ou plusieurs méthodologies à préciser si possible dans les métadonnées

- Type : CharacterString

- Valeurs possibles : Un ou plusieurs caractères alpha non accentués préfixant un nombre à valeurs dans une série numérique croissante avec possibilité de saut / valeurs manquantes dans la suite

- Contraintes : 1 Valeur non vide

*precisionXY*

- Définition : Précision planimétrique exprimée en cm

- Type : Integer

- Contraintes : 1 Optionnel,

*précisionZ*

- Définition : Précision altimétrique exprimée en cm

- Type : Integer

- Contraintes : 0..1 Optionnel, à renseigner si disponible ou pour les saisies nouvelles

*producteur*

- Définition : Producteur de la donnée

- Type :CharacterString

- Valeurs possibles : La valeur sera saisie et déterminée par le producteur de façon stable. Cet attribut permettra de filtrer l'ensemble des objets d'un producteur donné .

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS (obligatoire):|_PCRS.ID|
|Numero Point:|_PCRS.NUMEROPOINT|
|Précision Planimétrique:|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique:|_PCRS.PRECISIONALTIMETRIQUE|
|Horodatage:|_PCRS.HORODATAGE|
