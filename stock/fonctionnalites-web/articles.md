---
description: >-
  Retrouver et gérer les articles, c'est-à-dire les pièces uniques des
  références gérées en quantité à l'article.
---

# Articles

**Chemin :** Stock › Articles

Un **article** est une pièce ou un conditionnement unique d'une [référence](references.md) gérée en quantité **à l'article**. Chaque article a son propre code-barre, son emplacement, et éventuellement un lot et une date de péremption.

{% hint style="info" %}
Les articles sont normalement créés lors d'une [réception](ordres/receptions/). La création manuelle depuis cette page, un import ou l'API de création d'articles restent possibles.
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

### Trier la liste

* Cliquez sur l'en-tête d'une colonne pour trier la liste. Le tri choisi est mémorisé et retrouvé à la prochaine ouverture de la page.
* Le tri sur la **Date d'entrée en stock** fonctionne dans les deux sens. Les articles sans date d'entrée en stock restent toujours en fin de liste, même en tri croissant. À date égale, l'ordre d'affichage reste stable.

### Organiser les colonnes

* **Gestion des colonnes** permet d'afficher ou de masquer chaque colonne, y compris la colonne **Imprimer**.
* Vous pouvez réorganiser les colonnes en faisant glisser leur en-tête. L'ordre est enregistré pour votre utilisateur et restauré à chaque ouverture de la page ; chaque utilisateur conserve son propre ordre.

## Créer un article

1. Cliquez sur **Nouvel article**. Une page de création s'ouvre.
2. Choisissez la **Référence**, puis le **Fournisseur** et la **Référence fournisseur** parmi ceux de la référence. Le **Type** est repris de la référence, et le **Code barre** est généré automatiquement.
3. Renseignez le **Libellé**, la **Quantité** et l'**Emplacement** (obligatoires).
4. Complétez si besoin : **Anomalie**, **Projet**, **Commentaire**, **Tag RFID**, **Lot**, **Date de péremption**, **Prix unitaire**.
5. Cliquez sur **Enregistrer**.

## Imprimer l'étiquette des nouveaux articles

La colonne **Imprimer** permet de repérer d'un coup d'œil les articles dont l'étiquette n'a pas encore été imprimée, par exemple les articles créés automatiquement par l'interface avec votre ERP.

* Tant que l'étiquette d'un article n'a pas été imprimée depuis cette colonne, un bouton **Imprimer** est affiché sur sa ligne.
* Au clic, l'étiquette est générée et l'article est marqué comme « étiquette imprimée » : le bouton disparaît aussitôt, sans recharger la page.
* La colonne est visible pour les utilisateurs ayant le droit d'afficher les articles.

{% hint style="info" %}
Les articles existant avant la mise en place de cette fonctionnalité sont considérés comme déjà imprimés : le bouton n'apparaît que pour les articles créés ensuite.
{% endhint %}

{% hint style="success" %}
Astuce : triez la liste sur la **Date d'entrée en stock** et placez la colonne **Imprimer** en première position pour traiter rapidement les étiquettes des derniers articles entrés.
{% endhint %}

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

* **Imprimer** : imprimer l'étiquette de l'article (réimpression possible à tout moment) ;
* **Accéder à la demande** : si l'article est dans une demande ;
* **Voir mouvements de traçabilité** ;
* **Historique des données** : si l'article est associé à un objet connecté (icône wifi) ;
* **Supprimer** : impossible si l'article est consommé ou lié à un inventaire, un mouvement ou une demande.

<details>

<summary>Colonnes disponibles</summary>

Imprimer, Libellé, Référence article, Référence fournisseur, Code barre, Type, Statut, Quantité, Emplacement, Prix unitaire, Dernier inventaire, Lot, Date d'entrée en stock, Date d'expiration, Commentaire, et les champs libres.

</details>
