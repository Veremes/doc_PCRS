# MarcheEscalierPCRS #



**Nom de la classe**

MarcheEscalierPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Marche d'escalier

**Définition**

Classe permettant de décrire une « marche permettant de franchir une dénivellation, à dissocier des proéminences de bâtiments. A généraliser aux marches dans la voirie. » (d'après AIVF_20_1)

**Modélisation**

Polyligne <br>
Un escalier est composé d'une ou plusieurs portions, séparées par des paliers intermédiaires. Une portion est composée d'une ou plusieurs marches, et un symbole peut être attaché à chaque portion d'escalier. Les paliers intermédiaires peuvent si besoin être décrits au moyen des dernières marches de chaque portion d'escalier.
Les rampes d’accès sont levées aux ruptures de pentes.  

**La classe contient**

Les escaliers du PCRS peuvent se retrouver dans deux thématiques, le bâti et la voirie Dans tous les cas, il s'agit d'escaliers extérieurs, et ayant au moins une limite apparente sur le domaine public.   
Les proéminences bâties (non utiles pour franchir un obstacle) ne sont pas inclues dans cette classe.

**Contraintes**

Une marche milieu (ou les deux marches milieu lorsque les marches sont en nombre pair) d'une portion d'escalier située entre deux paliers peut être porteuse d'un symbole indiquant le sens de la montée. Le point porteur du symbole est alors déterminé au centre du centroïde de la marche milieu (ou des deux marches milieu lorsque les marches sont en nombre pair).

**Critères de sélection**

L'escalier du PCRS doit obligatoirement être situé à l'extérieur, et proposer au moins une limite apparente avec le domaine public.

**Géométrie**

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

[Identifiant Habillage Symbole](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-habillage-symbole)

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
