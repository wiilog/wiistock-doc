# Réceptions

La réception permet de rentrer des références et des articles en stock. Vous pouvez créer des attendues de réception avant de recevoir vos références. Vous pouvez également importer vos attendues de réception grâce à l'outil d'import de l'application (Paramétrage > Données > Imports & mises à jour).

Cette fonctionnalité est uniquement disponible en web.

Pour accéder à la page, vous devez aller dans le menu <mark style="background-color:blue;">**Ordre**</mark>, puis <mark style="background-color:blue;">**Réceptions**</mark>.

La page des réceptions contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Nouvel réception**, destiné à la création de réception
* Un bouton **Exporter au format CSV**, sous le bouton **Nouvelle réception**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un bouton **Gestion des colonnes**, sous la bouton **Nouvelle réception**, permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différentes réceptions créées

{% embed url="https://www.screencast.com/t/7UbBhxsJ" %}
Page des réceptions
{% endembed %}

### Contenu des filtres

Les filtres affichés sont paramétrables dans [<mark style="color:blue;">Paramétrage > Stock > Réceptions > Champs fixes</mark>](../../../parametrages/receptions.md)  Le tableau ci-dessous récapitule tous les filtres disponibles.

Une fois que vous avez renseigné vos filtres, cliquez sur <mark style="background-color:blue;">**Filtrer**</mark>. Les filtres sont conservés d'une session à l'autre (ils seront toujours actifs si vous changez de page ou que vous vous déconnectez et reconnectez).

| Filtre                       | Description                                                                                                                                                                               |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                       | La tranche basse filtrant sur la date de création de la réception                                                                                                                         |
| **Au**                       | La tranche haute filtrant sur la date de création de la réception                                                                                                                         |
| **Statuts**                  | Statut de la réception. Vous pouvez mettre plusieurs statuts pour filtrer sur les réception ayant ces statuts                                                                             |
| **Demandeurs**               | Pour filtrer sur les personnes ayant créées une réception. Le filtre va chercher dans la liste des utilisateurs de l'application. Vous pouvez filtrer sur plusieurs demandeurs à la fois  |
| **Fournisseurs**             | Pour filtrer sur le fournisseur indiqué sur la réception. Le filtre va chercher dans la liste des fournisseurs de l'application. Vous pouvez filtrer sur plusieurs fournisseurs à la fois |
| **Urgence ?**                | Si le switch est activé, seules les réceptions avec des références en urgence apparaitront                                                                                                |
| **Date attendue jj/mm/aaaa** | Filtre sur la date attendue de la réception                                                                                                                                               |
| **N° de commande**           | Filtre sur le numéro de commande de la réception. Vous pouvez filtrer sur plusieurs numéros de commande à la fois                                                                         |

### Contenu du tableau

Les colonnes du tableau affichés à l'écran sont paramétrables en cliquant sur la flèche à droite de <mark style="background-color:blue;">**Nouvelle réception**</mark> et en choisissant <mark style="background-color:blue;">**Gestion des colonnes**</mark>. Cochez alors les champs que vous souhaitez afficher et <mark style="background-color:blue;">**Enregistrez**</mark>. Ce choix sera conservé d'une session à l'autre.&#x20;

En fonction du nombre de champs sélectionnés, une barre horizontale de défilement peut apparaître.&#x20;

| Colonne                                        | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Date création**                              | Date de création de la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **N° de réception**                            | Numéro de réception généré par Follow GT. Il est constitué d'un préfixe R, de l'année, du mois, et du jour de création, et d'un compteur                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Date attendue**                              | Date attendue de la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Date fin**                                   | Date de fin de la réception. Pour qu'une réception ait une date de fin, il faut avoir cliquer sur **Fin réception** sur le détail                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Numéro commande**                            | Numéro de commande mis sur la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Destinataire(s)**                            | Si une demande de livraison est générée suite à une réception, le demandeur de la demande de livraison sera mis en destinataire sur la réception. Une réception peut générer plusieurs demandes de livraison et ainsi avoir plusieurs demandeurs                                                                                                                                                                                                                                                                                           |
| **Fournisseur**                                | Fournisseur de la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Statut**                                     | <p>Statut de la réception . 4 statuts sont possibles : <br>- <em><strong>En attente de réception</strong></em> : la réception a été créée <br>- <em><strong>Anomalie</strong></em> : le switch Anomalie a été coché sur la réception pour indiquer un soucis sur la réception<br>- <em><strong>Réception totale</strong></em> : la réception est terminée, et le bouton <strong>Fin réception</strong> a été cliqué<br>- <em><strong>Réception partielle</strong></em> : la réception a été annulée. Elle passe en réception partielle</p> |
| **Emplacement de stockage**                    | Emplacement de stockage des références / articles réceptionnés. Cet emplacement sera utilisé pour les demandes de transfert générées via la réception pour renseigner l'emplacement de destination                                                                                                                                                                                                                                                                                                                                         |
| **Commentaire**                                | Commentaire sur la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Type(s) de demande(s) de livraison liée(s)** | Types des livraisons qui ont été créées sur la réception                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

### Créer une nouvelle réception

Afin de créer une nouvelle réception, il suffit de cliquer sur le bouton <mark style="background-color:blue;">**Nouvelle réception**</mark>. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs.&#x20;

Les champs affichés sur le formulaire sont paramétrables dans [<mark style="color:blue;">Paramétrage > Stock > Réceptions > Champs fixes</mark>](../../../parametrages/receptions.md), où vous pouvez choisir de les afficher ou non, ou de les rendre obligatoires ou non.&#x20;

Vous pouvez renseigner les champs suivants :&#x20;

* **Date commande** : date à laquelle la commande de ce qui va être réceptionné a été faite
* **Date attendue** : date à laquelle la commande est attendue
* **Numéro de commande** : numéro de commande de la réception
* **Emplacement** : emplacement de réception. Les références / articles seront déposés par défaut sur cet emplacement. Il est possible de paramétrer cet emplacement pour qu'il soit toujours le même et ne pas avoir à le saisir systématiquement dans [Paramétrage | Stock | Réceptions | Réceptions - Statuts](../../../parametrages/receptions.md)
* **Fournisseur** : fournisseur de la réception. Le champ va chercher dans le référentiel des fournisseurs. Tapez les premiers caractères du fournisseur souhaité pour avoir des propositions de fournisseurs ayant ces lettres dans leur nom. Si le fournisseur n'est pas présent dans la liste, vous pouvez en ajouter un nouveau en cliquant sur le <mark style="background-color:blue;">**+**</mark> à côté du champ, pour renseigner le nom et le code du fournisseur et l'ajouter dans la liste
* **Transporteur** : transporteur de la réception. Le champ va chercher dans le référentiel des transporteurs. Tapez les premiers caractères du transporteur souhaité pour avoir des propositions de transporteurs ayant ces lettres dans leur nom. Si le transporteur n'est pas présent dans la liste, vous pouvez en ajouter un nouveau en cliquant sur le <mark style="background-color:blue;">**+**</mark> à côté du champ, pour renseigner le nom et le code du transporteur et l'ajouter dans la liste
* **Emplacement de stockage** : emplacement où doivent être stockés les références / articles réceptionnés. Le champ va chercher dans le référentiel emplacement. Cet emplacement sera utilisé si vous créez une demande de transfert sur la modale de conditionnement de la réception. Il sera utilisé pour renseigner l'emplacement de destination de la demande de transfert
* **Anomalie** : ce switch permet d'indiquer que la réception a une anomalie. Le statut de la réception sera alors en _**Anomalie**_
* **Urgence ?** : ce switch permet d'indiquer que la réception créée est à traiter en urgence. Le détail de la réception aura alors la mention "cette réception est urgente" et la ligne de la réception sera rouge dans le tableau des réceptions.
* **Commentaire** : commentaire sur la réception
* **Pièces jointes** : vous pouvez ajouter des pièces jointes sur la réception tels que les documents de livraison fournit par le chauffeur par exemple
* **Champs libres** : la réception peut avoir des champs libres. Ils sont à configurer dans [<mark style="color:blue;">Paramétrage > Stock > Réceptions > Champs libres</mark>](../../../parametrages/receptions.md)<mark style="color:blue;">.</mark> Une réception n'a pas de type, les champs libres seront donc toujours les mêmes d'une réception à l'autre

Une fois les champs renseignés, cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>.&#x20;

{% embed url="https://www.screencast.com/t/8uKiNPXk1" %}
Modale nouvelle réception
{% endembed %}
