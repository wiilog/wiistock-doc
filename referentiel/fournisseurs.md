---
description: >-
  Les fournisseurs font partis du référentiel de l'application. Ils sont
  utilisés par les 2 briques de l'application.
---

# Fournisseurs

Ces derniers sont consultables dans l'onglet **Référentiel**, puis **Fournisseurs**. Cette page contient plusieurs éléments :&#x20;

* Une **recherche rapide**, permettant de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Nouveau fournisseur**</mark>, pour créer un nouveau fournisseur
* Un **tableau**, regroupant les différents fournisseurs créés

### Contenu du tableau

<table><thead><tr><th width="258.5">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Nom</strong></td><td>Nom du fournisseur</td></tr><tr><td><strong>Code de référence</strong></td><td>Code du fournisseur</td></tr><tr><td><strong>Possible douane</strong></td><td>Fournisseur livrant régulièrement des colis sous douane. Utilisé sur les arrivages<br>Oui/Non</td></tr><tr><td><strong>Urgent</strong></td><td>Fournisseur livrant régulièrement des colis à traiter en urgence. Utilisé sur les arrivages<br>Oui/Non</td></tr></tbody></table>

### Créer un nouveau fournisseur

Pour créer un nouveau fournisseur, cliquez sur <mark style="background-color:blue;">**Nouveau fournisseur**</mark>. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* Le **nom** du fournisseur, obligatoire
* Le **code de référence** du fournisseur, obligatoire
* La checkbox **Possible douane** : si elle est cochée, à la validation d'un arrivage avec ce fournisseur, une modale va apparaître demandant si l'arrivage doit être modifié (voir [Arrivages](../trace/parametrages/arrivages-ul.md))
* La checkbox **Urgent** : si elle cochée, à la validation d'un arrivage avec ce fournisseur, une modale va apparaître signifiant que les colis de ce fournisseur sont à traiter en urgence, plus l'arrivage est affiché en urgence (voir [Arrivages](../trace/parametrages/arrivages-ul.md))

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider l'ajout du fournisseur. Il pourra ainsi être utilisé sur tous les formulaires de l'application où un fournisseur est demandé.

Il est possible de créer un fournisseur directement dans la modale de création d'un arrivage ou d'une réception.

### Modifier un fournisseur

Pour modifier un fournisseur, cliquez sur la ligne de fournisseur à modifier pour ouvrir la modale de modification.

Modifiez ensuite les champs de la même façon qu'à la création et cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>.&#x20;

### Supprimer un fournisseur

Il est également possible de supprimer un fournisseur en cliquant sur les <img src="../.gitbook/assets/3points" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression du fournisseur.&#x20;

{% hint style="info" %}
Si le fournisseur est déjà utilisé dans l'application, vous ne pourrez pas le supprimer et une modale d'erreur apparaîtra.
{% endhint %}
