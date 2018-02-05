# PointLevePCRS #



**Nom de la classe**

PointLevePCRS

**Titre**

Point levé du PCRS

**Définition**

Point géoréférencé en planimétrie, ou planimétrie et altimétrie du PCRS.

**Modélisation**

Point

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

**Géométrie**

- Définition : Géométrie de type ponctuel

- Type : GM_Point

- Contraintes : 1

**Paramètres**

[Horodatage](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#horodatage)

[Identifiant PCRS](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#identifiant-pcrs)

[Numéro Point Levé](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#numero-point-leve)

[Précision Altimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-altimetrique)

[Précision Planimétrique](http://doc-pcrs.readthedocs.io/fr/latest/Projet_FME/PCRS_Parametres.html#precision-planimetrique)
