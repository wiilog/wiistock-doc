---
description: >-
  Regrouper des références dans un panier pour créer rapidement une demande de
  livraison, de collecte ou d'achat.
---

# Panier

**Chemin :** icône **panier** du bandeau

Le panier sert à créer une demande de stock en quelques clics. Ajoutez d'abord des références au panier depuis la page [Références](references.md) ou [Alertes](alertes.md) (icône panier), puis choisissez le type de demande.

{% hint style="info" %}
Dans le panier, vous demandez toujours une **quantité de référence**, jamais un article précis, même si la référence est gérée à l'article.
{% endhint %}

## Faire une demande de livraison

{% stepper %}
{% step %}
### Choisir le type de demande

Dans **Type de demande**, sélectionnez **Livraison**.
{% endstep %}

{% step %}
### Créer ou compléter une demande

* **Créer une nouvelle demande** : choisissez le **Type**, puis la **Destination** (elle peut se remplir automatiquement selon le type), et si besoin les champs libres et un commentaire.
* **Ajouter à une de mes demandes en brouillon** : choisissez la demande dans **Mes livraisons**. Ses informations et ses références s'affichent.
{% endstep %}

{% step %}
### Indiquer les quantités

Pour chaque référence, saisissez la **Quantité à livrer** : au moins 1, et au plus la quantité disponible. Une référence dont la quantité disponible est à 0 ne peut pas être livrée ; retirez-la avec l'icône corbeille.
{% endstep %}

{% step %}
### Valider

Cliquez sur **Valider mon panier**. Vous arrivez sur la demande, au statut **Brouillon** : validez-la pour qu'elle soit traitée.
{% endstep %}
{% endstepper %}

## Faire une demande de collecte

Le fonctionnement est le même que pour une livraison, avec ces différences :

* pour une nouvelle demande, renseignez le **Type**, l'**Objet**, le **Point de collecte** et la **Destination** : **Mise en stock** (crée une entrée en stock) ou **Destruction** (aucun mouvement de stock) ;
* la **Quantité à collecter** n'a pas de maximum, et une référence à 0 en stock peut être collectée.

## Faire une demande d'achat

* Les références sont regroupées **par acheteur**. Les références sans acheteur sont ignorées.
* Pour chaque acheteur, la liste **Mes demandes d'achat** permet de **créer une demande d'achat** ou d'ajouter les références à l'une de vos demandes en brouillon pour ce même acheteur.
* Cliquez sur **Valider mon panier**. Les demandes sont créées en **Brouillon** : validez-les pour qu'elles soient prises en compte.

Voir [Achats](demandes/achats.md).
