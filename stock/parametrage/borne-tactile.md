---
description: >-
  Paramétrer les bornes et tablettes en libre-service : entrée en stock par
  borne et sortie de stock rapide par tablette.
---

# Borne tactile

**Chemin :** Paramétrage › Stock › Borne tactile

Cette page règle les deux parcours en libre-service de Follow GT. Chacun s'utilise depuis un **lien externe**, à ouvrir sur la borne ou la tablette.

| Parcours                                   | Usage                                                                | Guide utilisateur                                                                                                     |
| ------------------------------------------ | -------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **Demande collecte et création référence** | Faire entrer rapidement en stock un nouvel article depuis une borne. | [Demande collecte et création référence](../fonctionnalites-borne-tablette/demande-collecte-et-creation-reference.md) |
| **Demande livraison rapide**               | Laisser un utilisateur sortir lui-même du stock depuis une tablette. | [Demande de livraison rapide](../fonctionnalites-borne-tablette/demande-de-livraison-rapide.md)                       |

## Demande collecte et création référence

### Général

* **Logo en haut à gauche** et **Logo en haut à droite** : les logos affichés sur la borne.
* **Exemple d'étiquette** : l'image de l'étiquette que l'opérateur doit scanner.
* **Messages** affichés sur la borne : message d'accueil, message d'information, message de scan de l'étiquette article, messages de validation (entrée d'une référence, entrée d'un article) et message d'erreur quand la quantité vaut 1.

Les messages acceptent deux variables : `@codearticle` (code de l'article remis en stock) et `@reference` (référence mise en stock).

### Création d'une référence

Ces valeurs s'appliquent aux références créées depuis la borne, toujours gérées en quantité par article :

| Champ                                            | Rôle                                                 |
| ------------------------------------------------ | ---------------------------------------------------- |
| **Type** \*                                      | Type de la référence créée.                          |
| **Champ libre**                                  | Champ libre de la référence qui recevra le n° de BL. |
| **Statut** \*                                    | Actif, Inactif ou Brouillon.                         |
| **Groupe de visibilité**                         | Groupe de visibilité appliqué à la référence.        |
| **Catégorie d'inventaire**                       | Catégorie d'inventaire appliquée à la référence.     |
| **Nom fournisseur** \* / **Code fournisseur** \* | Fournisseur associé par défaut.                      |

### Liens pour borne

Cliquez sur **Ajouter un lien externe** pour créer une borne. Renseignez le **type de collecte**, le **nom de la borne**, le **point de collecte** et le **demandeur**, puis enregistrez. Le **lien externe généré** est l'adresse à ouvrir sur la borne.

Le menu **⋮** d'une ligne permet de **Modifier**, de **Supprimer** ou de **Déconnecter** la borne.

## Demande livraison rapide

### Apparence générale

* **Logo en haut à gauche** et **Logo en haut à droite**.
* **Message d'information** \* : texte affiché sur la tablette, par exemple le contact en cas de problème.

### Liens pour tablette

Cliquez sur **Ajouter un lien externe** pour créer un lien de sortie de stock. Chaque lien combine :

| Champ                               | Rôle                                                                                                                    |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Type de livraison**               | Type des demandes de livraison créées.                                                                                  |
| **Groupe de visibilité**            | Limite la recherche aux références de ce groupe.                                                                        |
| **Destination**                     | Emplacement de livraison.                                                                                               |
| **Utilisateur(s) mail information** | Personnes qui reçoivent le récapitulatif de chaque sortie.                                                              |
| **Filtres**                         | Jusqu'à 3 filtres, choisis parmi les champs libres des articles ou références, pour aider la recherche sur la tablette. |

{% hint style="info" %}
Un même couple **Type de livraison** + **Groupe de visibilité** ne peut être utilisé que par un seul lien.
{% endhint %}

Le **lien externe généré** est l'adresse à ouvrir sur la tablette.

Cliquez sur **Enregistrer** pour valider vos modifications.
