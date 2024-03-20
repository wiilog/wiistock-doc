# Litiges / Qualité

Pour créer un litige, il faut le faire dans le détail d'une réception.

{% hint style="info" %}
Pour le suivre, vous avez la possibilité de le faire dans **le détail de la réception** ou alors dans la page **Qualité > Litiges**
{% endhint %}

## Créer un litige

Pour créer un litige, allez dans la zone **Liste des litiges** du détail de la réception et cliquez sur le bouton <mark style="background-color:blue;">**Nouveau litige**</mark>.&#x20;

Les champs suivants sont présents sur la modale de création de litige :&#x20;

* **Type\*** : type du litige
* **Statut\*** : statut du litige
* **Acheteur(s)** : acheteur ayant passé la commande. Ainsi, il pourra recevoir un mail à l'ouverture du litige si vous avez paramétré cela
* **Déclarant\*** : personne ayant créée le litige, par défaut l'utilisateur de la session en cours
* **Articles\*** : articles concernés par le litige
* **Commentaire** : commentaire sur le litige
* **Urgences ?** : indication que le litige est à traiter en urgence. La ligne du litige sera rouge sur le détail de l'arrivage et sur la page Qualité | Litiges. Si l'article que vous ajoutez dans le litige provient d'une ligne de réception en urgence, le litige sera automatiquement mis en urgence
* **Pièces jointes** : pour mettre des pièces jointes sur le litige

**Lorsque vous créez un litige sur une réception, celui-ci se retrouve automatiquement dans la page Qualité > Litiges**

{% embed url="https://www.screencast.com/t/87pjBFsHQDUS" %}
Créer un litige
{% endembed %}

## Suivre/Modifier un litige

### Dans le détail d'une réception

La zone **Liste des litiges** dans le détail d'une réception est constitué d'un tableau contenant les éléments suivants

| Colonne                | Description                           |
| ---------------------- | ------------------------------------- |
| **Type**               | Type du litige                        |
| **Statut**             | Statut actuel du litige               |
| **Dernier historique** | Dernier commentaire mis sur le litige |

Pour modifier le litige, cliquez sur la ligne du litige. La modale de modification du litige s'ouvrira alors. Elle contient les informations suivantes :&#x20;

* Le **type** : le type du litige. Vous pouvez requalifier le type du litige si besoin.
* Le switch **Urgence ?** : pour qualifier le litige en urgence. La ligne litige sera alors en rouge.
* Le **statut** : modifier le statut du litige pour le faire évoluer. Sélectionnez un statut en état Traité pour le clôturer. En fonction du paramétrage des statuts, un mail peut être envoyer à l'acheteur et/ou au déclarant du litige pour l'informer du changement de statut du litige
* Le/les **colis** : colis concerné(s) par le litige. Vous pouvez enlever un colis ou en ajouter
* L'**acheteur** : acheteur sur le litige. Vous pouvez le modifier
* Le **déclarant** : déclarant du litige. Vous pouvez le modifier
* Les **articles** : articles concernés par le litige. Vous pouvez en ajouter ou en enlever
* Le **commentaire** : inscrivez un commentaire et cliquez sur <mark style="background-color:blue;">**Ajouter**</mark> pour mettre le commentaire dans le tableau Historique, et créer ainsi potentiellement une conversation pour résoudre le litige
* Les **pièces jointes** : vous pouvez ajouter des pièces-jointes tels qu'une photo d'un article abîmé par exemple&#x20;
* Le tableau **Historique** : ce tableau retrace tout l'historique du litige, avec une ligne par modification, et les colonnes suivantes :&#x20;
  * **Utilisateur** : personne ayant réalisée la modification
  * **Date** : date et heure auxquels la modification a eu lieu
  * **Commentaire** : si un commentaire a été ajouté dans le champ Commentaire, il apparaîtra dans cette colonne
  * **Statut** : statut du litige au moment de la modification
  * **Type** : type du litige au moment de la modification
* Le tableau **Articles** : ce tableur récapitule la liste des articles concernés par le litige. Il contient les colonnes suivantes :&#x20;
  * **Code article** : code barre de l'article en litige
  * **Statut** : statut de l'article en litige
  * **Libellé** : libellé de l'article en litige
  * **Référence article** : code de la référence de l'article en litige
  * **Quantité** : quantité de l'article

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider vos modification.

{% embed url="https://www.screencast.com/t/nY2wkT2JP9" %}
Modification d'un litige
{% endembed %}

### Dans la page Qualité > Litiges

La page Qualité > Litiges sert à centraliser tous les litiges dans une seule et même page afin de les retrouver facilement. Cette page concerne surtout les personnes en charge de traiter les litiges, telles que des profils acteurs.&#x20;

La pages est constituée de :

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV** destiné à exporter l'ensemble des données (suivant les dates renseignées) au format CSV
* Un bouton **Gestion des colonnes**, sous la bouton "Exporter au format CSV", permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différents litiges créés

{% embed url="https://www.screencast.com/t/2NfEEGp2yj" %}
Page de centralisation des litiges
{% endembed %}

**Filtres**

Le tableau ci-dessous récapitule tous les filtres disponibles.

Une fois que vous avez renseigné vos filtres, cliquez sur <mark style="background-color:blue;">**Filtrer**</mark>. Les filtres sont conservés d'une session à l'autre (ils seront toujours actifs si vous changez de page ou que vous vous déconnectez et reconnectez).

| Filtre               | Description                                                                                                                                                                                                                                                                                  |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**               | La tranche basse filtrant sur la date de création du litige                                                                                                                                                                                                                                  |
| **Au**               | La tranche haute filtrant sur la date de création du litige                                                                                                                                                                                                                                  |
| **Statuts**          | Statut du litige. Vous pouvez mettre plusieurs statuts pour filtrer sur les litiges ayant ces statuts en cours                                                                                                                                                                               |
| **Origines**         | Origine du litige. Il est possible de créer un litige dans l'application soit dans un arrivage soit dans une réception                                                                                                                                                                       |
| **Utilisateurs**     | Pour filtrer sur l'acheteur du litige. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre              |
| **Numéro de litige** | Tapez précisément le numéro du litige que vous cherchez pour afficher celui-ci                                                                                                                                                                                                               |
| **Déclarant**        | Pour filtrer sur la personne ayant créée le litige. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Type**             | Type du litige                                                                                                                                                                                                                                                                               |
| **Urgence ?**        | Pour afficher seulement les litiges identifiés comme urgents                                                                                                                                                                                                                                 |

**Contenu du tableau**

Les colonnes du tableau affichés à l'écran sont paramétrables en cliquant sur la flèche à droite de "Exporter au format CSV" et en choisissant <mark style="background-color:blue;">**Gestion des colonnes**</mark>. Cochez alors les champs que vous souhaitez afficher et enregistrez. Ce choix sera conservé d'une session à l'autre. Vous pouvez également **modifier l'ordre des colonnes** en faisant un glisser déposer.&#x20;

En fonction du nombre de champs sélectionnés, une barre horizontale de défilement peut apparaître.&#x20;

| Colonne                | Description                                                                                                                                                                                             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro du litige**   | Numéro du litige généré par l'application. Il est constitué d'un préfixe (LA pour les litiges générés par arrivage, LR pour ceux générés par réception), de l'année, du mois, du jour, et d'un compteur |
| **Type**               | Type du litige                                                                                                                                                                                          |
| **Fournisseur**        | _Voir les litiges sur arrivage_                                                                                                                                                                         |
| **n° de réception**    | Numéro de la réception sur laquelle a été créée le litige                                                                                                                                               |
| **n° d'arrivage**      | _Voir les litiges sur arrivage_                                                                                                                                                                         |
| **Déclarant**          | Personne ayant créé le litige                                                                                                                                                                           |
| **Acheteur**           | Acheteur(s) renseigné(s) sur le litige                                                                                                                                                                  |
| **N° commande/BL**     | _Voir les litiges sur arrivage_                                                                                                                                                                         |
| **N° ligne**           | Numéro de commande de la ligne de réception                                                                                                                                                             |
| **Référence**          | Référence de l'article concerné par le litige                                                                                                                                                           |
| **Créé le**            | Date de création du litige                                                                                                                                                                              |
| **Modifié le**         | Date de dernière modification du litige                                                                                                                                                                 |
| **Statut**             | Statut actuel du litige                                                                                                                                                                                 |
| **Dernier historique** | Dernier commentaire mis sur le litige avec sa date et son heure                                                                                                                                         |

Pour **modifier un litige**, cliquez sur la ligne du litige à modifier. La même modale de modification de litige décrite précédemment s'ouvrira alors.

## Supprimer un litige

### Dans le détail d'une réception

Vous pouvez supprimer un litige en cliquant sur<img src="../../../../.gitbook/assets/3points" alt="" data-size="line">et en cliquant sur le bouton <mark style="background-color:blue;">**Supprimer**</mark>.

### Dans la page Qualité > Litiges

Vous pouvez supprimer un litige en cliquant sur les<img src="../../../../.gitbook/assets/3points" alt="" data-size="line">de la ligne du litige à supprimer et en cliquant sur le bouton <mark style="background-color:blue;">**Supprimer**</mark>. Il sera aussi supprimé de la réception.
