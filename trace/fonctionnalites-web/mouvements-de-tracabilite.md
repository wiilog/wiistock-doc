---
description: >-
  Suivre et enregistrer les déplacements des unités logistiques (UL) d'un
  emplacement à un autre, avant leur mise en stock.
---

# Mouvements de traçabilité

**Chemin :** Traçabilité › Mouvements · Web et nomade

Un mouvement de traçabilité enregistre ce qui arrive à une unité logistique (UL) : prise, dépose, groupage, etc. Tous les mouvements, qu'ils viennent du web ou du nomade, apparaissent sur cette page. Vous savez ainsi à tout moment où se trouve une UL.

## Créer un mouvement

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur **Nouveau mouvement**.
{% endstep %}

{% step %}
### Choisir l'action

La **Date** (par défaut : maintenant) et l'**Opérateur** sont préremplis. Choisissez ensuite l'**Action** : les champs du formulaire s'adaptent à votre choix (voir le tableau ci-dessous).
{% endstep %}

{% step %}
### Compléter et enregistrer

Renseignez les champs demandés, et si besoin un commentaire, des pièces jointes et les champs libres. Cliquez ensuite sur **Enregistrer**.
{% endstep %}
{% endstepper %}

| Action                | À quoi elle sert                                                     | Champs à renseigner                                       |
| --------------------- | -------------------------------------------------------------------- | --------------------------------------------------------- |
| **Prise**             | Prendre une UL sur un emplacement.                                   | UL, emplacement, quantité                                 |
| **Dépose**            | Déposer une UL sur un emplacement.                                   | UL, emplacement, quantité                                 |
| **Prises et déposes** | Enregistrer en une fois la prise et la dépose d'une ou plusieurs UL. | Emplacement de prise, UL, emplacement de dépose, quantité |
| **Groupage**          | Regrouper des UL dans une UL contenante (une palette, par exemple).  | UL contenante, UL                                         |
| **Passage à vide**    | Signaler qu'une UL est passée sur un emplacement.                    | UL, emplacement                                           |
| **Dépose dans UL**    | Déposer un ou plusieurs articles dans une UL.                        | UL, article(s), emplacement                               |

{% hint style="info" %}
Le type **Division** apparaît aussi dans la liste : c'est un mouvement créé automatiquement sur le **nomade**, lorsqu'on groupe une UL qui se trouve déjà dans un autre groupe. Il n'est pas à utiliser depuis le web.
{% endhint %}

{% hint style="info" %}
Pour une prise, le champ **Début de délai manuel** permet de fixer vous-même le point de départ du délai suivi dans les [Encours](encours.md).
{% endhint %}

## Consulter, modifier ou supprimer un mouvement

Le menu **⋮** d'une ligne propose trois actions :

* **Détails** : affiche le mouvement en lecture seule.
* **Modifier** : seuls le commentaire et les champs libres sont modifiables. Pour pouvoir modifier tout le mouvement, il faut le droit **Modifier l'ensemble de la modale mouvement** dans [Rôles](../../parametrages/utilisateurs/roles/) › Traçabilité › Mouvements.
* **Supprimer** : supprime le mouvement après confirmation.

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 13.47.48.png" alt="Modification d&#x27;un mouvement"><figcaption></figcaption></figure>

## Retrouver un mouvement

* **Filtres** : dates **Du** / **Au**, **Unité(s) logistique(s)**, **Article**, **Emplacement**, **Types**, **Opérateurs**.
* **Rechercher** : recherche rapide dans le tableau.
* La flèche à côté de **Nouveau mouvement** donne accès à **Exporter au format CSV** et à **Gestion des colonnes**.

<details>

<summary>Colonnes du tableau</summary>

| Colonne                    | Description                                            |
| -------------------------- | ------------------------------------------------------ |
| **Issu de**                | Origine du mouvement : arrivage, acheminement, nomade… |
| **Date**                   | Date du mouvement.                                     |
| **Unité logistique**       | UL ou article déplacé.                                 |
| **Référence**, **Libellé** | Référence et libellé de l'article, le cas échéant.     |
| **Groupe**                 | UL contenante, le cas échéant.                         |
| **Quantité**               | Quantité déplacée.                                     |
| **Emplacement**            | Emplacement du mouvement.                              |
| **Type**                   | Action réalisée.                                       |
| **Opérateur**              | Personne qui a fait le mouvement.                      |
| **Champs libres**          | Champs libres définis pour les mouvements.             |

</details>
