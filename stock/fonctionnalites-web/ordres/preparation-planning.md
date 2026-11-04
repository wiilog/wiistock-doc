---
description: >-
  Planifier les préparations par date, puis les lancer en masse après
  vérification du stock disponible.
---

# Préparation - Planning

**Chemin :** Ordre › Préparation - Planning

Avec le planning, les demandes de livraison peuvent être créées **sans vérifier le stock disponible**, avec des dates attendues différentes. Les préparations s'affichent ensuite sur un planning, et vous les **lancez en masse** une fois le stock vérifié.

## Activer le planning

| Où                                                                                    | Quoi activer                                                                                                                                   |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| [Rôles](../../../parametrages/utilisateurs/roles/) › Ordre › Préparations             | **Afficher préparations - planning** et, si besoin, **Modifier la date de préparation** (bouton **Modifier** sur le détail d'une préparation). |
| [Paramétrage › Stock › Demandes › Livraisons](../../parametrage/demandes/livraisons/) | **Réaliser une demande de livraison sans quantité en stock (lancement de préparation)**.                                                       |
| Livraisons › Champs fixes                                                             | Afficher **Date attendue** à la création.                                                                                                      |

Par défaut, la date de préparation est la date attendue de la livraison.

## Lire le planning

* **Filtres** : **Numéro de demande**, **Opérateurs**, **Type** et **Statuts** (tous sélectionnés par défaut).
* **Aujourd'hui** et les flèches permettent de naviguer. Le planning affiche 5 jours.
* Chaque étiquette indique le numéro de la préparation, son statut, le type de livraison, la date de création et la date attendue. Un clic ouvre le détail de la préparation.
* Pour changer la date d'une préparation **Validée**, faites glisser son étiquette sur un autre jour.

| Statut                      | Signification                                                          |
| --------------------------- | ---------------------------------------------------------------------- |
| **Validé**                  | La demande de livraison est validée. Premier statut d'une préparation. |
| **Lancé**                   | La préparation est lancée : le stock a été vérifié et réservé.         |
| **En cours de préparation** | L'opérateur a commencé la préparation.                                 |
| **Partiellement préparé**   | Une partie seulement a été préparée ; un reliquat a été créé.          |
| **Traité**                  | Toutes les quantités ont été préparées.                                |

## Lancer les préparations

{% stepper %}
{% step %}
### Choisir les préparations

Cliquez sur **Lancer les préparations**. La fenêtre liste les préparations **Validées** de la période affichée. Faites-les glisser vers **Préparation(s) à lancer**, ou cliquez sur **Lancer tous** (**Remettre tout** fait l'inverse).
{% endstep %}

{% step %}
### Vérifier le stock

Cliquez sur **Vérifier le stock**. Pour chaque référence, la quantité disponible est comparée à la quantité demandée :

* **contour vert** : le stock suffit ;
* **contour rouge** : le stock manque. La section **Manque quantité sur** indique la référence, la quantité disponible et la quantité demandée. Retirez la préparation concernée pour pouvoir continuer.
{% endstep %}

{% step %}
### Valider le lancement

Cliquez sur **Valider le lancement**. Les préparations passent **Lancé**, apparaissent sur le nomade (selon le paramétrage des types de livraison) et le stock disponible des références est réservé.
{% endstep %}
{% endstepper %}
