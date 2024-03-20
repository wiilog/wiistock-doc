---
description: >-
  Les mouvements de stock sont tous les mouvements d'entrées, de transferts, et
  de sorties de stock qui résultent des différentes demandes et réceptions sur
  l'application.
---

# Mouvements de stock

&#x20;Cette page est disponible dans le menu **Stock**, puis **Mouvements de stock**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Nouveau mouvement**</mark> pour créer un nouveau mouvement de stock
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, sous le bouton Nouveau mouvement, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différents mouvements

{% embed url="https://www.screencast.com/t/2mAcbOlv" %}
Page mouvements de stock
{% endembed %}

## Contenu des filtres

<table><thead><tr><th width="376.5">Filtre</th><th>Description</th></tr></thead><tbody><tr><td><strong>Du</strong></td><td>La tranche basse filtrant sur la date de création du mouvements de stock</td></tr><tr><td><strong>Au</strong></td><td>La tranche haute filtrant sur la date de création du mouvements de stock</td></tr><tr><td><strong>Emplacements</strong></td><td>Emplacements d'origine ou de destination des mouvements de stock</td></tr><tr><td><strong>Types</strong></td><td>Types de mouvement</td></tr><tr><td><strong>Utilisateurs</strong></td><td>Utilisateurs ayant réalisés les mouvements</td></tr></tbody></table>

## Contenu du tableau

| Colonne               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Date**              | Date du mouvement de stock                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Issu de**           | <p>Eléments ayant déclenché le mouvement de stock. La plupart de ces éléments sont cliquables et renvoie vers le détail de l'élément. Ces éléments peuvent être : <br>- <em><strong>collecte</strong></em> : l'article ou la référence a été remis en stock suite à une collecte<br>- <em><strong>livraison</strong></em> : l'article ou la référence a été sorti du stock suite à un ordre de livraison<br>- <em><strong>préparation</strong></em> : l'article ou la référence est transféré pour préparation pour la livraison<br>- <em><strong>réception</strong></em> : l'article ou la référence a été rentré en stock suite à sa réception<br>- <em><strong>import</strong></em> : réalisation d'import d'article ou de référence <br>- <em><strong>transfert de stock</strong></em> : l'article ou la référence a été transféré suite à une demande <br>- <em><strong>inventaire</strong></em> : correction de la quantité en stock de l'article ou la référence suite à un inventaire</p> |
| **Code barre**        | Code barre de l'article ou de la référence du mouvement de stock                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Référence article** | Code la référence article ayant le mouvement de stock                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Quantité**          | Quantité de l'article ou la référence sur le mouvement de stock                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Origine**           | Emplacement d'origine du mouvement. Selon le mouvement il peut être vide                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Destination**       | Emplacement de destination du mouvement. Selon le mouvement il peut être vide                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Type**              | <p>Type du mouvement. Les types de mouvements de stock possible sont les suivants : <br>- <em><strong>entrée</strong></em> : entrée d'article ou de référence. Incrément de la quantité en stock<br>- <em><strong>entrée inventaire</strong></em> : correction de quantité positive suite à un inventaire<br>- <em><strong>sortie</strong></em> : sortie d'article ou de référence. Décrément de la quantité en stock<br>- <em><strong>sortie inventaire</strong></em> : correction de quantité négative suite à un inventaire<br>- <em><strong>transfert</strong></em> : déplacement de référence ou d'un article d'un emplacement à un autre. Pas de changement de quantité en stock</p>                                                                                                                                                                                                                                                                                                        |
| **Opérateur**         | Opérateur ayant réalisé le mouvement                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

## Nouveau mouvement de stock

Pour ajouter un nouveau mouvement de stock, cliquez sur le bouton <mark style="background-color:blue;">**Nouveau mouvement**</mark> et compléter la modale qui s'ouvre. Vous devez d'abord remplir le champ **Référence** pour que les autres champs apparaissent :&#x20;

Si la **référence choisie est en gestion quantité par référence**, les champs suivants apparaitront :&#x20;

* **Libellé** : _champ indisponible_, il se remplit automatiquement avec le libellé de la référence choisie
* **Code barre** : _champ indisponible_, il se remplit automatiquement avec le code barre de la référence choisie
* **Emplacement** : _champ indisponible_, il se remplit automatiquement avec l'emplacement de la référence choisie
* **Type\*** : type de mouvement que vous souhaitez faire sur la référence. 3 types sont possibles :&#x20;
  * _**Entrée**_ : pour ajouter une quantité en stock. Le mouvement d'entrée se fera sur l'emplacement de la référence indiqué
  * _**Sortie**_ : pour enlever une quantité du stock. Le mouvement de sortie se fera à partir de l'emplacement de la référence indiqué
  * _**Transfert**_ : pour modifier d'emplacement la référence dans votre stock. Toute la quantité de la référence sera transférée sur l'emplacement indiqué. Il n'est pas possible de réaliser un mouvement de transfert si la référence est présente dans une demande de livraison/collecte/transfert en cours de traitement.&#x20;
* **Quantité disponible** : _champ indisponible_, il se remplit automatiquement avec la quantité en stock de la référence choisie
* **Quantité entrée/sortie\***, _apparaît quand le type entrée ou sortie est sélectionné_ : quantité à entrer ou à sortir de la référence
* **Emplacement\***, _apparaît quand le type transfert est sélectionné_ : emplacement sur lequel transférer la référence

{% embed url="https://www.screencast.com/t/rM35yfcLzj" %}
Mouvement de transfert de stock
{% endembed %}

Si la **référence choisie est en gestion quantité par article**, les champs suivants apparaitront :&#x20;

* **Libellé** : _champ indisponible_, il se remplit automatiquement avec le libellé de la référence choisie
* **Code barre article\*** : choisissez l'article sur lequel vous souhaitez faire un mouvement de stock
* **Emplacement**, _apparaît quand le code barre article est sélectionné_ : _champ indisponible_, il se remplit automatiquement avec l'emplacement de l'article choisie
* **Type**, _apparaît_ _quand le code barre article est sélectionné_. Les types de mouvements possibles sont les mêmes que décrit précédemment. Les mouvements porteront uniquement en revanche sur l'article sélectionné, comme le transfert qui se fera seulement sur l'article et pas sur l'ensemble de la référence
* **Quantité disponible**, _apparaît quand le code barre article est sélectionné_ : _champ indisponible_, il se remplit automatiquement avec la quantité en stock de l'article choisi
* **Quantité entrée/sortie\***, _apparaît quand le code barre article est sélectionné et que le type entrée ou sortie est sélectionné_ : quantité à entrer ou à sortir de l'article
* **Emplacement\***, _apparaît quand le code barre article est sélectionné et que le type entrée ou sortie est sélectionné_ : emplacement sur lequel transférer l'article

{% embed url="https://www.screencast.com/t/sOkjqioUDnmN" %}
Mouvement d'entrée de stock
{% endembed %}

Une fois les informations remplies, <mark style="background-color:blue;">**Enregistrez**</mark> votre mouvement. Vous le retrouverez en haut du tableau, horodaté à l'heure à laquelle vous l'avez créé

{% hint style="info" %}
Il n'est pas possible de modifier un mouvement de stock. Vous pouvez seulement le supprimer
{% endhint %}

## Supprimer un mouvement de stock

Vous pouvez supprimer un mouvement de stock en cliquant sur les<img src="../../.gitbook/assets/3points" alt="" data-size="line">de la ligne du mouvement que vous souhaitez supprimer et en appuyant sur <mark style="background-color:blue;">**Supprimer**</mark>.

Attention, vous ne pouvez pas supprimer le mouvement s'il est lié à des mouvements de traçabilité.&#x20;

{% hint style="info" %}
La suppression d'un mouvement de stock n'entraine pas de modification de la quantité de la référence en stock
{% endhint %}
