---
description: >-
  La page des articles regroupent tous les articles des références en gestion
  quantité par article.
---

# Articles

Cette page est disponible dans le menu **Stock**, puis **Articles**. Cette page contient plusieurs éléments :&#x20;

* Une **recherche rapide**, permettant de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Nouvel article**</mark> pour créer un nouvel article&#x20;
* Un bouton <mark style="background-color:blue;">**Impression des étiquettes**</mark>, sous le bouton Nouvel article, pour imprimer les étiquettes des articles. Ce bouton n'est disponible qu'après une recherche rapide
* Un bouton <mark style="background-color:blue;">**Gestion des colonnes**</mark>, sous le bouton Nouvel article, pour gérer les colonnes affichées à l'écran
* Un bouton <mark style="background-color:blue;">**Recherche rapide**</mark>, pour choisir dans quelles colonnes la recherche rapide va chercher
* Un bouton <mark style="background-color:blue;">**Articles actifs seulement**</mark>, sous le bouton Nouvel article, pour afficher seulement les articles en statut _disponible_, _en transit_, et _en litige_
* Un **tableau**, regroupant les différents articles&#x20;

{% embed url="https://www.screencast.com/t/Pbsx8lF6u7P" %}
Page article
{% endembed %}

### Contenu du tableau

Toutes les colonnes sont décrites, à vous de choisir celles qui vous souhaitez avoir à l'écran via la gestion des colonnes

| Colonne                    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Libellé**                | Libellé de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Référence article**      | Nom de la référence à laquelle appartient l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Référence fournisseur**  | Référence de l'article chez votre fournisseur                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Code barre**             | Code barre de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Type**                   | Type de la référence de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Statut**                 | <p>Statut de l'article. L'article peut avoir ces statuts : <br>- <em>disponible</em> : l'article est en stock et disponible. Il peut être solliciter dans les demandes<br>- <em>en transit</em> : l'article est encore en stock mais dans une demande. Il ne peut pas être ajouté à une demande<br>- <em>en litige</em> : l'article est sur un litige non traité dans une réception. Il est en stock mais ne peut pas être ajouté à une demande<br>- <em>consommé</em> : l'article n'est plus en stock</p> |
| **Quantité**               | Quantité de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Emplacement**            | Emplacement où se situe l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Prix unitaire**          | Prix unitaire de chaque article                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Dernier inventaire**     | Date de dernier inventaire de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Lot**                    | Lot de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Date d'entrée en stock** | Date à laquelle l'article est entré en stock                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Date d'expiration**      | Date de péremption de l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Commentaire**            | Commentaire sur l'article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

Dans ce tableau vous pouvez également accéder aux boutons suivants en cliquant sur les<img src="../../.gitbook/assets/3points" alt="" data-size="line">de chaque ligne :&#x20;

* Bouton <mark style="background-color:blue;">**Imprimer**</mark> : pour imprimer l'étiquette de l'article
* Bouton <mark style="background-color:blue;">**Accéder à la demande**</mark> : ce bouton apparait si l'article est dans une demande. Cliquez sur le bouton pour accéder au détail de la demande
* Bouton <mark style="background-color:blue;">**Voir mouvements de traçabilité**</mark> : cliquez sur ce bouton pour être redirigé vers la page des mouvements de traçabilité filtré sur l'article. Vous verrez alors tous les mouvements de traçabilité de l'article
* Bouton <mark style="background-color:blue;">**Historique des données**</mark> : ce bouton apparaît si l'article a été associé à un objet connecté. Si c'est le cas, la ligne de l'article aura un logo wifi. Cliquez sur le bouton pour voir toutes les données qui ont été associées à l'article via un objet connecté

### Ajouter un nouvel article

{% hint style="info" %}
L'ajout d'article doit se faire habituellement via une réception, mais il est possible de créer un article sur cette page.
{% endhint %}

Cliquez sur <mark style="background-color:blue;">**Nouvel article**</mark> et remplissez les champs suivants :&#x20;

* **Référence\*** : champ à remplir pour faire apparaître le champ suivant. Référence de l'article à ajouter
* **Fournisseur\*** : champ à remplir pour faire apparaître tous les autres champs. Fournisseur de l'article. Le choix des fournisseurs se fait parmi les fournisseurs renseignés de la référence choisie
* **Référence fournisseur\*** : nom de la référence chez le fournisseur, soit l'article fournisseur dans l'application. Le choix de l'article fournisseur se fait dans la liste des articles fournisseurs de la référence chez le fournisseur déjà renseignés
* **Libellé\*** : libellé de l'article
* **Type** : champ indisponible, type de la référence
* **Quantité\*** : quantité de l'article
* **Prix unitaire (€)** : prix de l'article
* **Emplacement\*** : emplacement de stockage de l'article, à sélectionner parmi la liste des emplacements de l'application
* **Statut** : champ renseigné automatiquement en disponible. Il ne peut pas être changé
* **Anomalie** : pour indiquer que l'article est en anomalie
* **Lot** : lot de l'article
* **Date de péremption** : date de péremption de l'article
* **Commentaire** : commentaire sur l'article
* **Champs libres** : champs libres sur les articles du type de la référence

{% embed url="https://www.screencast.com/t/ovgLPfW7PXtH" %}
Ajout d'un nouvelle article
{% endembed %}

### Modifier un article

Pour modifier un article cliquez sur la ligne de l'article que vous souhaitez modifier.&#x20;

La modale de modification d'article est différente de celle de création d'article. Vous avez les champs suivants :&#x20;

* **Libellé\***, _champ modifiable_ : libellé de l'article&#x20;
* **Type**, _champ non modifiable_ : type de la référence de l'article
* **Quantité**, _champ non modifiable_ : quantité de l'article
* **Prix unitaire (€)**, _champ modifiable_ : prix de l'article
* **Emplacement**, _champ non modifiable_ : emplacement sur lequel se trouve l'article
* **Statut**, _champ non modifiable_ : statut de l'article
* **Anomalie**, _champ modifiable_ : pour indiqué qu'il y a une anomalie sur l'article
* **Gestionnaires**, _champ non modifiable_ : gestionnaires de la référence de l'article. A modifier directement sur la référence
* **Lot**, _champ modifiable_ : lot de l'article
* **Catégorie d'inventaire**, _champ non modifiable_ : catégorie d'inventaire de la référence de l'article. A modifier directement sur la référence
* **Date dernier inventaire**, _champ non modifiable_ : date de dernier inventaire de l'article
* **Date de péremption**, _champ modifiable_ : date de péremption de l'article
* **Commentaire**, _champ modifiable_ : commentaire sur l'article
* **Champs libres** : tous les champs libres sur l'article sont modifiables
* **Articles fournisseurs**, _champs non modifiables_ : ensemble des articles fournisseurs lié à l'article

Modifiez les champs souhaitez et cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>.

{% embed url="https://www.screencast.com/t/3BED8IhYCYI" %}
Modification d'un article
{% endembed %}

### Supprimer un article

Pour supprimer un article, cliquez sur les<img src="../../.gitbook/assets/3points" alt="" data-size="line">de la ligne de l'article à supprimer et cliquez sur <mark style="background-color:blue;">**Supprimer**</mark>.&#x20;

Une modale de confirmation s'ouvrira alors. Cliquez sur <mark style="background-color:blue;">**Supprimer**</mark> pour confirmer la suppression.

Vous ne pourrez pas supprimer un article si :&#x20;

* il est consommé
* il est lié à des missions d'inventaire
* il est lié à des mouvements de stock
* il est lié à des mouvements de traçabilité
* il est lié à une demande de livraison
* il est lié à une demande de collecte
* il est lié à une demande de transfert
