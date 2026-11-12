---
description: >-
  Retrouver et gérer les articles, c'est-à-dire les pièces uniques des
  références gérées en quantité à l'article.
---

# Articles

**Chemin :** Stock › Articles

Un **article** est une pièce ou un conditionnement unique d'une [référence](references.md) gérée en quantité **à l'article**. Chaque article a son propre code-barre, son emplacement, et éventuellement un lot et une date de péremption.

{% hint style="info" %}
Les articles sont normalement créés lors d'une [réception](ordres/receptions/). La création manuelle depuis cette page ou un import reste possible.
{% endhint %}

## Les statuts d'un article

| Statut         | Signification                                                |
| -------------- | ------------------------------------------------------------ |
| **Disponible** | En stock et utilisable dans une demande.                     |
| **En transit** | En stock, mais déjà réservé dans une demande.                |
| **En litige**  | En stock, mais bloqué par un litige de réception non traité. |
| **Consommé**   | Sorti du stock.                                              |

## Retrouver un article

* Utilisez le champ **Rechercher**. Le choix des colonnes où il cherche se fait dans **Recherche rapide**, via la flèche à côté de **Nouvel article**.
* La même flèche donne accès à **Gestion des colonnes**, à **Impression des étiquettes** (après une recherche) et à **Articles actifs seulement** (statuts disponible, en transit et en litige).

## Créer un article

1. Cliquez sur **Nouvel article**. Une page de création s'ouvre.
2. Choisissez la **Référence**, puis le **Fournisseur** et la **Référence fournisseur** parmi ceux de la référence. Le **Type** est repris de la référence, et le **Code barre** est généré automatiquement.
3. Renseignez le **Libellé**, la **Quantité** et l'**Emplacement** (obligatoires).
4. Complétez si besoin : **Anomalie**, **Projet**, **Commentaire**, **Tag RFID**, **Lot**, **Date de péremption**, **Prix unitaire**.
5. Cliquez sur **Enregistrer**.

## Le détail d'un article

Cliquez sur une ligne pour ouvrir la fiche de l'article. Elle affiche notamment :

* la date d'entrée en stock, l'anomalie, le projet, le lot, la date de péremption, le prix unitaire ;
* le gestionnaire et la catégorie d'inventaire, repris de la référence ;
* la date du dernier inventaire, la **date de disponibilité constatée** et la **date d'épuisement constatée** ;
* les champs libres ;
* un lien **Ouvrir la page** vers ses mouvements de traçabilité.

Cliquez sur **Modifier** pour changer le libellé, le prix, l'anomalie, le lot, la date de péremption, le commentaire ou les champs libres. La quantité, l'emplacement et le statut ne se modifient pas ici : ils évoluent avec les mouvements de stock.

## Agir sur un article

Le menu **⋮** d'une ligne propose :

* **Imprimer** : imprimer l'étiquette de l'article ;
* **Accéder à la demande** : si l'article est dans une demande ;
* **Voir mouvements de traçabilité** ;
* **Historique des données** : si l'article est associé à un objet connecté (icône wifi) ;
* **Supprimer** : impossible si l'article est consommé ou lié à un inventaire, un mouvement ou une demande.

<details>

<summary>Colonnes disponibles</summary>

Libellé, Référence article, Référence fournisseur, Code barre, Type, Statut, Quantité, Emplacement, Prix unitaire, Dernier inventaire, Lot, Date d'entrée en stock, Date d'expiration, Commentaire, et les champs libres.

</details>
