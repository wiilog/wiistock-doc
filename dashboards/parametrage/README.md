---
description: >-
  Créer un dashboard, le structurer en lignes et colonnes, puis y ajouter des
  composants.
---

# Paramétrage

**Chemin :** Paramétrage › Dashboards › Paramétrage complet

{% hint style="info" %}
Limite : **75 composants** au total, quel que soit le nombre de dashboards. Chaque dashboard compte au maximum **6 lignes de 6 colonnes**, mais un dashboard aussi chargé devient difficile à lire.
{% endhint %}

## Créer et gérer un dashboard

Cliquez sur **Ajouter un dashboard**, saisissez le **Nom du dashboard\*** puis cliquez sur **Ajouter**. Les dashboards apparaissent en bas de la page : cliquez sur un nom pour l'ouvrir.

L'écrou à côté du nom donne accès à :

| Action                | Effet                                                                                                                                                                                                                                             |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Paramétrage**       | Renommer le dashboard. L'option **Mettre en valeur 1 ou 2 composant(s) avec le délai le plus court** concerne les composants [Quantité en cours sur n emplacement(s)](liste-des-composants/tracabilite/quantite-en-cours-sur-n-emplacement-s.md). |
| **Supprimer**         | Supprime le dashboard, après confirmation.                                                                                                                                                                                                        |
| **Dashboard externe** | Ouvre le lien du dashboard consultable sans connexion. Voir [Dashboards externes](../dashboards-externes.md).                                                                                                                                     |

{% hint style="warning" %}
Pensez à cliquer sur **Enregistrer** en bas à droite après chaque modification de structure ou de composant.
{% endhint %}

## Structurer le dashboard

Avant de commencer, listez les informations à afficher et la place dont chacune a besoin.

{% stepper %}
{% step %}
### Ajouter des lignes

Cliquez sur **Ajouter une ligne**, choisissez le nombre de colonnes, puis cliquez sur **Ajouter**. Répétez autant que nécessaire (6 lignes maximum).
{% endstep %}

{% step %}
### Diviser des cellules (facultatif)

Chaque cellule peut être divisée une fois : **Diviser en hauteur** (deux cellules l'une sur l'autre) ou **Diviser en largeur** (deux demi-colonnes).

Une division sans composant n'est pas enregistrée.
{% endstep %}

{% step %}
### Ajouter les composants

Dans une cellule, cliquez sur **Ajouter un composant**, choisissez-le (survolez l'icône **i** pour sa description), puis paramétrez-le. Voir la [liste des composants](liste-des-composants/).
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**, puis donnez l'accès au dashboard dans les [rôles](../acces-selon-les-roles.md).
{% endstep %}
{% endstepper %}

## Modifier une ligne

À droite de chaque ligne :

* **Crayon** : changer le nombre de colonnes. Les nouvelles colonnes s'ajoutent à droite. Si vous en retirez alors que des composants sont paramétrés, choisissez les composants à conserver : les cellules en trait plein ont un composant, celles en pointillés sont vides. Les composants gardés sont replacés à gauche.
* **Poubelle** : supprimer la ligne.

![](<../../.gitbook/assets/image (40).png>)
