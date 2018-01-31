# LimiteVoiriePCRS #



**Nom de la classe**

LimiteVoiriePCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Limite de voirie

**Définition**

Toute limite apparente de la chaussée, caractérisée par une bordure ou un changement de revêtement est décrite par un objet de cette classe.  

**Modélisation**

Polyligne
Les changements de revêtement sont levés point à point au niveau du sol.
Les quais, bordures, bordurettes... qui marquent la limite de la chaussée sont levés point à point, le long du fil d'eau uniquement. Pour les nouveaux levés, il est conseillé de laisser l’objet à gauche.
Les autres aspects de la modélisation géométrique sont propres à  ceux décrits dans la modélisation des objets linéaires de la classe abstraite ObjetVecteurPCRS.

**La classe contient**

Limites de chaussée revêtue, marquant la limite de la voirie (exemple un bord goudronné).

**Attributs**

*géométrie*

- Définition : Géométrie de type courbe

-Type : GM_Curve

- Contraintes : 1

**Paramètres**

![Identifiant PCRS](Parametres.html#Identifiant PCRS_PCRS.ID)

![Identifiant Objet](Parametres.html#Identifiant Objet_PCRS.IDOBJET)

![Thématique](Parametres.html#Thématique_PCRS.THEMATIQUE) 

![Qualité Catégorisation](Parametres.html#Qualité Catégorisation_PCRS.QUALITECATEGORISATION)

![Précision Planimetrique](Parametres.html#Précision Planimetrique_PCRS.PRECISIONPLANIMETRIQUE)

![Précision Altimétrique](Parametres.html#Précision Altimétrique_PCRS.PRECISIONALTIMETRIQUE)

![Producteur](Parametres.html#Producteur_PCRS.PRODUCTEUR)

![Numero(s) des Point(s) Levé(s) (séparés par ",")](Parametres.html#Numero(s) des Point(s) Levé(s) (séparés par ",")_PCRS.NUMEROPOINT)