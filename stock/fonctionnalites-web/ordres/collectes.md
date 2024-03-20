# Collectes

L'ordre de collecte est généré suite à la validation de la collecte. L'ordre est ce qui sera traité, et son traitement passera la demande en traité

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Ordre**</mark>, puis <mark style="background-color:blue;">**Collectes**</mark>. Vous pouvez arriver aussi directement sur le détail d'un ordre de collecte à partir du détail d'une demande de collecte en cliquant sur la flèche à droite de l'entête puis sur <mark style="background-color:blue;">**Aller vers l'ordre de collecte**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différents ordres de collectes créées

## Contenu des filtres

| Filtre                 | Description                                                                                                                                                                                                                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création de l'ordre de collecte                                                                                                                                                                                                                                 |
| **Au**                 | La tranche haute filtrant sur la date de création de l'ordre de collecte                                                                                                                                                                                                                                 |
| **Statuts**            | Le(s) statut(s) des ordres de collecte à filtrer                                                                                                                                                                                                                                                         |
| **Numéros de demande** | Pour filtrer sur les numéros de demande de collecte ayant générés les ordres                                                                                                                                                                                                                             |
| **Utilisateurs**       | Pour filtrer sur la personne ayant traitée l'ordre de collecte. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Type**               | Le type des ordres de collecte à filtrer                                                                                                                                                                                                                                                                 |

## Contenu du tableau

| Colonne              | Description                                                    |
| -------------------- | -------------------------------------------------------------- |
| **Numéro**           | Numéro de l'ordre de collecte                                  |
| **Statut**           | Statut de l'ordre de collecte                                  |
| **Date de création** | Date de création de l'ordre de collecte                        |
| **Opérateur**        | Opérateur ayant traité l'ordre de collecte                     |
| **Type**             | Type de la demande de collecte ayant créée l'ordre de collecte |

{% embed url="https://www.screencast.com/t/2kjJHNvhLT" %}
Page Ordre collecte
{% endembed %}

## Détails de l'ordre de collecte

L'ordre de collecte est constituée d'une entête et d'un tableau contenant la liste des références à collecter.

L'entête est constituée des champs :&#x20;

* **Numéro** : numéro de l'ordre de collecte
* **Statut** : statut actuel de l'ordre de collecte
* **Opérateur** : opérateur ayant traité l'ordre de collecte. Le champ est donc rempli seulement si l'ordre de collecte est traité
* **Demandeur** : personne ayant créée la demande ayant générée l'ordre de collecte
* **Destination** : instruction si la référence doit être détruite ou remise en stock
* **Point de collecte** : emplacement où les références doivent être collectées
* **Date de création** : date de création de l'ordre de collecte
* **Date de collecte** : date à laquelle l'ordre de collecte a été traité

Dans cette entête se trouve également les boutons :&#x20;

* **Finir la collecte** : pour finir la collecte. Ce bouton clôture la collecte à certaines conditions, voir plus bas.&#x20;
* Sous la flèche :&#x20;
  * **Aller vers la demande de collecte** : pour retourner sur le détail de la demande de collecte ayant générée l'ordre
  * **Imprimer les étiquettes** : impression des étiquettes de code barre des articles à remettre en stock ou des références à détruire
  * **Supprimer** : suppression de l'ordre de collecte. La demande passera alors en état Brouillon
  * **Associer à un capteur** : disponible seulement pour les collectes de mise en stock. Pour associer les articles de l'ordre de collecte à un capteur de température ou GPS et suivre la collecte

Tableau de la liste des articles :&#x20;

| Colonne         | Description                          |
| --------------- | ------------------------------------ |
| **Référence**   | Référence à collecter                |
| **Libellé**     | Libellé de la référence à collecter  |
| **Emplacement** | Emplacement de la référence en stock |
| **Quantité**    | Quantité à collecter                 |

## Traiter l'ordre de collecte

Il est possible de traiter l'ordre de collecte sur la supervision, ce que nous allons voir ici. Pour voir le traitement sur le terminal mobile, voir [Stock > Fonctionnalités mobiles > Collectes.](../../fonctionnalites-mobile/stock-i-collecte.md)

### Modifier l'ordre de collecte&#x20;

Avant de traiter l'ordre de collecte, vous pouvez venir modifier la quantité de chaque ligne de référence à collecter. Pour cela, cliquez sur les<img src="../../../.gitbook/assets/3-points.png" alt="" data-size="line">à gauche de la ligne de la référence dont vous souhaitez modifier la quantité et cliquez sur <mark style="background-color:blue;">**Modifier**</mark>. Plusieurs cas peuvent se présenter :&#x20;

* **Référence en gestion quantité par article + ajout de la référence sur la demande par un utilisateur en ajout quantité par article + collecte de **_**Mise en stock**_ : dans ce cas, l'utilisateur a directement choisi l'article qui était sorti du stock à remettre en stock ou alors a généré un nouvel article à mettre en stock. Il n'est pas possible alors de modifier la quantité à collecter
* **Référence en gestion quantité par article ou référence + ajout de la référence sur la demande par un utilisateur en ajout quantité par référence + collecte de **_**Mise en stock**_** ou **_**Destruction**_** :** une modale _Modifier la quantité_ vous permet de choisir une quantité différente à collecter. Il est seulement possible de changer cette quantité pour une quantité inférieure.

### Valider la quantité de la référence à collecter

* **Pour les références en gestion quantité par article ou référence avec ajout de la référence sur la demande par un utilisateur en ajout quantité par article + collecte de Mise en stock ou Destruction :** cliquez sur la ligne pour la passer en vert, signifiant ainsi que cette ligne a été collectée
* **Pour les références en gestion quantité par article avec ajout de la référence sur la demande par un utilisateur en ajout quantité par référence + collecte de Mise en stock**  : sélectionnez le code de l'article qui était sorti du stock à remettre en stock, ou si l'article que vous collectez n'est pas étiqueté, ne sélectionnez rien pour créer un nouvel article. Indiquez la quantité à collecter et Ajouter. Cliquez à nouveau sur la ligne de l'article pour la passer en vert et signifier ainsi que la ligne a bien été collectée.&#x20;

Une fois que toutes les lignes de votre ordre de collecte sont vertes, cliquez sur <mark style="background-color:blue;">**Finir la collecte.**</mark>

### Valider la collecte&#x20;

**Pour une destruction**

Cliquez sur <mark style="background-color:blue;">**Finir la collecte**</mark>. L'ordre de collecte passe en Traité et la demande liée en Collecté.

Aucun mouvement de stock n'est généré suite à une collecte de destruction

**Pour une mise en stock**

Cliquez sur Finir la collecte, une modale va alors s'ouvrir pour indiquer où sont déposés en stock les articles / références collectés. Pour chaque code barre, indiquez l'endroit où vous le déposez et cliquez sur Finir la collecte.

{% embed url="https://www.screencast.com/t/H2Kc2uSxF" %}

L'ordre de collecte passe en Traité et la demande liée en Collecté.

Des mouvements de stock de type entrée sont alors créés sur les emplacements indiqués pour les codes barres de la collecte avec comme origine du mouvement l'emplacement de collecte. Des mouvements de prise sur l'emplacement de collecte et de dépose sur les emplacements indiqués sont créés.



