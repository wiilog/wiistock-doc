---
description: >-
  La demande d'achat sert à venir indiquer à un acheteur identifié la nécessité
  de commander des références.
---

# Achats

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Demande**</mark>, puis <mark style="background-color:blue;">**Achat**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes d'achat créées

### Contenu des filtres

| Filtre         | Description                                                                                                                                                                                                                                                                                           |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**         | La tranche basse filtrant sur la date de création de la demande d'achat                                                                                                                                                                                                                               |
| **Au**         | La tranche haute filtrant sur la date de création de la demande d'achat                                                                                                                                                                                                                               |
| **Statuts**    | Le(s) statut(s) des demandes d'achat à filtrer                                                                                                                                                                                                                                                        |
| **Demandeurs** | Pour filtrer sur la personne ayant créée la demande d'achat. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Acheteurs**  | Pour filtrer sur l'acheteur identifié de la demande d'achat. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |

### Contenu du tableau

| Colonne                     | Description                                                                                                             |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Numéro**                  | Numéro de la demande d'achat                                                                                            |
| **Date de création**        | Date de création de la demande d'achat                                                                                  |
| **Date de validation**      | Date de la validation de la demande d'achat : date de passage du statut en état Brouillon à un statut en état A traiter |
| **Date de prise en compte** | Date de passage d'un statut à un état A traiter à un statut à un état En cours                                          |
| **Date de traitement**      | Date de passage à un statut en état Traité                                                                              |
| **Demandeur**               | Personne ayant créée la demande                                                                                         |
| **Statut**                  | Statut actuel de la demande                                                                                             |
| **Acheteur**                | Acheteur de la demande                                                                                                  |

## Créer une demande d'achat

### Via le bouton "+"

Dans le bouton d'action rapide, sélectionnez **Achat** pour créer une demande d'achat.

![](<../../../.gitbook/assets/2022-05-30 15_23_54-FollowGT _ Demande _ Achat.png>)

Contrairement aux autres demandes, la demande d'achat ne passe pas par une modale permettant de renseigner des champs fixes ou des champs libres. Au clic sur <mark style="background-color:blue;">**+**</mark>, vous êtes redirigés directement vers le détail d'une demande d'achat qui est directement créé au statut Brouillon.

{% hint style="info" %}
Avant de pouvoir créer une demande d'achat, il faut donc avoir paramétré au préalable les différents statuts de votre workflow d'achat
{% endhint %}

Le **détail** est constitué de :&#x20;

* une **entête**. Elle contient les différentes informations de la demande d'achat qui ne concernent pas les références
* le **tableau** de la **liste des références**, qui a les colonnes suivantes :&#x20;

| Colonne                | Description                                                                                                             |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Référence**          | Référence à acheter                                                                                                     |
| **Libellé**            | Libellé de la référence à acheter                                                                                       |
| **Quantité demandée**  | Quantité demandée de la référence à acheter                                                                             |
| **Quantité en stock**  | Quantité en stock actuelle de la référence à acheter                                                                    |
| **Quantité commandée** | Quantité qui a été commandée de la référence à acheter. Cette colonne sera donc remplie à la fin de la demande          |
| **N° commande**        | Numéro de la commande passée pour acheter la référence demandée. Cette colonne sera donc remplie à la fin de la demande |

Pour ajouter une référence à acheter, cliquer sur <mark style="background-color:blue;">**Ajouter référence**</mark>.

Si vous cliquez sur <mark style="background-color:blue;">**Chercher une référence**</mark> sous <mark style="background-color:blue;">**Ajouter référence**</mark>, vous serez redirigé vers la page des références.

Une modale s'ouvrira alors. Tapez le code de la référence pour faire apparaître les autres champs. La modale est constituée de ces champs :&#x20;

* **Référence\*** : référence à acheter
* **Libellé** : libellé de la référence à acheter
* **Emplacement**: Pour les références gérées en quantité à la référence, l'emplacement sera grisé. Pour les références gérées en quantité à l'article, l'emplacement peut être sélectionné si une ou plusieurs règles de stockage ont été paramétrées au préalable sur la référence en question. L'emplacement n'est pas obligatoire pour ajouter la référence à la demande d'achat.
* **Quantité en stock** : quantité en stock de la référence à acheter
* **Acheteur** : acheteur de la référence
* **Quantité demandée\*** : quantité demandée à l'achat de la référence

Remplissez les champs et cliquez sur <mark style="background-color:blue;">**Ajouter**</mark>.&#x20;

La référence doit avoir un acheteur pour être ajoutée. Si ce n'est pas la première référence que vous ajoutez, la référence doit avoir le même acheteur que les références ajoutées précédemment.&#x20;

Si c'est la première référence que vous ajoutez, le champ _Acheteur_ de l'entête sera alors rempli avec l'acheteur de cette première référence.&#x20;

Une fois que vous avez fini d'ajouter toutes vos références à acheter. Cliquez sur <mark style="background-color:blue;">**Valider**</mark>.

Une modale s'ouvrira alors pour choisir le statut suivant de la demande d'achat. Dans cette modale, seuls des statuts en état _A traiter_ sont proposés

### Via le panier

Le fonctionnement du panier est détaillé précisément dans [Panier](../panier.md).

Pour créer une demande d'achat via le panier, allez dans la page _Stock > Références_, et cliquez sur l'icône Panier de chaque référence qui vous souhaitez faire acheter.

Cliquez ensuite sur l'icône Panier dans l'entête pour aller dans le panier.&#x20;

Sélectionnez le type de demande Achat, et dans la zone des références, et sélectionnez _Créer une demande d'achat_ pour faire une nouvelle demande.&#x20;

Sur la zone à droite, renseignez les quantités demandées à l'achat pour chaque référence.&#x20;

Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> ensuite pour créer la demande en brouillon et être redirigé vers le détail de la demande expliqué au dessus, ou vers la liste des demandes d'achat si plusieurs ont été créées car vous avez mis au panier des références ayant des acheteurs différents.

<mark style="background-color:blue;">**Validez**</mark> la demande pour qu'elle soit prise en compte et traitée ensuite.

## Faire évoluer la demande d'achat

**Brouillon vers A traiter**

Lorsque votre demande est sur un statut en état _Brouillon_, et que vous cliquez sur <mark style="background-color:blue;">**Valider**</mark>, une modale "_Valider une demande d'achat_" s'ouvre afin que vous puissiez valider un premier statut comme quoi la demande est à traiter.

Ainsi tous les statuts proposés sont les statuts paramétrés qui sont en état _A traiter_ (voir [Paramétrages >  Stock >Demandes > ](../../parametrage/demandes/achats/statuts.md)[Achat](../../parametrage/demandes/achats/statuts.md)[ > ](../../parametrage/demandes/achats/statuts.md)[Statuts](../../parametrage/demandes/achats/statuts.md)).

La date de validation est alors complétée et le bouton <mark style="background-color:blue;">**Valider**</mark> est transformé en bouton <mark style="background-color:blue;">**Prendre en compte**</mark>.

Vous pouvez modifier la demande sur un autre statut en état _A traiter_ si vous en avez paramétré plusieurs en cliquant sur <mark style="background-color:blue;">**Modifier**</mark> sous la flèche à droite de <mark style="background-color:blue;">**Prendre en compte**</mark>.

Vous pouvez paramétrer sur le statut l'envoi d'un mail à l'acheteur afin qu'il soit informé qu'il a une demande d'achat à traiter.&#x20;

L'envoi d'un mail à l'acheteur ou au demandeur au passage d'un statut est paramétrable pour n'importe quel statut.&#x20;

**A traiter vers En cours**

Cette étape est ensuite une étape pour l'acheteur afin qu'il indique qu'il a bien pris en compte la demande.&#x20;

Pour cela, il faut cliquer sur <mark style="background-color:blue;">**Prendre en compte**</mark> pour faire ouvrir la modale "_Valider la prise en compte_". L'acheteur peut ensuite choisir de passer la demande à un statut en état _En cours_ parmi les statuts paramétrés.

La date de prise en compte est alors complétée et la bouton <mark style="background-color:blue;">**Prendre en compte**</mark> est remplacé par <mark style="background-color:blue;">**Terminer la demande**</mark>.&#x20;

L'acheteur peut modifier la demande sur un autre statut en état _En cours_ si vous en avez paramétré plusieurs en cliquant sur <mark style="background-color:blue;">**Modifier**</mark> sous la flèche à droite de <mark style="background-color:blue;">**Terminer la demande**</mark>.

**En cours vers Traité**

Une fois que la demande est sur un statut en état _En cours_, il est possible de venir cliquer sur chaque ligne des références demandées à l'achat pour venir renseigner les informations de la commande d'achat qui a été passée. En cliquant sur la ligne d'une référence, vous ouvrez une modale qui contient les champs suivants :&#x20;

* **Quantité commandée\*** : quantité commandée de la référence
* **N° commande** : numéro de la commande passée pour cette référence
* **Fournisseur** : fournisseur choisi pour la commande passée pour cette référence
* **Date de commande** : date à laquelle la commande a été passée
* **Date attendue** : date de réception attendue de cette commande

Renseigner ces champs permettra ensuite de venir créer une réception dans Wiilog quand la demande aura été terminée, si un statut avec création de réception est sélectionnée. Les champs obligatoires dépendent du paramétrage des champs fixes de réception.&#x20;

Pour clôturer la demande d'achat, l'acheteur doit cliquez sur <mark style="background-color:blue;">**Terminer la demande**</mark> pour ouvrir la modale "_Terminer la demande_". Il doit choisir alors le statut parmi les statuts paramétrés en état _Traité_.&#x20;

Si le statut sélectionné est un statut qui doit créer une réception derrière, il faut absolument avoir renseigné les informations de la modale décrite précédemment.&#x20;

Si le statut sélectionné ne crée pas de réception derrière, il peut clôturer simplement la demande en cliquant sur <mark style="background-color:blue;">**Enregistrer**</mark>.&#x20;

La date de traitement de la demande est alors renseignée, et si une ou plusieurs réceptions sont créées, vous pouvez voir la réception en question en cliquant sur <mark style="background-color:blue;">**Aller vers les réceptions**</mark> sous la flèche.&#x20;

## Modifier une demande d'achat

Vous pouvez modifier une demande d'achat tant qu'elle n'est pas clôturée.&#x20;

Pour modifier une demande d'achat, allez sur le détail, et cliquez sur la flèche tout à droite pour sélectionner le bouton <mark style="background-color:blue;">**Modifier**</mark>.

Vous pouvez modifier les champs suivants :&#x20;

* **Statut** : vous pouvez changer le statut de la demande mais seulement par un autre statut du même état
* **Commentaire** : vous pouvez ajouter un commentaire
* **Pièce jointe** : vous pouvez ajouter une pièce jointe

## Supprimer une demande d'achat

Vous pouvez supprimer une demande d'achat à n'importe quel moment en fonction de vos droits.&#x20;

Pour la supprimer, allez sur le détail et cliquez sur la flèche à droite pour accéder au bouton <mark style="background-color:blue;">**Supprimer**</mark>.

Cliquez dessus. Une modale de confirmation de suppression apparaîtra alors. Cliquez sur <mark style="background-color:blue;">**Supprimer**</mark> pour confirmer la suppression.&#x20;

