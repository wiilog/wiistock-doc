---
description: >-
  Collecter les références demandées, puis les remettre en stock ou les
  détruire.
---

# Collectes

**Chemin :** Ordre › Collecte · ou depuis une demande : flèche › **Aller vers l'ordre de collecte**

Un ordre de collecte est créé automatiquement quand une [demande de collecte](../demandes/collectes.md) est validée. La collecte se fait généralement sur le nomade (voir [Collecte nomade](../../fonctionnalites-mobile/stock-i-collecte.md)), mais elle est aussi possible ici.

## Collecter sur le web

{% stepper %}
{% step %}
### Ouvrir l'ordre

Cliquez sur la ligne de l'ordre de collecte **à traiter**. L'entête rappelle la **Destination** (mise en stock ou destruction) et le **Point de collecte**.
{% endstep %}

{% step %}
### Ajuster les quantités (si besoin)

Le menu **⋮** d'une ligne propose **Modifier** pour collecter une quantité **inférieure** à celle demandée. Ce n'est pas possible si l'article à remettre en stock a été choisi précisément dans la demande.
{% endstep %}

{% step %}
### Valider chaque ligne

Cliquez sur chaque ligne pour la passer en vert. Pour une mise en stock d'une référence gérée à l'article, choisissez d'abord l'article à remettre en stock, ou ne choisissez rien pour créer un nouvel article, puis indiquez la quantité.
{% endstep %}

{% step %}
### Finir la collecte

Cliquez sur **Finir la collecte**. Pour une mise en stock, indiquez pour chaque code-barre l'emplacement où il est déposé.
{% endstep %}
{% endstepper %}

## Ce qui se passe à la fin de la collecte

* L'ordre passe **Traité** et la demande **Collecté** (ou **Partiellement collecté**).
* **Mise en stock** : un mouvement de stock d'**entrée** est créé pour chaque code-barre, ainsi qu'une prise sur le point de collecte et une dépose sur l'emplacement choisi.
* **Destruction** : aucun mouvement de stock n'est créé.

## Les actions de l'ordre

Sous la flèche de l'entête :

* **Aller vers la demande de collecte** ;
* **Imprimer les étiquettes** : étiquettes des articles à remettre en stock ou des références à détruire ;
* **Supprimer** : la demande repasse en brouillon ;
* **Associer à un capteur** : pour une mise en stock, associe la collecte à un objet connecté (température, GPS…).

## Retrouver un ordre de collecte

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Numéros de demande**, **Opérateur**.
* **Colonnes** : numéro, statut, date de création, opérateur, type.
* Le bouton **Exporter au format CSV** exporte les ordres filtrés.
