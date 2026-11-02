---
description: >-
  Demander la livraison d'une ou plusieurs références depuis le stock, puis
  suivre la demande jusqu'à la livraison.
---

# Livraisons

**Chemin :** Demande › Livraison · création avec le bouton **+** du bandeau, puis **Livraison**

Une demande de livraison sert à se faire livrer des références du stock. Une fois validée, elle crée un [ordre de préparation](../ordres/preparations.md), puis un [ordre de livraison](../ordres/livraisons.md). La quantité en stock diminue à la livraison.

## Créer une demande de livraison

{% stepper %}
{% step %}
### Créer l'entête

Cliquez sur le bouton **+** du bandeau, puis sur **Livraison**. Renseignez :

* le **Type** : il détermine les champs libres et les emplacements autorisés ;
* la **Destination** : l'emplacement de livraison, éventuellement prérempli selon le type ;
* le **Destinataire** ;
* si besoin la **Date attendue**, le **Projet** et un **Commentaire**.

Cliquez sur **Enregistrer** : la demande est créée en **Brouillon** et sa fiche s'ouvre.
{% endstep %}

{% step %}
### Ajouter les références

Dans **Liste des articles**, remplissez directement la ligne du tableau : **Référence**, **Quantité**, et si besoin **Remarques** et **Projets**. Le code-barre, le libellé et l'emplacement se complètent automatiquement. Cliquez sur **+** pour ajouter une ligne, et sur la corbeille pour en retirer une.
{% endstep %}

{% step %}
### Valider

Cliquez sur **Valider** : la demande passe **à traiter** et l'ordre de préparation est créé.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Autres façons de créer une demande de livraison :**

* depuis le [panier](../panier.md), après avoir ajouté des références ;
* par import, dans [Paramétrage › Données › Imports & mises à jour](../../../parametrages/donnees/imports-and-mises-a-jour.md) ;
* depuis une tablette, avec la [demande de livraison rapide](../../fonctionnalites-borne-tablette/demande-de-livraison-rapide.md).
{% endhint %}

## Les statuts d'une demande

| Statut                    | Signification                                                                             |
| ------------------------- | ----------------------------------------------------------------------------------------- |
| **Brouillon**             | En cours de constitution, pas encore validée.                                             |
| **À traiter**             | Validée. L'ordre de préparation est à traiter.                                            |
| **Partiellement préparé** | Une partie seulement a été préparée ; une nouvelle préparation a été créée pour le reste. |
| **Préparé**               | La préparation est terminée. L'ordre de livraison est à traiter.                          |
| **Livré partiellement**   | Une partie seulement a été livrée.                                                        |
| **Livré**                 | Tout a été livré.                                                                         |

## Le détail d'une demande

Cliquez sur une ligne de la liste pour ouvrir la demande : statut, créateur, destinataire, destination, date et type, puis la **liste des articles**.

La flèche à côté de **Valider** donne accès aux actions :

* **Modifier** et **Supprimer** : possibles uniquement en **Brouillon** ;
* **Aller vers l'ordre de préparation** / **Aller vers l'ordre de livraison** (au pluriel en cas de traitement partiel) ;
* **Aller vers la réception** : si la demande a été générée par une réception.

{% hint style="warning" %}
**Supprimer une demande déjà validée** : supprimez d'abord l'ordre de livraison, puis l'ordre de préparation. La demande repasse en brouillon et peut alors être supprimée. Une demande livrée ne peut plus être supprimée.
{% endhint %}

## Retrouver une demande

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Créé par**, **Destinataires**.
* La flèche à côté de **Exporter au format CSV** donne accès à **Gestion des colonnes**.
* Le **numéro** d'une demande commence par **DL**, suivi de la date et d'un compteur.
