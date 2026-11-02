---
description: >-
  Demander la récupération de références à remettre en stock ou à détruire, et
  suivre la demande.
---

# Collectes

**Chemin :** Demande › Collecte · création avec le bouton **+** du bandeau, puis **Collecte**

Une demande de collecte sert à faire récupérer des références sur un point de collecte, pour les **remettre en stock** (la quantité en stock augmente) ou les **détruire** (aucun mouvement de stock). Une fois validée, elle crée un [ordre de collecte](../ordres/collectes.md).

## Créer une demande de collecte

{% stepper %}
{% step %}
### Créer l'entête

Cliquez sur le bouton **+** du bandeau, puis sur **Collecte**. Renseignez :

* le **Type** : il détermine les champs libres et les emplacements autorisés ;
* l'**Objet** de la collecte ;
* le **Point de collecte** ;
* la **Destination** : **Mise en stock** ou **Destruction** ;
* si besoin un **Commentaire**.

Cliquez sur **Enregistrer** : la demande est créée en **Brouillon** et sa fiche s'ouvre.
{% endstep %}

{% step %}
### Ajouter les références

Cliquez sur **Ajouter un article**. Choisissez la **Référence** et la **Quantité à collecter**, puis cliquez sur **Ajouter**. Recommencez pour chaque référence.

Pour une mise en stock d'une référence gérée à l'article (et selon votre rôle), un champ **Code article** apparaît : choisissez un article sorti récemment, ou laissez vide pour qu'un nouvel article soit créé.
{% endstep %}

{% step %}
### Valider

Cliquez sur **Valider** : la demande passe **à traiter** et l'ordre de collecte est créé.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Vous pouvez aussi créer une collecte depuis le [panier](../panier.md), ou depuis une borne avec la [demande collecte et création référence](../../fonctionnalites-borne-tablette/demande-collecte-et-creation-reference.md).
{% endhint %}

## Les statuts d'une demande

| Statut                     | Signification                                                                                |
| -------------------------- | -------------------------------------------------------------------------------------------- |
| **Brouillon**              | En cours de constitution, pas encore validée.                                                |
| **À traiter**              | Validée. L'ordre de collecte est à traiter.                                                  |
| **Partiellement collecté** | Une partie seulement a été collectée ; un nouvel ordre de collecte a été créé pour le reste. |
| **Collecté**               | Tout a été collecté.                                                                         |

## Le détail d'une demande

Cliquez sur une ligne de la liste pour ouvrir la demande. La flèche à côté de **Valider** donne accès à :

* **Modifier** et **Supprimer** : possibles uniquement en **Brouillon** ;
* **Aller vers l'ordre de collecte** (ou les ordres, en cas de traitement partiel).

{% hint style="warning" %}
Pour supprimer une demande déjà validée, supprimez d'abord son ordre de collecte : la demande repasse en brouillon. Une demande collectée ne peut plus être supprimée.
{% endhint %}

## Retrouver une demande

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Créé par**.
* **Colonnes** : création, validation, créé par, numéro, objet, statut, type.
* Le bouton **Exporter au format CSV** exporte les demandes filtrées.
