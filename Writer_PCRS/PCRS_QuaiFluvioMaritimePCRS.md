# QuaiFluvioMaritimePCRS #



**Nom de la classe**

QuaiFluvioMaritimePCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Quais fluvio-maritimes

**Définition**

Ouvrage le long de berge, de rive ou de rivage d'un port ou d'une voie navigable, aménagée en vue de permettre l'accostage des bâtiments de navigation, l'embarquement ou le débarquement des passagers, le chargement ou le déchargement des marchandises.  

**Modélisation**

Polyligne Les quais sont levés au nez du quai. Les autres aspects de la modélisation géométrique sont propres à  ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS.

**La classe contient**
- Quais    

**Contraintes**

Classe essentielle du PCRS

**Attributs**

*géométrie*

- Définition : Géométrie de quai

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|QUALITECATEGORISATION|
|Précision Planimetrique|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|_PCRS.PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
