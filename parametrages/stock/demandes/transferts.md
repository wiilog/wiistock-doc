---
description: >-
  La demande de transfert sert à demander à transférer une référence ou un
  article d'emplacement, sans sortie de stock
---

# Transferts

&#x20;Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Demande**</mark>, puis <mark style="background-color:blue;">**Transferts**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes de transfert créées

{% embed url="https://www.screencast.com/t/cVniCJqGMh" %}
Page demande de transfert
{% endembed %}

### Contenu des filtres

| Filtre         | Description                                                                  |
| -------------- | ---------------------------------------------------------------------------- |
| **Du**         | La tranche basse filtrant sur la date de création de la demande de transfert |
| **Au**         | La tranche haute filtrant sur la date de création de la demande de transfert |
| **Statuts**    | Statut de la demande de transfert                                            |
| **Demandeurs** | Personne ayant créée la demande de transfert                                 |
| **Opérateurs** | Opérateurs ayant traités la demande de transfert                             |

### Contenu du tableau

| Colonne                | Description                                                                                                                                                |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro**             | Numéro de la demande de transfert. Ce numéro est constitué du préfixe DT- avec ensuite l'année, le mois, le jour de création de la demande, et un compteur |
| **Statut**             | Statut de la demande de transfert                                                                                                                          |
| **Demandeur**          | Personne ayant créée la demande de transfert                                                                                                               |
| **Origine**            | Emplacement où se situe les références / les articles qui doivent être transférés                                                                          |
| **Destination**        | Emplacement où les références / les articles doivent être déplacés                                                                                         |
| **Date de création**   | Date de création de la demande de transfert                                                                                                                |
| **Date de validation** | Date de validation de la demande de transfert (passage du statut _Brouillon_ à _A traiter_)                                                                |

### Créer une demande de transfert

Dans le bouton d'action rapide, sélectionnez <mark style="background-color:blue;">**Transfert**</mark> pour créer une demande de transfert.

![](<../../../.gitbook/assets/image (81).png>)

Une modale s'ouvrira alors pour remplir les informations d'entête de la demande :&#x20;

* **Demandeur** : champ non modifiable. Il contient le nom de la personne ayant créée la demande
* **Origine\*** : emplacement duquel les références / articles doivent être déplacées
* **Destination\*** : emplacement vers lequel les références / articles doivent être déplacées
* **Commentaire** : commentaire sur la demande

{% hint style="info" %}
Contrairement aux collectes ou aux livraisons, une demande de transfert n'a pas de type
{% endhint %}

Une fois que vous avez au moins renseigné tous les champs obligatoires(\*), cliquez sur <mark style="background-color:blue;">**Créer la demande**</mark> pour créer la demande en statut _**Brouillon**_ et être redirigé vers le détail de la demande.

Le **détail** est constitué de :&#x20;

* une **entête**. Elle contient les différents champs renseignés précédemment ainsi que la date de création et de validation&#x20;
* le **tableau** de la **liste des articles**, qui a les colonnes suivantes :&#x20;

| Colonne        | Description                                        |
| -------------- | -------------------------------------------------- |
| **Référence**  | Référence à transférer                             |
| **Code barre** | Code barre article ou de la référence à transférer |
| **Quantité**   | Quantité de la référence ou de l'article           |

Pour ajouter un article, cliquez sur <mark style="background-color:blue;">**Ajouter un article**</mark>

Une modale s'ouvrira alors. Tapez dans un premier temps le code de la référence. La référence doit être sur l'emplacement d'origine dans le cas d'une référence en gestion quantité par référence. Dans le cas d'une référence en gestion quantité par article, au moins un des articles de la référence en état disponible doit être présent sur l'emplacement d'origine.

Pour les **références en gestion quantité par référence**, il n'y a pas d'autres champs à renseigner. Cliquez sur <mark style="background-color:blue;">**Ajouter**</mark> pour ajouter la référence dans la demande de transfert. Ainsi, l'ensemble de la quantité de la référence sera transférée vers l'emplacement de destination. La colonne _Quantité_ est remplie avec toute la quantité en stock de la référence. La colonne _Code barre_ est remplie avec le code barre de la référence (en REF).

Pour les **références en gestion quantité par article**, vous devez sélectionner l'article à transférer après avoir sélectionné la référence. Seul les articles présents sur l'emplacement d'origine de la demande seront proposés. Cliquez sur <mark style="background-color:blue;">**Ajouter**</mark> ensuite pour ajouter l'article à la demande de transfert. La quantité mise dans le tableau sera la quantité totale de l'article sélectionné. Le code barre mis dans le tableau sera le code barre de l'article sélectionné (en ART).

Cliquez sur le bouton <mark style="background-color:blue;">**Valider**</mark> après avoir ajouté toutes les références et/ou tous les articles que vous souhaitez transférer.&#x20;

Un ordre de transfert sera alors généré et la demande de transfert passera en A traiter.&#x20;

{% embed url="https://www.screencast.com/t/bF2DlrhKVoFz" %}
Demande de transfert en gestion quanté par aticle
{% endembed %}

### Modifier une demande de transfert

Il est possible de modifier une demande de transfert tant que celle-ci est en brouillon.

Pour cela, cliquez sur la flèche à droite de **Valider**, et sur <mark style="background-color:blue;">**Modifier**</mark>. Vous aurez ensuite la possibilité de modifier la destination du transfert, et son commentaire.

<mark style="background-color:blue;">**Enregistrer**</mark> pour valider les modifications

### Supprimer une demande de transfert

La suppression d'une demande de transfert est directement possible si celle-ci est en brouillon.

Pour cela, cliquez sur la flèche à droite de **Valider**, et sur <mark style="background-color:blue;">**Supprimer**</mark>.&#x20;

La demande sera alors supprimée.

Si la demande est en statut à traiter, il vous faudra supprimer l'ordre de transfert pour que la demande liée soit passée en état brouillon et qu'elle soit supprimable à son tour.

### Visualiser une demande de transfert

Pour accéder au détail de la demande de transfert, cliquez sur la ligne de la demande que vous souhaitez voir. Vous arriverez alors sur le détail de la demande.&#x20;

Dans l'entête de la demande, vous avez une flèche qui donne accès aux boutons <mark style="background-color:blue;">**Aller vers l'ordre de transfert**</mark>**.**&#x20;

En cliquant sur ces boutons, vous serez redirigé vers le détail de l'ordre de transfert.

Vous pouvez cliquez sur la ligne d'un article / d'une référence également dans le tableau pour ouvrir le détail d'un article de référence ou le détail d'un article selon la gestion quantité de la référence cliquée.&#x20;

{% embed url="https://www.screencast.com/t/qPek9aYpH1" %}
Depuis une demande de tranfert aller vers son ordre
{% endembed %}

### Workflow d'une demande de transfert

Une demande de transfert passe par les statuts suivants :&#x20;

* **brouillon** : la demande vient d'être créer mais est toujours en cours de constitution. Elle n'a pas été encore validée
* **à traiter** : la demande a été validée et doit être traitée. L'ordre de transfert a été générée, il est en statut à traiter (Documentation Ordre de transfert : [Stock > Ordres > Transfert](../../../stock/fonctionnalites-web/ordres/transferts.md))
* **traité** : toutes les références et les articles demandées sont transférés. L'ordre de transfert est traité ce qui passe la demande à _Traité_
