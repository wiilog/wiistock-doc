---
description: >-
  Retrouver toutes les unités logistiques (UL) et les groupes d'UL, savoir où
  ils se trouvent et consulter leur historique.
---

# Unités logistiques

**Chemin :** Traçabilité › Unités logistiques

Cette page liste toutes les unités logistiques (UL) créées dans Follow GT, ainsi que les groupes d'UL. Une UL peut provenir d'un arrivage, d'un acheminement, d'un mouvement ou d'une réception.

## Retrouver une UL

1. Renseignez un ou plusieurs filtres, puis cliquez sur **Filtrer**. Vos filtres sont conservés d'une session à l'autre.
2. Cliquez sur la **loupe** d'une ligne pour voir directement l'historique des mouvements de l'UL.

<details>

<summary>Filtres disponibles</summary>

| Filtre                  | Description                                                                                                               |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Du** / **Au**         | Période. La flèche à côté permet de choisir la date sur laquelle filtrer : **Dernier mouvement** ou **Date de création**. |
| **Unité logistique**    | Numéro de l'UL.                                                                                                           |
| **Natures**             | Une ou plusieurs natures d'UL.                                                                                            |
| **Dernier emplacement** | UL dont le dernier mouvement a eu lieu sur cet emplacement.                                                               |
| **N° d'arrivage UL**    | UL issues de cet arrivage.                                                                                                |
| **Projet**              | Projet issu du référentiel Projets.                                                                                       |
| **Association**         | Numéro de bon de réception associé à l'UL.                                                                                |
| **Type**                | Afficher uniquement les UL, ou uniquement les groupes.                                                                    |
| **Délai de traitement** | Afficher uniquement les UL soumises à un délai de traitement.                                                             |

</details>

{% hint style="warning" %}
**Dernier emplacement** ne garantit pas que l'UL s'y trouve : si son dernier mouvement est une prise, elle est en cours de déplacement.
{% endhint %}

## Le détail d'une UL

Cliquez sur une ligne pour ouvrir la fiche de l'UL. Elle regroupe :

* **Description** : date de création, arrivage camion et arrivage UL d'origine, tracking associé, n° de commande, poids, volume, projet, fournisseur, transporteur, association IoT ;
* **Historique de groupage** : groupes dans lesquels l'UL a été mise ou retirée ;
* **Historique de traçabilité** : tous les mouvements de l'UL ;
* **Projets assignés** et **Champs libres**.

## Agir sur une UL

Les actions sont disponibles dans le menu **⋮** de la ligne ou en haut de la fiche :

| Action                           | Résultat                                                                                                                                                     |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Modifier**                     | Modifier la nature, la quantité, le poids, le volume et le commentaire. Le poids et le volume servent notamment pour la lettre de voiture des acheminements. |
| **Voir les mouvements**          | Afficher l'historique des mouvements de l'UL.                                                                                                                |
| **Recalculer le délai de traça** | Recalculer le délai de traitement de l'UL.                                                                                                                   |
| **Supprimer**                    | Supprimer l'UL. Il faut d'abord supprimer ses mouvements et les éléments liés, sinon un message d'erreur s'affiche.                                          |

{% hint style="info" %}
Une icône **wifi** signale une UL qui est, ou a été, associée à un objet connecté. Le bouton **Historique des données** affiche alors les données remontées par les capteurs. Voir [IoT](https://app.gitbook.com/s/id6mpmGgIXZ3CFWUO3AX/iot).
{% endhint %}

## Colonnes du tableau

Pour choisir les colonnes affichées, ouvrez la flèche à côté de **Exporter au format CSV**, puis **Gestion des colonnes**.

<details>

<summary>Colonnes disponibles</summary>

| Colonne                                                 | Description                                                                                         |
| ------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **Numéro d'UL**                                         | Numéro de l'UL. Pour une UL issue d'une réception, c'est le numéro de l'article ou de la référence. |
| **Nature**                                              | Nature de l'UL. Elle est vide pour les UL issues d'une réception.                                   |
| **Quantité**                                            | Quantité contenue dans l'UL.                                                                        |
| **Projet**, **Numéro de projet**                        | Projet rattaché à l'UL.                                                                             |
| **Date dernier mouvement**, **Date de création**        | Dates clés de l'UL.                                                                                 |
| **Issu de**                                             | Lien vers l'arrivage, l'acheminement ou la réception d'origine.                                     |
| **Dernier emplacement**                                 | Emplacement du dernier mouvement connu.                                                             |
| **Association**                                         | Numéro de l'association BR.                                                                         |
| **Arrivage camion**                                     | Arrivage camion lié à l'UL.                                                                         |
| **Délai de traitement**, **Date limite de traitement**  | Suivi du délai de traitement, si un délai s'applique.                                               |
| **Groupe rattaché**                                     | Groupe dans lequel se trouve l'UL.                                                                  |
| **Fournisseur**, **N° commande / BL**, **Transporteur** | Informations reprises de l'arrivage.                                                                |

</details>
