Accès DSL asymétrique
=====================

Accès ADSL
----------

Les accès ADSL sont livrés sans EAS, sur une interface cuivre.

A chaque utilisateur sont associées une ou deux connexions ATM de niveau
VC qui supportent le flux ATM bidirectionnel entre l'équipement terminal
de l’utilisateur et un DSLAM.

Débits
~~~~~~

IMAGE ICI

Pour sélectionner le VC “Best Effort” ou le VC d’un accès ADSL Mono-VC,
les trames doivent emprunter les circuits:

Virtual Path Identifier (Vpi): 8

Virtual Circuit Identifier (Vci): 35

Pour utiliser le VC “Premium” d’un Accès ADSL Bi-VC, les trames doivent
être emprunter les circuits:

Virtual Path Identifier (Vpi): 8

Virtual Circuit Identifier (Vci): 50

La somme des débits des VC ne peut pas dépasser le débit du profil de la
ligne. En cas de congestion, le trafic du VC premium est prioritaire sur
le VC “Best Effort”.

Établissement de session IP
~~~~~~~~~~~~~~~~~~~~~~~~~~~

L’utilisateur se connecte à la plate-forme de services de l’opérateur
grâce à l’établissement d’une unique session PPPoE par VC entre le
terminal utilisateur et le point central d'aiguillage du réseau d’accès
DSL.

Accès VDSL
----------

Les accès VDSL sont livrés sans EAS, sur une interface cuivre.

Débits
~~~~~~

IMAGE ICI

Les flux issus des sites extrémités sont transportés dans le VLAN
d’accès jusqu’au DSLAM.

Le service emprunte une ou deux connexions Ethernet de niveau VLAN entre
le modem installé chez le client et le DSLAM.

Pour sélectionner le VLAN “Best Effort” ou le VLAN d’un accès VDSL
MonoVlan, les trames doivent être encapsulées avec un marquage dot1Q 835

Pour utiliser le VLAN “Premium” d’un Accès VDSL Bi-VLAN, les trames
doivent être encapsulées avec un marquage dot1Q 850

La somme des débits des VLAN ne peut pas dépasser le débit du profil de
la ligne. En cas de congestion, le trafic du VLAN premium est
prioritaire sur le VLAN “Best Effort”.

Établissement de session IP
~~~~~~~~~~~~~~~~~~~~~~~~~~~

L’utilisateur se connecte à la plate-forme de services de l’opérateur
grâce à l’établissement d’une unique session PPPoE par VLAN entre le
terminal utilisateur et le point central d'aiguillage du réseau d’accès
DSL.
