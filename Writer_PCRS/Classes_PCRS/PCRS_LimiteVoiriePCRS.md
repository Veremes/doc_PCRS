# PCRS_LimiteVoiriePCRS #



**Nom de la classe**

LimiteVoiriePCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Limite de voirie

**Définition**

Toute limite apparente de la chaussée, caractérisée par une bordure ou un changement de revêtement est décrite par un objet de cette classe.  

**Modélisation**

Polyligne <br>
Les changements de revêtement sont levés point à point au niveau du sol.
Les quais, bordures, bordurettes... qui marquent la limite de la chaussée sont levés point à point, le long du fil d'eau uniquement. Pour les nouveaux levés, il est conseillé de laisser l’objet à gauche.
Les autres aspects de la modélisation géométrique sont propres à  ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS.

**La classe contient**

Limites de chaussée revêtue, marquant la limite de la voirie (exemple un bord goudronné).

**Géométrie**

- Définition : Géométrie de type courbe.

- Type : GM_Curve.

**Paramètres**

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
