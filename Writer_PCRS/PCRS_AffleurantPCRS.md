# PCRS_AffleurantPCRS #



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

Selon les classes d'affleurant spécialisées, et représentées (de préférence) par une représentation exhaustive et interopérable comme le polygone AffleurantEnveloppePCRS, éventuellement complété par un habillage de type HabillageLignesPCRS, néanmoins d'autres modélisation géométriques sont offertes afin de ne pas perdre d'informations. La modélisation géométrique est propre à chacune des classes d'affleurant spécialisées AffleurantXXXPCRS du PCRS.

**La classe contient**

Bouches, avaloirs, regards, plaques, poteaux, coffrets...

**Contraintes**

Classe essentielle du PCRS.

**Paramètres**

[Gestionnaire](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#gestionnaire)

[Identifiant Affleurant Symbole](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-affleurant-symbole)

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Identifiant Source](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-source)

[Nature](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#nature)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Réseau](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#reseau)

[Source](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#source)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
