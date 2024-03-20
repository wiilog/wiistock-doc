# Suivre le traitement d’une demande de livraison/collecte

La livraison/collecte suit le même fonctionnement qu’une [livraison](suivre-le-traitement-dune-demande-de-livraison.md). Elle va suivre le même comportement qu’une livraison en cas d’attente de validation, de sous-traitance, d’écartement de colis ou de rejet de livraison sur la tournée.

La livraison/collecte possède juste un statut en plus par rapport à la livraison : le statut « Objets déposés » qui permet de savoir quand est-ce que les objets collectés sur cette livraison ont été retourné au CLB.

{% embed url="https://www.screencast.com/t/hF9J7GVk" %}
Détail d'une demande de livraison/collecte
{% endembed %}

En cas de non-livraison, le traitement est le même que pour une livraison, et la collecte ne se fait pas.

En cas de non-collecte (la livraison a cependant pu se faire), il n’y aura pas de statut « Objets déposés », et vous devrez refaire une demande de collecte pour ce patient si nécessaire.
