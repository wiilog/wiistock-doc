---
description: >-
  La demande de livraison sert à demander à se faire livrer une ou plusieurs
  références et décrémentent donc le stock lorsqu'elle est traitée.
---

# Livraisons

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Demande**</mark>, puis <mark style="background-color:blue;">**Livraisons**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un bouton **Gestion des colonnes**, sous le bouton Exporter au format CSV, pour choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différentes demandes de livraison créées

{% embed url="https://www.screencast.com/t/IhGictNlQQ" %}
Page demande de livraison
{% endembed %}

### Contenu des filtres

| Filtre           | Description                                                                                                                                                                                                                                                                                                |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**           | La tranche basse filtrant sur la date de création de la demande de livraison                                                                                                                                                                                                                               |
| **Au**           | La tranche haute filtrant sur la date de création de la demande de livraison                                                                                                                                                                                                                               |
| **Statuts**      | Le(s) statut(s) des demandes de livraison à filtrer                                                                                                                                                                                                                                                        |
| **Utilisateurs** | Pour filtrer sur la personne ayant créée la demande de livraison. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Type**         | Le type des demandes de livraison à filtrer                                                                                                                                                                                                                                                                |

### Contenu du tableau

| Colonne                | Description                                                                                                      |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Numéro**             | Numéro de la demande de livraison. Il est constitué du préfixe DL, de l'année, du mois, du jour et d'un compteur |
| **Type**               | Le type de la demande de livraison                                                                               |
| **Statut**             | Le statut actuel de la demande de livraison                                                                      |
| **Date de création**   |  La date de création de la demande de livraison                                                                  |
| **Date de validation** | La date de validation de la demande de livraison (passage du statut brouillon à à traiter)                       |
| **Destination**        | Emplacement demandée de livraison                                                                                |
| **Demandeur**          | Personne ayant crée la demande                                                                                   |
| **Commentaire**        | Commentaire renseigné sur la demande                                                                             |

## Créer une demande de livraison

### Via le bouton "+"

Dans le bouton d'action rapide, sélectionnez <mark style="background-color:blue;">**Livraison**</mark> pour créer une demande de livraison.

![](<../../../.gitbook/assets/image (30).png>)

Une modale s'ouvrira alors pour remplir les informations d'entête de la demande :&#x20;

* **Demandeur** : personne créant la demande. Il n'est pas possible de changer ce champ une fois la demande validée. Par défaut, ce champ se remplit avec la personne connectée
* **Type** : type de la demande. Le type permet de venir définir plus précisément le flux de demande. Sa sélection permet de faire apparaître les champs libres associés au type de livraison (pour paramétrer les champs libres : [<mark style="color:blue;">Paramétrage > Stock > Demandes > Livraisons - Types et champs libres</mark>](../../../parametrages/track/demandes/livraison-types-and-champs-libres.md)). Le choix de type conditionne aussi le choix de la destination de 2 façons : l'affichage d'un emplacement par défaut par type de demande de livraison si un paramétrage dans ce sens a été fait ([Paramétrage > Stock > Demandes > Livraisons](../../../parametrages/stock/demandes/livraisons/)) ; la restriction des emplacements possibles à sélectionner. Selon le type, il sera possible de sélectionner seulement les emplacements autorisés sur le type (à aller paramétrer directement sur l'emplacement : [Référentiel > Emplacements](../../../referentiel/emplacements.md)). Le type n'est plus modifiable une fois la demande validée
* **Destination** : une fois le type sélectionné, vous pouvez choisir l'emplacement de livraison. Pour cela, commencez à taper la première lettre de l'emplacement souhaité. Vous pouvez directement faire apparaître les emplacements possibles aussi si le paramétrage "Gérer le champ "Destination" en liste déroulante" est activé ([Paramétrage > Stock > Demandes > Livraisons](../../../parametrages/stock/demandes/livraisons/))
* **Champs libres :** remplissez les champs libres s'il y en a de paramétrés
* **Commentaire :** vous avez également la possibilité d'ajouter un commentaire

En cliquant sur <mark style="background-color:blue;">**Enregistrer**</mark>, la demande de livraison est créée au statut brouillon et vous êtes redirigé vers le **détail de la demande**.

Le **détail** est constitué de :&#x20;

* une **entête**. Elle contient les différents champs renseignés précédemment ainsi que la date de création et de validation&#x20;
* le **tableau** de la **liste des articles**, qui a les colonnes suivantes :&#x20;

| Colonne                       | Description                                                                                                                                                                                                                                                                                                                                                                                    |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Référence**                 | Référence à se faire livrer                                                                                                                                                                                                                                                                                                                                                                    |
| **Code barre**                | Code barre de la référence à se faire livrer ou de l'article précis                                                                                                                                                                                                                                                                                                                            |
| **Libellé**                   | Libellé de la référence à se faire livrer                                                                                                                                                                                                                                                                                                                                                      |
| **Emplacement**               | Emplacement où se situe la référence/l'article                                                                                                                                                                                                                                                                                                                                                 |
| **Emplacement cible picking** | Colonne affichée selon paramétrage. Pour que cette colonne soit affichée, le paramétrage "Faire apparaitre l'emplacement cible de picking à l'ajout d'une référence et dans son traitement" doit être activé ([Paramétrage > Stock > Demandes > Livraisons](../../../parametrages/stock/demandes/livraisons/)). Cet emplacement désigne l'emplacement où le picking de l'article doit se faire |
| **Quantité à prélever**       | Quantité souhaitée à se faire livrer                                                                                                                                                                                                                                                                                                                                                           |

Pour ajouter un article, cliquez sur la flèche à droite de **Chercher une Référence**, et sur <mark style="background-color:blue;">**Ajouter un article**</mark>

Une modale s'ouvrira alors. Tapez le code de la référence pour faire apparaître les autres champs. La modale est constituée de ces champs :&#x20;

* **Référence\*** : référence à se faire livrer
* **Code article\***, _selon paramétrage_ : si la référence est en gestion quantité par article et que votre rôle est en ajout quantité par article, ce champ apparaîtra. Il consiste à choisir précisément l'article à se faire livrer
* **Quantité à livrer\*** : quantité de la référence à se faire livrer
* **Emplacement cible picking**, _selon paramétrage_ : si le paramétrage "Faire apparaitre l'emplacement cible de picking à l'ajout d'une référence et dans son traitement" est activé, que la référence est en gestion quantité par article, et que votre rôle est en ajout quantité par référence, ce champ apparaîtra. Vous pouvez renseigner ici l'emplacement sur lequel l'article de référence doit être prélevé
* **Quantité disponible** : champ non modifiable. Quantité disponible à la livraison de la référence

Remplissez les différents champs et cliquez sur <mark style="background-color:blue;">**Ajouter**</mark>.&#x20;

Répéter l'opération autant de fois que de référence que vous souhaitez vous faire livrer.&#x20;

Une fois que vous avez fini de faire votre demande de livraison, cliquez sur <mark style="background-color:blue;">**Valider**</mark> pour que votre livraison soit prise en compte et traitée.

Un ordre de préparation sera alors créé.

{% embed url="https://www.screencast.com/t/kRWcfesd3" %}
Ajout d'article sur une demande de livraison
{% endembed %}

### Via le panier

Le fonctionnement du panier est détaillé précisément dans [Panier](../panier.md).

Pour créer une demande de livraison via le panier, allez dans la page _Stock > Références_, et cliquez sur l'icône Panier de chaque référence qui vous souhaitez vous faire livrer.

Cliquez ensuite sur l'icône Panier dans l'entête pour aller dans le panier.&#x20;

Sélectionnez le type de demande Livraison, et sélectionnez _Créer une nouvelle demande_ pour faire une nouvelle demande. La section _Ma nouvelle demande de livraison_ apparaît alors. Remplissez les champs _Type_, _Destination_, les _champs libres_, et le _commentaire_ si besoin. Ils ont la même logique que décrit au dessus.

Sur la zone à droite, renseignez les quantités à se faire livrer dans chaque référence.&#x20;

Renseignez aussi l'emplacement cible picking si vous avez activé le paramétrage.

Il n'y aura pas de sélection d'article dans le panier même si vous êtes en ajout quantité par article.&#x20;

Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> pour créer la demande en brouillon et être redirigé vers le détail de la demande expliqué au dessus.&#x20;

<mark style="background-color:blue;">**Validez**</mark> la demande pour qu'elle soit prise en compte et traitée ensuite.

{% embed url="https://www.screencast.com/t/apGP4Zyjcxm" %}
Demande de livraison via le panier
{% endembed %}

### Via import et mise à jour

Vous pouvez créer des livraisons via import grâce à l'outil d'import [(Voir Paramétrage > Données > Import & mises à jour)](../../../parametrages/donnees/imports-and-mises-a-jour.md)

### Modifier une demande de livraison

Il est possible de modifier une demande de livraison tant que celle-ci est en brouillon.

Pour cela, cliquez sur la flèche à droite de **Valider**, et sur <mark style="background-color:blue;">**Modifier**</mark>. Vous aurez ensuite la possibilité de modifier la destination de la livraison, ses champs libres et son commentaire.

<mark style="background-color:blue;">**Enregistrer**</mark> pour valider les modifications

### Supprimer une demande de livraison

La suppression d'une demande de livraison est directement possible si celle-ci est en brouillon.

Pour cela, cliquez sur la flèche à droite de **Valider**, et sur <mark style="background-color:blue;">**Supprimer**</mark>.&#x20;

La demande sera alors supprimée.

Si la demande est en statut à traiter, il vous faudra supprimer l'ordre de préparation pour que la demande liée soit passée en état brouillon et qu'elle soit supprimable à son tour.

Si la demande est en statut préparé, il vous faudra supprimer l'ordre de livraison, pour débloquer la suppression de la préparation, pour passer la demande de livraison en bouillon et qu'elle soit supprimable à son tour.&#x20;

{% hint style="info" %}
Si la demande est livrée, il n'est plus possible de la supprimer.
{% endhint %}

### Visualiser une demande de livraison

Pour accéder au détail de la demande de livraison, cliquez sur la ligne de la demande que vous souhaitez voir. Vous arriverez alors sur le détail de la demande.&#x20;

Dans l'entête de la demande, vous avez une flèche qui donne accès aux boutons <mark style="background-color:blue;">**Aller vers l'ordre de préparation**</mark> et <mark style="background-color:blue;">**Aller vers l'ordre de livraison**</mark>, à partir du statut préparé pour ce dernier bouton. Si la demande a été partiellement livrée à un moment, les boutons s'appelleront **Aller vers les ordres de préparations** et **Aller vers les ordres de livraisons** car plusieurs ordres de préparations et donc de livraison auront été générés.&#x20;

En cliquant sur ces boutons, vous serez redirigé vers le détail de l'ordre de préparation ou l'ordre de livraison généré par la demande ou la préparation dans le cas où il n'y a pas eu de traitement partiel. Dans le cas d'un traitement partiel, le bouton redirigera vers la liste des ordres de préparations ou la liste des ordres de livraison liés à la demande.&#x20;

Vous pouvez également avoir un bouton <mark style="background-color:blue;">**Aller vers la réception**</mark> si la demande de livraison a été générée suite à une réception. Si vous cliquez sur ce bouton, vous serez redirigé vers la réception qui contient les articles qui ont été mis dans la demande.&#x20;

{% embed url="https://www.screencast.com/t/3rCS5RNajD" %}
Depuis une demande de livraison aller vers sa préparation et/ou son ordre
{% endembed %}

## Workflow d'une demande de livraison

Une demande de livraison passe par les statuts suivants :&#x20;

* **brouillon** : la demande vient d'être créer mais est toujours en cours de constitution. Elle n'a pas été encore validée
* **à traiter** : la demande a été validée et doit être traitée. L'ordre de préparation a été générée, il est en statut à traiter (Documentation Ordre de préparation : [Stock > Ordres > Préparations](../ordres/preparations.md))
* **préparé** : l'ordre de préparation a été traité et est lui-même en statut préparé, ce qui passe la demande en préparé, et crée un ordre de livraison en à traiter (Fonctionnement Ordre de livraison : [Stock > Ordres > Livraisons](../ordres/livraisons.md))
* **partiellement préparé** : tous les articles n'ont pas été prélevé sur la préparation ce qui a généré une nouvelle préparation à traiter. La demande passe alors en partiellement préparé
* **livré** : tous les articles demandés sont livrés. L'ordre de livraison est passé en livré ce qui passe la demande en livré
* **livré partiellement** : lorsqu'il y a eu préparation partielle et que seulement une partie de préparation a été livrée, la demande passe en partiellement livrée
