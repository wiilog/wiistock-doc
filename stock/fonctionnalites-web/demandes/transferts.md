---
description: >-
  Demander le déplacement de références ou d'articles d'un emplacement à un
  autre, sans sortie de stock.
---

# Transferts

**Chemin :** Demande › Transfert · création avec le bouton **+** du bandeau, puis **Transfert**

Une demande de transfert sert à faire déplacer des références ou des articles d'un emplacement à un autre. La quantité en stock ne change pas. Une fois validée, elle crée un [ordre de transfert](../ordres/transferts.md).

## Créer une demande de transfert

{% stepper %}
{% step %}
### Créer l'entête

Cliquez sur le bouton **+** du bandeau, puis sur **Transfert**. Renseignez l'**Origine** et la **Destination** (obligatoires), et si besoin un **Commentaire**. Cliquez sur **Enregistrer** : la demande est créée en **Brouillon**.

Une demande de transfert n'a pas de type.
{% endstep %}

{% step %}
### Ajouter les références ou articles

Cliquez sur **Ajouter un article**, puis choisissez la **Référence** :

* **gérée à la référence** : elle doit se trouver sur l'emplacement d'origine. Toute sa quantité sera transférée ;
* **gérée à l'article** : choisissez ensuite l'**article** à transférer, parmi ceux disponibles sur l'emplacement d'origine.

Cliquez sur **Ajouter**, et recommencez si besoin.
{% endstep %}

{% step %}
### Valider

Cliquez sur **Valider** : la demande passe **à traiter** et l'ordre de transfert est créé.
{% endstep %}
{% endstepper %}

## Les statuts d'une demande

| Statut        | Signification                                 |
| ------------- | --------------------------------------------- |
| **Brouillon** | En cours de constitution, pas encore validée. |
| **À traiter** | Validée. L'ordre de transfert est à traiter.  |
| **Traité**    | Tout a été transféré.                         |

## Le détail d'une demande

Cliquez sur une ligne de la liste pour ouvrir la demande. Un clic sur une ligne d'article ouvre la fiche de la référence ou de l'article. La flèche à côté de **Valider** donne accès à :

* **Modifier** (destination et commentaire) et **Supprimer** : possibles uniquement en **Brouillon** ;
* **Aller vers l'ordre de transfert**.

Pour supprimer une demande à traiter, supprimez d'abord son ordre de transfert : la demande repasse en brouillon.

## Retrouver une demande

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Créé par**.
* **Colonnes** : numéro (**DT** + date + compteur), statut, créé par, origine, destination, date de création, date de validation.
* Le bouton **Exporter au format CSV** exporte les demandes filtrées.
