---
description: Livrer les références préparées et clôturer la demande de livraison.
---

# Livraisons

**Chemin :** Ordre › Livraison · ou depuis une demande ou une préparation : flèche › **Aller vers l'ordre de livraison**

Un ordre de livraison est créé automatiquement à la fin d'une [préparation](preparations.md). Une fois livré, il clôture la [demande de livraison](../demandes/livraisons.md) et la quantité sort du stock. La livraison se fait généralement sur le nomade (voir [Livraison nomade](../../fonctionnalites-mobile/stock-i-livraison.md)), mais elle est aussi possible ici.

## Livrer sur le web

1. Cliquez sur la ligne de l'ordre de livraison **à traiter**.
2. Vérifiez la liste des articles à livrer.
3. Cliquez sur **Finir la livraison**.

## Ce qui se passe à la fin de la livraison

* L'ordre de livraison passe **Livré**, ou **Partiellement livré** s'il vient d'une préparation partielle.
* La demande de livraison passe **Livré**, ou **Livré partiellement** si d'autres préparations restent à livrer.
* Un **mouvement de sortie** est créé pour chaque référence ou article, de l'emplacement de préparation vers le point de livraison. La quantité en stock diminue.

## Les actions de l'ordre

Sous la flèche à côté de **Finir la livraison** :

* **Retourner à la demande de livraison** et **Retourner à la préparation** ;
* **Supprimer** : l'ordre de préparation repasse **à traiter**. Une fenêtre vous demande l'emplacement où déposer les références préparées, pour ne pas perdre leur traçabilité.

Un clic sur une ligne d'article ouvre la fiche de la référence ou de l'article.

## Retrouver un ordre de livraison

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Numéros de demande**, **Opérateur**.
* **Colonnes** : numéro, statut, date de création, opérateur, type.
* Le bouton **Exporter au format CSV** exporte les ordres filtrés.
