---
description: Déclarer et suivre un litige sur les articles d'une réception.
---

# Litiges / Qualité

**Chemin :** détail d'une réception › **Liste des litiges** (création) · Qualité › Litiges (suivi)

Un article reçu est abîmé ou non conforme ? Déclarez un litige depuis la réception, puis suivez-le jusqu'à sa résolution.

## Créer un litige

{% stepper %}
{% step %}
### Ouvrir la réception

Ouvrez le [détail de la réception](detail-reception.md), puis cliquez sur **Nouveau litige** dans la zone **Liste des litiges**.
{% endstep %}

{% step %}
### Décrire le litige

| Champ                                | Description                                                                                     |
| ------------------------------------ | ----------------------------------------------------------------------------------------------- |
| **Type\*** / **Statut\***            | Type et statut de départ du litige.                                                             |
| **Acheteur(s)**                      | Acheteurs de la commande : ils peuvent recevoir un mail selon le paramétrage des statuts.       |
| **Déclarant\***                      | Vous, par défaut.                                                                               |
| **Articles\***                       | Articles concernés.                                                                             |
| **Commentaire** / **Pièces jointes** | Précisions, photos…                                                                             |
| **Urgence ?**                        | Affiche le litige en rouge. Automatique si l'article vient d'une ligne de réception en urgence. |
{% endstep %}

{% step %}
### Enregistrer

Le litige apparaît dans la réception (colonnes Type, Statut, Dernier historique) et dans **Qualité › Litiges**, avec un numéro **LR** + date + compteur.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Les types et statuts se paramètrent dans [Paramétrage › Stock › Réceptions](../../../parametrage/receptions.md) (Litiges - Types et Litiges - Statuts).
{% endhint %}

## Faire avancer un litige

Cliquez sur la ligne du litige (dans la réception ou dans **Qualité › Litiges**). Vous pouvez :

* **requalifier** le type ou l'urgence ;
* **changer le statut** : un statut à l'état _Traité_ clôture le litige ;
* modifier l'acheteur, le déclarant, **ajouter ou retirer des articles** ;
* **ajouter un commentaire** avec **Ajouter** : il s'inscrit dans l'**Historique** (utilisateur, date, commentaire, statut, type) ;
* joindre des fichiers.

Le tableau **Articles** récapitule les articles en litige (code, statut, libellé, référence, quantité). Cliquez sur **Enregistrer**.

## Suivre tous les litiges

La page **Qualité › Litiges** centralise les litiges de réception et d'arrivage : filtres, colonnes et export sont décrits dans [Litiges / Qualité (Trace)](../../../../trace/fonctionnalites-web/litiges-qualite.md#suivre-tous-les-litiges).

## Supprimer un litige

Dans le menu **⋮** de la ligne, cliquez sur **Supprimer**, dans la réception ou dans **Qualité › Litiges**. Le litige est supprimé partout.
