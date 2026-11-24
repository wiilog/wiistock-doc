---
description: >-
  Déclarer et suivre les non-conformités constatées sur un arrivage UL ou une
  réception.
---

# Litiges / Qualité

**Chemin :** Qualité › Litiges (suivi) · détail d'un arrivage UL (création)

Une marchandise livrée n'est pas conforme ? Déclarez un litige sur l'arrivage, puis suivez-le jusqu'à sa résolution. Les litiges de réception Stock apparaissent aussi sur cette page.

## Créer un litige

{% stepper %}
{% step %}
### Ouvrir l'arrivage

Ouvrez le [détail de l'arrivage UL](arrivages-unites-logistiques/details-arrivage.md) concerné, puis cliquez sur **Nouveau litige**.
{% endstep %}

{% step %}
### Décrire le litige

Les informations de l'arrivage (fournisseur, transporteur, chauffeur, n° d'arrivage, n° commande / BL, acheteurs) sont reprises automatiquement. Elles ne se modifient pas ici, mais sur l'arrivage.

Renseignez ensuite :

* le **Type** de litige ;
* le **Déclarant** (vous, par défaut) ;
* le **Statut** ;
* les **unité(s) logistique(s)** concernées ;
* si besoin un commentaire, des pièces jointes, et **Urgence ?** pour afficher le litige en rouge.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**. Le litige apparaît sur l'arrivage et dans **Qualité › Litiges**.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Les types et les statuts se paramètrent dans [Litiges - Types](../parametrage/arrivages-ul/litiges-types.md) et [Litiges - Statuts](../parametrage/arrivages-ul/litiges-statuts.md). Selon ce paramétrage, un changement de statut peut envoyer un mail à l'acheteur et au déclarant.
{% endhint %}

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 11.14.09.png" alt="Création d&#x27;un litige"><figcaption></figcaption></figure>

## Faire avancer un litige

Cliquez sur la ligne du litige, que ce soit sur l'arrivage ou dans **Qualité › Litiges**. Vous pouvez alors :

* **requalifier** le type ou l'urgence ;
* **changer le statut** : un statut à l'état _Traité_ clôture le litige ;
* **ajouter ou retirer** des UL ;
* **ajouter un commentaire** avec **Ajouter** : il s'inscrit dans l'**Historique**, ce qui permet d'échanger autour du litige ;
* **joindre des fichiers**, par exemple la photo d'un colis abîmé.

Cliquez sur **Enregistrer** pour valider.

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 11.46.33.png" alt="Modification d&#x27;un litige"><figcaption></figcaption></figure>

## Suivre tous les litiges

La page **Qualité › Litiges** centralise tous les litiges, ceux des arrivages comme ceux des réceptions.

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Origines** (arrivage ou réception), **Déclarant**, **Acheteurs**, **Numéro de litige**, **Type**.
* **Numéro de litige** : **LA** + date + compteur pour un litige d'arrivage, **LR** pour un litige de réception.
* La flèche à côté de **Exporter au format CSV** donne accès à **Gestion des colonnes**. Vous pouvez aussi réordonner les colonnes par glisser-déposer.

<details>

<summary>Colonnes disponibles</summary>

Numéro du litige, Type, N° d'arrivage UL, N° de réception, Acheteur(s), N° commande / BL, N° ligne, Fournisseur, Référence, Déclarant, Créé le, Modifié le, Statut, Dernier historique.

</details>

## Supprimer un litige

Dans le menu **⋮** de la ligne, cliquez sur **Supprimer**, sur l'arrivage ou dans **Qualité › Litiges**. Le litige est supprimé partout.
