---
description: >-
  Préparer les références d'une demande de livraison, sur le web ou sur le
  nomade, avant leur livraison.
---

# Préparations

**Chemin :** Ordre › Préparation · ou depuis une demande de livraison : flèche › **Aller vers l'ordre de préparation**

Un ordre de préparation est créé automatiquement quand une [demande de livraison](../demandes/livraisons.md) est validée. Une fois la préparation terminée, Follow GT crée l'[ordre de livraison](livraisons.md). La préparation se fait généralement sur le nomade (voir [Préparation nomade](../../fonctionnalites-mobile/stock-i-preparation.md)), mais elle est aussi possible ici.

## Préparer sur le web

{% stepper %}
{% step %}
### Ouvrir l'ordre

Cliquez sur la ligne de l'ordre de préparation **à traiter**.
{% endstep %}

{% step %}
### Saisir les quantités prélevées

Cliquez sur chaque ligne à préparer :

* **référence gérée à la référence** (ou article déjà choisi dans la demande) : la quantité demandée est préremplie. Gardez-la ou indiquez une quantité inférieure, puis cliquez sur **Enregistrer** ;
* **référence gérée à l'article** : choisissez les articles à prendre. Cochez **Quantité totale ?** pour prendre tout un article, ou saisissez une quantité. Les articles sont proposés dans l'ordre FIFO ou FEFO de la référence, après ceux de l'emplacement de picking s'il y en a un.

La ligne passe en vert. Vous ne pouvez pas prélever plus que la quantité demandée.
{% endstep %}

{% step %}
### Finir la préparation

Dès qu'au moins une ligne est verte, cliquez sur **Finir la préparation**, puis indiquez l'**emplacement** où les références ont été préparées.
{% endstep %}
{% endstepper %}

## Ce qui se passe à la fin de la préparation

* L'ordre de préparation et la demande de livraison passent **Préparé**, ou **Partiellement préparé** s'il manque des quantités.
* Un **ordre de livraison** est créé, au statut **À traiter**.
* En cas de préparation partielle, un nouvel **ordre de préparation** est créé pour le reste.
* Un **mouvement de transfert** est créé pour chaque référence ou article, de son emplacement de stockage vers l'emplacement de préparation. La quantité disponible de la référence diminue ; la quantité en stock ne change pas encore.

## Les actions de l'ordre

Sous la flèche à côté de **Finir la préparation** :

| Action                                  | Résultat                                                                                                                                                                             |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Supprimer**                           | Supprime l'ordre (s'il n'est pas préparé). La demande repasse en brouillon.                                                                                                          |
| **Imprimer les étiquettes**             | Imprime les étiquettes des articles et des références à livrer.                                                                                                                      |
| **Imprimer le bon de préparation**      | Génère le bon de préparation, selon le modèle paramétré par type de livraison dans [Modèles de document](../../../parametrages/modeles-de-document.md#livraison-bon-de-preparation). |
| **Retourner à la demande de livraison** | Ouvre la demande d'origine.                                                                                                                                                          |
| **Aller vers l'ordre de livraison**     | Une fois l'ordre préparé.                                                                                                                                                            |
| **Associer à un capteur**               | Associe la préparation à un objet connecté (température, GPS…).                                                                                                                      |

Sur chaque ligne d'article, le menu **⋮** propose **Voir** (fiche de la référence ou de l'article) et **Imprimer** (étiquette).

## Retrouver un ordre de préparation

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Numéros de demande**, **Opérateur**.
* **Colonnes** : numéro, statut, date de création, opérateur, type.
* Le bouton **Exporter au format CSV** exporte les ordres filtrés.
