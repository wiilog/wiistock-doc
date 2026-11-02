---
description: >-
  Déplacer les références ou articles d'une demande de transfert vers leur
  nouvel emplacement.
---

# Transferts

**Chemin :** Ordre › Transfert · ou depuis une demande : flèche › **Aller vers l'ordre de transfert**

Un ordre de transfert est créé automatiquement quand une [demande de transfert](../demandes/transferts.md) est validée. Le transfert se fait généralement sur le nomade (voir [Transfert nomade](../../fonctionnalites-mobile/stock-i-transfert.md)), mais il est aussi possible ici.

## Transférer sur le web

1. Cliquez sur la ligne de l'ordre **à traiter**. L'entête rappelle l'**Origine** et la **Destination**.
2. Vérifiez la liste des références et des articles.
3. Cliquez sur **Transférer**.

**Résultat :** l'ordre et la demande passent **Traité**, et un **mouvement de transfert** est créé pour chaque référence ou article, de l'origine vers la destination.

{% hint style="info" %}
**Dépose réelle** : si l'option _Autoriser la dépose des articles sur un emplacement libre_ est activée dans le [paramétrage du terminal mobile](../../../parametrages/terminal-mobile/transfert-a-traiter.md), l'opérateur peut déposer sur un autre emplacement que la destination. Cet emplacement s'affiche alors dans **Dépose réelle**.
{% endhint %}

## Les actions de l'ordre

Sous la flèche à côté de **Transférer** :

* **Aller vers la demande de transfert** ;
* **Supprimer** : la demande repasse en brouillon. Si l'ordre est déjà traité, une fenêtre vous demande où déposer les références transférées, pour ne pas perdre leur traçabilité.

Un clic sur une ligne ouvre la fiche de la référence ou de l'article.

## Retrouver un ordre de transfert

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Créé par**, **Traité par**.
* **Colonnes** : numéro (**OT** + date + compteur), statut, créé par, traité par, origine, destination, date de création, date de traitement.
* Le bouton **Exporter au format CSV** exporte les ordres filtrés.
