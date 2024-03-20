# Stock I Collecte

Dans ce menu vous avez accès aux collectes, créer suite à la validation d'une demande de collecte sur le web. Sur le nomade vous allez pouvoir traiter cette collecte.

Vous avez la liste sous forme de "carte" avec plusieurs informations :&#x20;

* **Demandeur** : Utilisateur qui a créé la demande de collecte
* **Numéro** (ex : C-20230414170506) : Numéro de la collecte avec le format C-aaaammjjhhmmss
* **Flux** : Indication du type de collecte
* **Point de collecte** : Emplacement de collecte des références
* **Destination** : 2 choix "Mise en stock" ou "Destruction" : La mise en stock rentre dans le stock la référence, la destruction n'a pas d'impact sur le stock.

## Traitement de la collecte

Rentrez dans le détail d'un ordre de collecte, vous aller avoir des informations de la collecte dans l'entête :&#x20;

* Numéro de l'ordre de collecte&#x20;
* Point de collecte
* Commentaire
* Indication de Mise en stock ou Destruction

Puis 2 encarts "Collecté" et "À collecter" qui contient la liste des références / articles à collecter. Au fur et à mesure que vous scannez vos références, elles vont se transférer dans "Collecté". Cela indique que vous les avez bien collectés.

Pour passer une référence / articles de "À collecter" à "Collecté" vous pouvez scanner ou prendre en photo (via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>)) le Code barre. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo.&#x20;

Si vous scannez un code barre référence ou un code barre article vous aller avoir des options différentes :

### Références

Vous avez scanné le code barre de la référence, l'étape d'après est de confirmer la quantité prise, puis de <mark style="background-color:blue;">**Valider**</mark>. Une fois l'ensemble des références collectées <mark style="background-color:blue;">**Valider**</mark>.

{% embed url="https://www.screencast.com/t/RjbSs8gyPGK" %}
Flux collecte d'une référence
{% endembed %}

### Articles

{% hint style="info" %}
Si votre rôle est en **Ajout quantité : Référence**, c'est l'opérateur qui traite la collecte qui va choisir quel article prendre ou créer un nouvel article.
{% endhint %}

Vous avez scanné le code barre de la référence, vous pouvez scanner un code barre article (issus des articles déjà consommés (consommé depuis max 3 mois)) ou le sélectionner via la loupe. Si vous ne voulez pas remettre un article déjà consommé en stock vous pouvez cliquer sur <mark style="background-color:blue;">**Générer nouvel article**</mark>, cela vous créera alors un article.

L'étape d'après est de confirmer la quantité prise, puis <mark style="background-color:blue;">**Valider**</mark>

{% embed url="https://www.screencast.com/t/EVxl3THLjcH" %}
Flux collecte d'un article consommé
{% endembed %}

{% hint style="info" %}
Si votre rôle est en **Ajout quantité : Article**, lors de la création de la demande de collecte c'est le demandeur qui choisit l'article à prendre ou bien de créer un nouvel article.
{% endhint %}

Vous avez scanné le code barre de l'article, l'étape d'après est de confirmer la quantité prise, puis de <mark style="background-color:blue;">**Valider**</mark>. Une fois l'ensemble des articles collectés <mark style="background-color:blue;">**Valider**</mark>.

{% embed url="https://www.screencast.com/t/iU4pb3z2aS" %}
Flux collecte d'un article
{% endembed %}

## Dépose des références et articles

**Mise en stock**

Quand vous avez fini de passer toutes les références/articles dans l'encart "Collecté" cliqué sur <mark style="background-color:blue;">**Valider**</mark>. Un message pop-up apparait vous indique que pour valider l'entrée en stock vous devez effectuer une dépose. Un bouton vous redirige vers le menu de dépose (Transfert manuel ⎮ Dépose). Vous devez choisir l'emplacement sur lequel déposer vos références/articles, scanner les références/articles qui correspondent à cet emplacement et Valider. \
Vous venez de finaliser la collecte.

{% embed url="https://www.screencast.com/t/ygTEXx8kAyx" %}

**Destruction**

Quand vous avez fini de passer toutes les références/articles dans l'encart "Collecté" cliqué sur <mark style="background-color:blue;">**Valider**</mark>. Vous venez de finaliser la collecte, aucun mouvement ne se créer et la quantité en stock de la référence ne change pas.

## Mouvement de stock

**Mise en stock**

Un mouvement d'entrée de stock se créer et la référence vient de s'incrémenter de la quantité collectée.&#x20;

Un mouvement d'entrée de stock de l'article se créer, si vous avez sélectionné un article consommé il est de nouveau disponible. La référence vient de s'incrémenter de la quantité collectée.&#x20;
