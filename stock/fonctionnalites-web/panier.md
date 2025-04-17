---
description: >-
  Le panier permet de réaliser plusieurs demandes de stock de façon rapide et
  ergonomique.
---

# Panier

{% hint style="info" %}
Dans le panier, l'ajout d'une quantité d'une référence se fera toujours à la référence, et pas à l'article, c'est-à-dire que le demandeur viendra demander une quantité globale et n'indiquera pas précisément les articles à se faire livrer si la référence demandée est en gestion quantité par article.
{% endhint %}

Le panier est constitué de 2 zones : une **zone Demande**, qui permet de choisir quel type de demande l'on souhaite créer et ses caractéristiques, et une **zone Références**, qui contient les références et le choix de la quantité à mettre dans la demande. Selon le type de demande choisi, les zones n'afficheront donc pas les mêmes informations.

{% embed url="https://www.screencast.com/t/kXgWKBbR27X" %}

## Type de demande : Livraison

### Partie Demande

Lorsque vous sélectionnez la livraison, vous avez le choix entre 2 radios boutons :&#x20;

* <mark style="background-color:blue;">**Ajouter à une de mes demandes en brouillon**</mark> : sélectionnez ce bouton pour ajouter vos références du panier dans une demande en brouillon dont vous êtes le demandeur
* <mark style="background-color:blue;">**Créer une nouvelle demande**</mark> : sélectionnez ce bouton pour créer une nouvelle demande de livraison

Si vous choisissez d'ajouter à une **demande en brouillon**, vous aurez les informations suivantes :&#x20;

* **Mes livraisons** : sélectionnez la demande de livraison sur laquelle vous souhaitez ajouter vos références. Les demandes proposées sont celles en brouillon dont vous êtes le demandeur. Vous disposez des informations suivantes dans le select :&#x20;
  * N° de la demande - Type de la demande - Emplacement de destination - Date et heure de création

Une fois la demande choisie, les informations de la demande de livraison apparaissent :&#x20;

* **Champs libres** : champs libres de la demande de livraison
* **Commentaire** : commentaire de la demande de livraison
* **Références présentes dans la demande** : références et libellés des références déjà présentes dans la demande de livraison avec la quantité à livrer

{% embed url="https://www.screencast.com/t/boqi42H7nP" %}
Ajouter à une demande de livraison
{% endembed %}

Si vous choisissez de **créer une nouvelle demande**, les champs suivants apparaitront :&#x20;

* **Type\*** : type de la demande de livraison
* **Destination** : emplacement de livraison. Le champ n'est pas disponible tant que le type de la livraison n'est pas sélectionné, car selon le type sélectionné, seuls certains emplacements peuvent être autorisés. A la sélection du type, la destination peut être automatiquement renseignée si un emplacement de livraison par défaut a été paramétré pour ce type ([Paramétrages > Stock > Demandes > Livraisons](../parametrage/demandes/livraisons/))
* **Champs libres** : champs libres du type de la demande de livraison
* **Commentaire** : commentaire sur la demande de livraison

{% embed url="https://www.screencast.com/t/cbfpxixYj3Z" %}
Créer une demande de livraison
{% endembed %}

### Partie Références

Chaque référence est matérialisé par un rectangle. La couleur de l'extérieure du rectangle est celle du type de la référence.

Sur la partie de gauche, il y a le **code de la référence**, et dessous le **libellé de la référence**.

Sur la zone du milieu, la **quantité disponible** de la référence est visible, avec dessous l'ensemble des **références articles fournisseurs**.

Sur la zone à droite, le champ **Quantité à livrer\*** est à compléter. Vous ne pouvez pas mettre moins qu'1, et plus que la quantité disponible. Si le champ est complétement grisé, cela signifie que la quantité disponible est égale à 0. Cette référence ne peut donc pas être livrée et doit être enlever du panier.

A droite du rectangle de la référence, un bouton avec une icône poubelle permet de venir enlever les références du panier.

{% embed url="https://www.screencast.com/t/TdaIaSqngTKO" %}
Référence à livrer
{% endembed %}

Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> pour créer votre livraison en _Brouillon_ ou mettre à jour une demande. Vous serez redirigé vers le détail de la demande de livraison. Validez là pour la sortir de l'état Brouillon et qu'elle soit prise en compte.

## Type de demande : Collecte

### Partie Demande

Lorsque vous sélectionnez la collecte, vous avez le choix entre 2 radios boutons :&#x20;

* <mark style="background-color:blue;">**Ajouter à une de mes demandes en brouillon**</mark> : sélectionnez ce bouton pour ajouter vos références du panier dans une demande en brouillon dont vous êtes le demandeur
* <mark style="background-color:blue;">**Créer une nouvelle demande**</mark> : sélectionnez ce bouton pour créer une nouvelle demande de collecte

Si vous choisissez d'ajouter à une **demande en brouillon**, vous aurez les informations suivantes :&#x20;

* **Mes collectes** : sélectionnez la demande de collecte sur laquelle vous souhaitez ajouter vos références. Les demandes proposées sont celles en brouillon dont vous êtes le demandeur. Vous disposez des informations suivantes dans le select :&#x20;
  * N° de la demande - Type de la demande - Emplacement de collecte - Date et heure de création

Une fois la demande choisie, les informations de la demande de collecte apparaissent :&#x20;

* **Destination** : demande de collecte de destruction ou de mise en stock
* **Objet** : objet de la demande de collecte
* **Champs libres** : champs libres de la demande de collecte
* **Commentaire** : commentaire de la demande de collecte
* **Références présentes dans la demande** : références et libellés des références déjà présentes dans la demande de collecte avec la quantité à collecter

Si vous choisissez de **créer une nouvelle demande**, les champs suivants apparaitront :&#x20;

* **Type\*** : type de la demande de collecte
* **Objet\*** : objet de la demande de collecte. Champ texte
* **Point de collecte**: emplacement de collecte. Le champ n'est pas disponible tant que le type de la collecte n'est pas sélectionné, car selon le type sélectionné, seuls certains emplacements peuvent être autorisés
* **Destination\*** : _Destruction_ ou _Mise en stock_. La mise en stock créera un mouvement d'entrée en stock pour les références collectées, contrairement à la destruction qui ne créera aucun mouvement
* **Champs libres** : champs libres du type de la demande de collecte
* **Commentaire** : commentaire sur la demande de collecte

### Partie Références

La partie Référence est pratiquement la même que sur les demandes de livraison.&#x20;

Seul le texte sur la quantité change. Il y a Quantité à collecter et non plus Quantité à livrer.&#x20;

Il n'y a pas de quantité maximale. La quantité minimale est aussi de 1. Et il est possible de demande à collecter une référence dont la quantité disponible est égale à 0.



Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> pour créer votre collecte en _Brouillon_ ou mettre à jour une demande. Vous serez redirigé vers le détail de la demande de collecte. Validez là pour la sortir de l'état Brouillon et qu'elle soit prise en compte.

## Type de demande : Achat

### Partie Demande

Pour les achats, aucun élément à sélectionner dans la partie Achat car il n'y a pas de champs fixes ou libres à indiquer sur une demande d'achat. Pour le choix d'ajouter à une demande existante ou d'en créer une nouvelle, cette partie se fait sur la partie des références pour les demandes d'achat.

### Partie Référence

Pour les demandes d'achat, les références sont classées par acheteur.

Sous chaque section avec un acheteur différent, un select **Mes demandes d'achat** vous permet de choisir si vous souhaitez créer une nouvelle demande d'achat ou bien ajouter les références à une demande d'achat déjà existante.

Si vous souhaitez **créer une nouvelle demande** pour un lot des références ayant un même acheteur, laissez le select sur _Créer une demande d'achat_

Si vous souhaitez _ajouter à une demande d'achat existante_ un lot des références ayant un même acheteur, sélectionnez la demande parmi celles proposées. Sont proposées seulement les demandes avec le même acheteur, le même demandeur que l'utilisateur de la session en cours, et en statut Brouillon. Vous disposez des informations suivantes dans le select :

* N° de demande d'achat - Date et heure de création de la demande

{% embed url="https://www.screencast.com/t/WiiaC1R11kAY" %}
Demande d'achat
{% endembed %}

Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> pour créer les demandes d'achat au statut _Brouillon_. Si vous avez créé ou mis à jour une demande d'achat, vous serez redirigé vers le détail de la demande d'achat. Validez là pour la sortie de l'état Brouillon et qu'elle soit prise en compte. Si vous avez créé ou mis à jour plusieurs demandes d'achat, vous serez redirigé vers la liste des demandes d'achat.

Si votre panier contient des références n'ayant pas d'acheteur, les références seront ignorées lors de la validation du panier de demande d'achat.
