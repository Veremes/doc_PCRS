# ProeminenceBatiPCRS #



**Nom de la classe**

ProeminenceBatiPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Proéminence du Bâti, Soubassement

**Définition**

Classe permettant de décrire l'ensemble des constructions liées au bâtiment, dont l'emprise est différente de celle levée par les façades (AIVF_19_8), et levée au niveau du trottoir.

**Modélisation**

Polyligne La proéminence du bâti est levée point par point au niveau du trottoir et au sens de l'emprise maximum du bâtiment sur le domaine public.
Les autres aspects de la modélisation géométrique sont propres à  ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS.

**La classe contient**

Perron, marche de maison
Terrasse - Devanture
Véranda

**Critères de sélection**

Ne comprend pas les caves.

**Attributs**

*géométrie*

- Définition : Géométrie de type courbe

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

| Libellé | Paramètre |
| ---------|:-------------|
|Identifiant PCRS|_PCRS.ID|
|Identifiant Objet|_PCRS.IDOBJET|
|Thématique|_PCRS.THEMATIQUE|
|Qualité Catégorisation|_PCRS.QUALITECATEGORISATION|
|Précision Planimetrique|_PCRS.PRECISIONPLANIMETRIQUE|
|Précision Altimétrique|_PCRS.PRECISIONALTIMETRIQUE|
|Producteur|_PCRS.PRODUCTEUR|
|Numero(s) des Point(s) Levé(s) (séparés par ",")|_PCRS.NUMEROPOINT|
