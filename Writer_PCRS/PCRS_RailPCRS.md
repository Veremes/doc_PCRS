# RailPCRS #



**Nom de la classe**

RailPCRS

**Sous-classe de**

ObjetVecteurPCRS

**Titre**

Rail d'un tronçon de voie ferrée

**Définition**

Classe permettant de décrire de façon unitaire et continue l'assemblage de rails d'un tronçon de voie ferrée. Un rail est un guide linéaire constitué de profilés d'acier laminés soudés bout à bout, et constituant le chemin de roulement et de guidage des roues des véhicules ferroviaires. Une voie ferroviaire simple est constituée de deux rails parallèles et à écartement fixe et standardisé qui peut être différent par pays (1,435 m en France).

**Modélisation**

Polylignes <br>
Le levé topographique d'une voie ferrée simple est effectué rail par rail et toujours à l'intérieur vers l'axe de la voie, de façon à maintenir un écart uniforme entre les deux polylignes, et égal à l'écartement du rail. Le nivellement de chaque point de levé doit correspondre à un point situé sur la partie supérieure du rail en contact au niveau de la bande de roulement. Le nivellement des deux rails d'une même section transversale d'une voie simple est normalement identique pour un alignement droit et peut être différent pour une courbe ou une clothoïde (raccordement entre courbe et alignement droit) selon le tracé en plan de la voie ferrée.
Le gestionnaire du PCRS a toute latitude pour préciser lorsque les circonstances le justifient d'autres modes de levé (typiquement dans l'axe du rail au milieu de la bande de roulement sur un rail Vignole) : le cahier des charges ainsi que les Métadonnées de livraison devront alors explicitement préciser le mode de levé associé.
Un rail est souvent décrit dans le secteur ferroviaire par emprises et par tronçons. Cette description « métier » peut être conservée dans le PCRS, mais les attributs servant à la décrire ne font pas à proprement parler partie du PCRS.

**La classe contient**

Tout type de rail (anciennement champignon/double champignon, Vignole, à gorge...) utilisé sur une voie ferrée de tout type (normale, industrielle, à crémaillère, pour le transport urbain, de type tramway).

**Contraintes**

Deux rails connexes doivent lorsqu'il s'agit de la même voie simple partager aux tolérances de précisions planimétrique et altimétriques près une même extrémité. Un aiguillage qui assure la jonction rail par rail entre deux voies simples devra partager (au sens du géoréférencement et aux tolérances de précisions près) chacune de ses extrémités avec un des points levés des rails connectés. La description n'est cependant pas explicitement  topologique : on ne cherchera pas à décrire les relations entre nœuds et segments du réseau ainsi formé.
Classe essentielle du PCRS.

**Critères de sélection**

Ne concerne que les voies situées sur le domaine public ou en assurant sa desserte.

**Géométrie**

- Définition : Géométrie de type courbe

- Type : GM_Curve

- Contraintes : 1

**Paramètres**

[Identifiant Objet](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-objet)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro(s) des Point(s) Levé(s) (séparés par ",")](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-s-des-point-s-leve-s-separes-par)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)

[Producteur](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#producteur)

[Qualité Catégorisation](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#qualite-categorisation)

[Thématique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#thematique)
