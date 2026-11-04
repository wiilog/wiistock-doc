---
description: >-
  Ajouter les références attendues, réceptionner les quantités ou les articles,
  puis clôturer la réception.
---

# Détail réception

Cliquez sur une ligne de la liste des [réceptions](./) pour ouvrir son détail. Il contient trois zones :

* l'**entête**, avec les informations de la réception et ses actions ;
* la **liste des articles** à réceptionner ;
* la liste des **litiges** (voir [Litiges / Qualité](litiges-qualite.md)).

{% hint style="info" %}
L'entête affiche « Cette réception est URGENCE » si la case **Urgence ?** est cochée, ou un message si une référence de la réception fait l'objet d'une [urgence Stock](../../../../urgences/urgences.md).
{% endhint %}

## Ajouter une référence attendue

1. Cliquez sur **Ajouter une référence**, puis choisissez la **Référence**. Si elle n'existe pas, cliquez sur **Créer**.
2. Renseignez le **Numéro de commande d'achat** (prérempli avec celui de l'entête) et la **Quantité à recevoir**.
3. Complétez si besoin : **Prix unitaire**, **Anomalie**, **Commentaire**.
4. Cliquez sur **Enregistrer**, ou sur **Réceptionner les articles** pour passer directement à la réception d'une référence gérée à l'article.

## Réceptionner une référence gérée à la référence

1. Cliquez sur la ligne de la référence.
2. Saisissez la **Quantité reçue**, puis cliquez sur **Enregistrer**.

**Résultat :** un mouvement d'entrée en stock et un mouvement de traçabilité sont créés, la quantité en stock augmente et la colonne **Reçu** se met à jour.

## Réceptionner des articles (référence gérée à l'article)

{% stepper %}
{% step %}
### Ouvrir la réception des articles

Cliquez sur **Réceptionner les articles** à l'ajout de la ligne, ou sur **Réception** dans l'entête, puis choisissez la référence à recevoir.
{% endstep %}

{% step %}
### Décrire le conditionnement

Renseignez la **Référence fournisseur**, le nombre d'**Article(s)** (une étiquette par article) et la **Quantité** par article, puis si besoin le **Lot**, la **Date de péremption** et les champs libres. Cliquez sur **Ajouter des articles**. Recommencez pour un autre conditionnement.
{% endstep %}

{% step %}
### Créer une demande dans la foulée (facultatif)

* **Livraison** : renseignez le **Demandeur**, le **Type** et la **Destination**. Selon le paramétrage, la demande est créée seule, avec sa préparation, ou en livraison directe.
* **Transfert** : l'**Emplacement d'origine** (réception) et l'**Emplacement de stockage** sont préremplis.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**. Les articles sont créés avec leurs étiquettes, les mouvements d'entrée en stock et de traçabilité sont générés, et la colonne **Reçu** se met à jour.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Vous ne pouvez pas réceptionner plus que la quantité **À recevoir**.
{% endhint %}

## Les actions

**Dans l'entête :**

| Action                             | Résultat                                                                                   |
| ---------------------------------- | ------------------------------------------------------------------------------------------ |
| **Réception**                      | Ouvre la réception des articles.                                                           |
| **Finir la réception**             | Passe la réception en **Réception totale** et remplit la date de fin.                      |
| **Modifier**                       | Modifie les champs de la réception (selon le paramétrage des champs fixes).                |
| **Voir les demandes de livraison** | Si la réception en a créé.                                                                 |
| **Supprimer**                      | Possible seulement si la réception ne contient plus d'articles.                            |
| **Annuler cette réception**        | Sur une réception totale : elle repasse en **Réception partielle** et peut être complétée. |

**Sur la liste des articles :** **Générer les étiquettes** (flèche à côté de **Ajouter une référence**) et, sur chaque ligne, **Voir mouvements de traçabilité**, **Voir les articles** (gestion à l'article), **Imprimer** et **Supprimer**. Pour supprimer une ligne déjà réceptionnée à l'article, supprimez d'abord ses articles.
