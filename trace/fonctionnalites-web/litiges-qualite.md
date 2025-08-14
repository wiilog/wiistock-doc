# Litiges / Qualité

Si les marchandises livrées sur votre arrivage ont des éléments non conforme, vous pouvez créer un litige et le suivre dans Wiilog.&#x20;

**Pour créer un litige, il faut le faire dans le détail d'un arrivage UL.**&#x20;

Pour le suivre, vous avez la possibilité de le faire dans le détail de l'arrivage UL ou alors dans la page Qualité > Litiges

## Créer un litige

Pour créer un litige, allez dans la zone **Liste des litiges** du détail de l'arrivage UL et cliquez sur le bouton <mark style="background-color:blue;">**Nouveau litige**</mark>.&#x20;

Les champs suivants sont présents sur la modale de création de litige :&#x20;

* Le **fournisseur** : fournisseur de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Le **transporteur** : transporteur de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Le **chauffeur** : chauffeur de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Le **numéro de l'arrivage** : numéro de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Le **numéro de commande / BL** : les numéros de commande de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Les **acheteurs** : les acheteurs de l'arrivage. Le champ ne peut pas être modifié. Allez modifier l'arrivage pour modifier le champ sur cette fenêtre
* Le **type** : le type du litige. Pour indiquer le type du litige. Les types sont paramétrables ([<mark style="color:blue;">Paramétrages > Trace > Arrivages UL > Litiges - Types</mark>](../parametrage/arrivages-ul/litiges-types.md))
* Le **déclarant** : par défaut, la personne ayant créée le litige. Une autre personne peut être renseignée
* Le **statut** : statut du litige, pour voir où en est le litige. Le workflow des litiges n'est pas dépendant des types et est paramétrable ([<mark style="color:blue;">Paramétrages > Arrivages > Litiges - Statuts</mark>](../parametrage/arrivages-ul/litiges-statuts.md)). Le statut d'un litige peut déclencher, en fonction du paramétrage, un envoi de mail à l'acheteur pour l'informer de l'ouverture du litige.
* Le/les **unité(s) logistique(s)** : le ou les unité(s) logistique(s) qui sont concernés par les litiges
* **Commentaire** : vous pouvez ajouter un complétement d'information sur le litige
* Switch **Urgence ?** : si vous l'activez, la ligne du litige apparaîtra en rouge
* **Pièce jointe** : vous pouvez ajouter des pièces jointes sur le litige

Lorsque vous créez un litige sur un arrivage, celui-ci se retrouve automatiquement dans la page Qualité > Litiges

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 11.14.09 (1).png" alt=""><figcaption></figcaption></figure>

## Suivre/Modifier un litige

### Dans le détail d'un arrivage

La zone **Liste des litiges** est constitué d'un tableau contenant les éléments suivants

| Colonne                  | Description                                              |
| ------------------------ | -------------------------------------------------------- |
| **Date de création**     | Date et heure auxquels a été créée le litige             |
| **Statut**               | Statut actuel du litige                                  |
| **Type**                 | Type du litige                                           |
| **Date de modification** | Dernières date et heure auxquels a été modifié le litige |

Pour modifier le litige, cliquez sur la ligne du litige. La modale de modification du litige s'ouvrira alors. Elle contient les informations suivantes :&#x20;

* Le **type** : le type du litige. Vous pouvez requalifier le type du litige si besoin.
* Le switch **Urgence ?** : pour qualifier le litige en urgence. La ligne litige sera alors en rouge.
* Le **statut** : modifier le statut du litige pour le faire évoluer. Sélectionnez un statut en état Traité pour le clôturer. En fonction du paramétrage des statuts, un mail peut être envoyer à l'acheteur et/ou au déclarant du litige pour l'informer du changement de statut du litige
* Le/les **colis** : colis concerné(s) par le litige. Vous pouvez enlever un colis ou en ajouter
* Le **commentaire** : inscrivez un commentaire et cliquez sur Ajouter pour mettre le commentaire dans le tableau Historique, et créer ainsi potentiellement une conversation pour résoudre le litige
* Les **pièces jointes** : vous pouvez ajouter des pièces jointes tels qu'une photo d'un colis abîmé par exemple&#x20;
* Le tableau **Historique** : ce tableau retrace tout l'historique du litige, avec une ligne par modification, et les colonnes suivantes :&#x20;
  * **Utilisateur** : personne ayant réalisée la modification
  * **Date** : date et heure auxquels la modification a eu lieu
  * **Commentaire** : si un commentaire a été ajouté dans le champ Commentaire, il apparaîtra dans cette colonne
  * **Statut** : statut du litige au moment de la modification
  * **Type** : type du litige au moment de la modification

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider vos modification.

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 11.46.33.png" alt=""><figcaption></figcaption></figure>

### Dans la page Qualité > Litiges

La page Qualité > Litiges sert à centraliser tous les litiges dans une seule et même page afin de les retrouver facilement. Cette page concerne surtout les personnes en charge de traiter les litiges, telles que des profils acteurs.&#x20;

La pages est constituée de :

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark> destiné à exporter l'ensemble des données (suivant les dates renseignées) au format CSV
* Un bouton <mark style="background-color:blue;">**Gestion des colonnes**</mark>, sous la bouton **Exporter au format CSV**, permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différents litiges créés

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
| Acheteur             | Afficher les Litiges associés à l'acheteur                                                                                                                                                                                                                                                   |

**Contenu du tableau**

Les colonnes du tableau affichés à l'écran sont paramétrables en cliquant sur la flèche à droite de **Exporter au format CSV** et en choisissant <mark style="background-color:blue;">**Gestion des colonnes**</mark>. Cochez alors les champs que vous souhaitez afficher et enregistrez. Ce choix sera conservé d'une session à l'autre. Vous pouvez également **modifier l'ordre des colonnes** en faisant un glisser déposer.&#x20;

En fonction du nombre de champs sélectionnés, une barre horizontale de défilement peut apparaître.&#x20;

| Colonne                | Description                                                                                                                                                                                             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro du litige**   | Numéro du litige généré par l'application. Il est constitué d'un préfixe (LA pour les litiges générés par arrivage, LR pour ceux générés par réception), de l'année, du mois, du jour, et d'un compteur |
| **Type**               | Type du litige                                                                                                                                                                                          |
| **Fournisseur**        | Fournisseur de l'arrivage concerné par le litige                                                                                                                                                        |
| **n° de réception**    | _Voir les litiges sur réception_                                                                                                                                                                        |
| **n° d'arrivage UL**   | Numéro de l'arrivage sur lequel a été créé le litige                                                                                                                                                    |
| **Déclarant**          | Personne ayant créé le litige                                                                                                                                                                           |
| **Acheteur**           | Acheteur(s) associé(s) à l'arrivage sur lequel a été créé le litige                                                                                                                                     |
| **N° commande/BL**     | Numéro de commande renseigné sur l'arrivage sur lequel a été créé le litige                                                                                                                             |
| **N° ligne**           | _Voir les litiges sur réception_                                                                                                                                                                        |
| **Référence**          | _Voir les litiges sur réception_                                                                                                                                                                        |
| **Créé le**            | Date de création du litige                                                                                                                                                                              |
| **Modifié le**         | Date de dernière modification du litige                                                                                                                                                                 |
| **Statut**             | Statut actuel du litige                                                                                                                                                                                 |
| **Dernier historique** | Dernier commentaire mis sur le litige avec sa date et son heure                                                                                                                                         |
| **Fournisseur**        | Le fournisseur de l'arrivage UL                                                                                                                                                                         |
| **Référence**          | La référence de l'article si renseignée                                                                                                                                                                 |

Pour **modifier un litige**, cliquez sur la ligne du litige à modifier. La même modale de modification de litige décrite précédemment s'ouvrira alors.

{% embed url="https://www.screencast.com/t/uD8ir8be" %}
Modification d'un litige
{% endembed %}

## Supprimer un litige

### Dans le détail d'un arrivage

Vous pouvez supprimer un litige en cliquant sur<img src="../../.gitbook/assets/3points" alt="" data-size="line">et en cliquant sur le bouton <mark style="background-color:blue;">**Supprimer**</mark>.

### Dans la page Qualité > Litiges

Vous pouvez supprimer un litige en cliquant sur les<img src="../../.gitbook/assets/3points" alt="" data-size="line">de la ligne du litige à supprimer et en cliquant sur le bouton <mark style="background-color:blue;">**Supprimer**</mark>. Il sera aussi supprimé de l'arrivage.
