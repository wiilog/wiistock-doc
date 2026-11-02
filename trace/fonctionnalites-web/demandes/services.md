---
description: >-
  Demander une intervention sur le site logistique (réparation, manutention,
  assistance…) et suivre son traitement.
---

# Services

**Chemin :** Demande › Service · création avec le bouton **+** du bandeau, puis **Service**

Une demande de service sert à demander une opération qui ne concerne pas le stock : réparer du mobilier, déplacer une machine, demander de l'aide… L'équipe concernée la traite (sur le web ou le nomade) et fait avancer son statut.

## Créer une demande de service

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur le bouton **+** du bandeau, puis sur **Service**.

<figure><img src="../../../.gitbook/assets/image (34).png" alt="Menu de création rapide"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Renseigner la demande

Les champs obligatoires sont : **Type**, **Statut** et **Date attendue**. Les statuts proposés dépendent du type choisi.

Complétez si besoin : **Objet**, **Urgences**, **Chargement**, **Déchargement**, **Nombre d'opération(s) réalisée(s)**, **Destinataires**, champs libres, commentaire et pièces jointes. Le champ **Créé par** est prérempli avec votre nom.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer** : la demande apparaît dans la liste.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Les types, statuts et champs se paramètrent dans [Paramétrage › Trace › Services](../../parametrage/services/).
{% endhint %}

## Suivre une demande et changer son statut

Cliquez sur une ligne de la liste pour ouvrir la demande :

* **à gauche** : les informations de la demande, l'urgence, les pièces jointes et le commentaire ;
* **à droite** : la **timeline des statuts** et les dates (attendue, de réalisation).

Pour faire avancer la demande, cliquez sur **Changer le statut**, choisissez le nouveau statut, puis cliquez sur **Enregistrer**. La timeline se met à jour.

{% hint style="warning" %}
Une fois la demande traitée, son statut ne peut plus être changé.
{% endhint %}

## Modifier ou supprimer une demande

* **Modifier** : depuis le menu **⋮** de la liste, ou avec le bouton **Modifier** du détail. Le type, le statut et la date de réalisation ne sont pas modifiables. Il faut avoir le droit de modification.
* **Supprimer** : depuis le menu **⋮** de la liste ou du détail, après confirmation.

## Retrouver une demande

* **Filtres** : période (la flèche permet de choisir la date de création, la date attendue ou la date de réalisation), **Type**, **Statuts**, **Créé par**, **Destinataires**, **Objet**.
* La flèche à côté de **Exporter au format CSV** donne accès à **Gestion des colonnes**.

<details>

<summary>Colonnes disponibles</summary>

Numéro de demande, Date demande, Type, Créé par, Objet, Date attendue, Date de réalisation, Statut, Urgent, Nombre d'opération(s) réalisée(s), Traité par, Destinataires.

</details>
