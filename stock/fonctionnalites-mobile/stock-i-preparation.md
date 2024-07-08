---
description: >-
  Les préparations servent à transférer les références/articles du stock vers un
  emplacement provisoire.
---

# Stock I Préparation

Dans ce menu vous avez accès aux préparations, créer suite à la validation d'une demande de livraison.

Vous avez la liste sous forme de "carte" avec plusieurs informations :&#x20;

* **Demandeur** : Utilisateur qui a créé la demande de livraison
* **Numéro** (ex : P-20230414170506-01) : Numéro de la préparation avec le format P-aaaammjjhhmmss-n
* **Flux** : Indication du type de livraison
* **Commentaire** : commentaire de la livraison
* **Date attendue** : Date souhaitée de livraison (en fonction de la date la couleur de l'entête change voir [Paramétrage > Terminal mobile > Préparations/Livraisons](../../parametrages/terminal-mobile/preparation-livraison.md))
* **Projet** : Indication du projet de la livraison issu du référentiel projet

{% embed url="https://www.screencast.com/t/ndmrtxBS" %}

## Traitement de la préparation

### Références

Rentrer dans l'ordre de préparation (en cliquant sur la "carte") pour voir le détail des références à préparer.&#x20;

{% embed url="https://www.screencast.com/t/D4wGW69yUFhE" %}
Détails d'une préparation
{% endembed %}

Vous avez la liste des références. Pour passer la référence de l'état _À préparer_ à _Préparer_, il faut scanner ou prendre en photo via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>) le code barre de la référence. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo.

Après le scan de votre référence vous devez valider la quantité prise du stock. Une fois que vous avez scanné les références vous pouvez valider et choisir l'emplacement sur lequel vous faite votre préparation.&#x20;

### Articles

Sur une étiquette d'article vous avez comme info :&#x20;

* **Référence article** : code référence de la référence
* **Libelle** : libellé de l'article
* **Code barre** : Code barre de l'article (ex : ART230400001)&#x20;
* **Emplacement** : Emplacement de l'article&#x20;
* **Quantité** : Quantité demandée

{% hint style="info" %}
Si votre rôle est en **Ajout quantité : Référence**, c'est l'opérateur qui traite la préparation qui va choisir quel article prendre.
{% endhint %}

{% embed url="https://www.screencast.com/t/EEtooZaDrmqP" %}
Préparation d'article
{% endembed %}

Après le scan de votre référence vous devez choisir l'article, puis confirmer la quantité à sortir du stock.

Selon le paramétrage dans [Terminal mobile > Préparation](../../parametrages/terminal-mobile/preparations.md),  Afficher l'écran de suggestion d'article sans sélection manuelle de l'article coché, vous ne pourrez pas sélectionner manuellement un article dans la liste (écran du milieu), il faudra le scanner ou prendre en photo l'article.

{% embed url="https://www.screencast.com/t/lqZKuVOMsWot" %}
Écran de sélection d'article sans sélection manuelle
{% endembed %}

{% hint style="info" %}
Si votre rôle est en **Ajout quantité : Article**, lors de la création de la demande de livraison c'est le demandeur qui choisit l'article à prendre.
{% endhint %}

{% embed url="https://www.screencast.com/t/phiQsBhc0x6K" %}
Préparation d'article
{% endembed %}

Vous avez la liste des références à préparer avec l'article à prendre. Pour passer la référence de l'état _À préparer_ à _Préparer_, il faut scanner ou prendre en photo via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>) le code barre de l'article. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo.

Après le scan de votre article vous devez valider la quantité prise du stock. Une fois que vous avez scanné l'ensemble de vos articles vous pouvez valider et choisir l'emplacement sur lequel vous faites votre préparation.

### Unité logistique (article contenu)

_À venir._

## Ordre de livraison

À la validation d'une préparation l'ordre de livraison se crée au statut "à traiter", il est alors possible de retrouver l'ordre sur le nomade dans [Stock > Livraison](stock-i-livraison.md).

## Mouvement de stock

À la validation de la préparation un mouvement de transfert de stock entre l'emplacement du stock de la référence et l'emplacement de préparation. Il n'y a pas de changement dans les quantités à ce stade là.

* Sur la référence la quantité disponible diminue en fonction de la quantité préparé (la Quantité en stock ne bouge pas)
* Sur l'article, son statut passe à "en transit"
