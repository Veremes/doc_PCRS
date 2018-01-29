# EmpriseEchangePCRS #



**Nom de la classe**

EmpriseEchangePCRS  

**Titre**

Emprise d'échange du PCRS

**Définition**

Une emprise d'échange du PCRS constitue un élément surfacique de délimitation de l'espace public, et lorsque disponible de l'espace privé. Elle est localisée sur une commune, et peut être qualifiée par les tronçons de voirie concernés.
Une emprise d'échange du PCRS permet d'accéder à l'ensemble des éléments constituant le PCRS, et sert en particulier à repérer les objets du PCRS, en général associés à une thématique et porteurs de précision, ainsi que les affleurants de réseaux de tous types.
Parmi les éléments d'habillage d'une emprise d'échange du PCRS, on distinguera en particulier les noms ainsi que les numéros de voirie devant obligatoirement figurer dans un PCRS.
Une emprise d'échange du PCRS contient également des éléments de calendrier précisant la date de publication des données concernées.
Le modèle de données prévoit la gestion de la composante image : ainsi, l'emprise d'échange du PCRS peut également être décrite par une ou plusieurs images haute ou très haute résolution éventuellement complétées d'objets vecteurs.

**Modélisation**

Surface La collectivité gestionnaire du PCRS a toute latitude quant à la définition géométrique des emprises de publication du PCRS. Il est toutefois conseillé de publier le PCRS à au moins deux niveaux complémentaires d'emprises, à savoir un niveau continu (ou régulier, fixe) et associé à un découpage régulier du territoire (comme un carroyage) et un niveau discontinu (ou irrégulier, variable) correspondant à des découpages à base d’entités (tronçons, voire communes…).

**La classe contient**

Les emprises d'échanges du PCRS peuvent suivre des logiques différentes :
- les emprises de type couloir, c'est à dire associées à un axe de voirie et définies d'une part par les limites apparentes des propriétés privées étendues perpendiculairement à l'axe de voirie d'environ 15 mètres (à adapter localement), et d'autre part en incluant les surfaces tampon associées aux amorces de voies aux intersections et sur une longueur d'environ 10 mètres (à adapter localement).

- par extension des emprises de type couloir, il est également possible d'inclure dans cette définition géométrique toute surface de l'espace public ou privé bornée par des limites apparentes de propriétés privées et n'incluant pas d'axe de voirie.
- les emprises de type opération, c'est à dire associées à une opération particulière impactant le PCRS, par exemple la pose de rails de tramway. Ce type d'emprise ne contient aucune information de gestion quant à l'opération concernée, mais permet par exemple de regrouper des emprises élémentaires de type couloir disposant de caractéristiques communes
- les emprises de type casé, liées à un carroyage particulier - les emprises de type limite administrative, permettant d'accéder à l'intégralité d'un PCRS sur une limite administrative donnée, et en particulier par commune
- les emprises de type raster, éventuellement liées à un carroyage particulier, et permettant de référencer une image à haute ou très haute résolution.

 **Contraintes**

 Classe essentielle du PCRS, accompagnant les métadonnées de publication du PCRS.

 **Attributs**

 *complément*

 - Définition : Information complémentaire liée au type d'emprise de publication du PCRS, gérée par le gestionnaire  du PCRS et potentiellement à tout utilisateur du PCRS

 - Type : CharacterString

 - Valeurs possibles : Selon le type d'emprise de publication, par exemple :
    - un toponyme pour une emprise de type couloir

    - le nom de l'opération pour une emprise de concernant une opération donnée

    - la référence du carreau (si elle n'est pas redondante avec l'identifiant de l'emprise), ou le nom du carroyage pour une emprise de type régulière

    - le nom ou le type de la limite administrative pur une emprise de type administrative ...

- Contraintes : 0..1 Optionnel : information en complément de l'identifiant d'emprise, et liée au type de l'emprise de publication devant être renseignée si gérée par le gestionnaire du PCRS

*datePublication*

- Définition : Date de mise à disposition de l'emprise du PCRS

- Type : Date

- Contraintes : 1

*gestionnaire*

- Définition : Nom de la collectivité gestionnaire du PCRS

- Type : CharacterString

- Contraintes : 1

*type*

- Définition : Type d'emprise du PCRS

- Type : CharacterString

- Valeurs possibles : Par exemple : Couloir, Opération, Carreau, LimiteAdministrative

- Contraintes : 0..1

*idEmprise*

- Définition : Identifiant de l'entreprise

- Type : CharacterString

- Contraintes : 1

*géométrie*

- Définition : Géométrie représentée par un ensemble de surface .

- Type : GM_MultiSurface

- Contraintes : 1

**Paramètres**

![Identifiant Emprise](Parametres.html#Identifiant Emprise_PCRS.IDEMPRISE)

![Complement](Parametres.html#Complement_PCRS.IDEMPRISE)

![Date de Publication](Parametres.html#Date de Publication_PCRS.DATEPUBLICATION)

![PCRS Id](Parametres.html#PCRS Id|_PCRS.ID)

![Object Id](Parametres.html#Object Id|_PCRS.OBJECT_ID)

![Fournisseur](Parametres.html#Fournisseur_PCRS.FOURNISSEUR)

![Type](Parametres.html#Type_PCRS.TYPE)