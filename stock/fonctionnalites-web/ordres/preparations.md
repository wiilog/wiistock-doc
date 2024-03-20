# Préparations

L'ordre de préparation est généré suite à la validation de la demande de livraison. Une fois que l'ordre de préparation sera traité, il fera avancé le statut de la demande de livraison et générera un ordre de livraison.

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Ordre**</mark>, puis <mark style="background-color:blue;">**Préparations**</mark>. Vous pouvez arriver aussi directement sur le détail d'un ordre de préparation à partir du détail d'une demande de livraison en cliquant sur la flèche à droite de l'entête puis sur <mark style="background-color:blue;">**Aller vers l'ordre de préparation**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différents ordres de préparation créés

### Contenu des filtres

| Filtre                 | Production                                                                                                                                                                                                                                                                                                  |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création de l'ordre de préparation                                                                                                                                                                                                                                 |
| **Au**                 | La tranche haute filtrant sur la date de création de l'ordre de préparation                                                                                                                                                                                                                                 |
| **Statuts**            | Le(s) statut(s) des ordres de préparation à filtrer                                                                                                                                                                                                                                                         |
| **Numéros de demande** | Pour filtrer sur les numéros de demande de livraison ayant générés les ordres                                                                                                                                                                                                                               |
| **Utilisateurs**       | Pour filtrer sur la personne ayant traitée l'ordre de préparation. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Type**               | Le type des ordres de préparation à filtrer                                                                                                                                                                                                                                                                 |

### Contenu du tableau

| Colonne              | Description                                                        |
| -------------------- | ------------------------------------------------------------------ |
| **Numéro**           | Numéro de l'ordre de préparation                                   |
| **Statut**           | Statut de l'ordre de préparation                                   |
| **Date de création** | Date de création de l'ordre de préparation                         |
| **Opérateur**        | Opérateur ayant traité l'ordre de préparation                      |
| **Type**             | Type de la demande de livraison ayant créée l'ordre de préparation |

### Détails de l'ordre de préparation

L'ordre de préparation est constituée d'une entête et d'un tableau contenant la liste des références à préparer.

L'entête est constituée des champs :&#x20;

* **Numéro** : numéro de l'ordre de préparation
* **Statut** : statut actuel de l'ordre de préparation
* **Point de livraison** : emplacement où livrer les références demandées
* **Opérateur** : opérateur ayant traité l'ordre de préparation. Le champ est donc rempli seulement si l'ordre de préparation est préparé
* **Demandeur** : personne ayant créée la demande ayant générée l'ordre de préparation

Dans cette entête se trouve également les boutons :&#x20;

* <mark style="background-color:blue;">**Finir la préparation**</mark> : pour finir la préparation. Ce bouton clôture la préparation à certaines conditions, voir plus bas, et génère ainsi un ordre de livraison. Il n'est plus disponible lorsque la préparation est préparée.&#x20;
* Sous la flèche :&#x20;
  * **Supprimer** : bouton disponible seulement si l'ordre n'est pas au statut Préparé. Suppression de l'ordre de préparation. La demande passera alors en état Brouillon
  * **Imprimer les étiquettes** :  impression des étiquettes de code barre des articles et des références à livrer
  * **Retourner à la demande de livraison** : pour aller sur la demande de livraison ayant générée l'ordre de préparation
  * **Aller vers l'ordre de livraison** : bouton disponible si l'ordre de préparation est au statut Préparé. Permet d'aller sur l'ordre de livraison généré suite au traitement de la préparation
  * **Associer à un capteur** : disponible seulement pour les collectes de mise en stock. Pour associer les articles de l'ordre de collecte à un capteur de température ou GPS et suivre la collecte

Tableau de la liste des articles :&#x20;

| Colonne                          | Description                                                                                                                                                                                                                        |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Référence**                    | Référence à livrer                                                                                                                                                                                                                 |
| **Libellé**                      | Libellé de la référence à livrer                                                                                                                                                                                                   |
| **Emplacement**                  | Emplacement où se situe la référence à livrer                                                                                                                                                                                      |
| **Emplacement cible de picking** | Colonne apparaissant si le paramétrage "Faire apparaitre l'emplacement cible de picking à l'ajout d'une référence et dans son traitement" est activé. Emplacement où allant prélever la quantité en stock de la référence à livrer |
| **Quantité en stock**            | Quantité en stock de la référence à livrer                                                                                                                                                                                         |
| **Quantité à prélever**          | Quantité à livrer de la référence                                                                                                                                                                                                  |
| **Quantité prélevée**            | Quantité prête pour la livraison                                                                                                                                                                                                   |

Sur chaque ligne, vous avez accès au bouton<img src="../../../.gitbook/assets/3-points.png" alt="" data-size="line">qui donne accès aux boutons suivants :&#x20;

* Bouton <mark style="background-color:blue;">**Voir**</mark> : ouvre la fiche _**Article de référence**_ pour les références gérées par référence ou pour les références gérées par article dont l'article à livrer n'a pas encore été sélectionné. Pour les références gérées par article et dont l'article a été sélectionné, ce bouton ouvre la modale _**Détail de l'article**_
* Bouton <mark style="background-color:blue;">**Imprimer**</mark> : bouton disponible pour les références en gestion quantité par référence ou pour les référence en gestion quantité par article dont l'article a été sélectionné. Ce bouton imprime l'étiquette de référence ou l'étiquette de l'article

### Traiter l'ordre de préparation

Il est possible de traiter l'ordre de préparation sur la supervision, ce que nous allons voir ici. Pour voir le traitement sur le terminal mobile, voir [Stock > Fonctionnalités mobiles > Préparation](../../fonctionnalites-mobile/stock-i-preparation.md).

#### Valider les quantités préparés

Pour pouvoir cliquer sur **Finir la préparation**, il faut d'abord venir renseigner les quantités prélevées de la référence et quels articles sont pris pour la livraison. Selon la gestion quantité de la référence et la façon dont elle a été ajoutée sur la demande de livraison, plusieurs cas sont possibles pour la sélection de la quantité sur la préparation

**Référence en gestion quantité par référence**

Pour préparer une référence en gestion quantité par référence, cliquez sur la ligne de la référence à préparer. Une modale _**Modifier la quantité**_ va s'ouvrir alors. Le champ _Quantité_ sera déjà rempli avec la quantité à prélever, soit la quantité demandée en livraison sur la demande.&#x20;

Si vous préparez toute la quantité demandée, laissez la quantité et appuyez sur <mark style="background-color:blue;">**Enregistrer**</mark>.

Si vous préparez une quantité inférieure à la quantité demandée, renseignez cette quantité et appuyez sur <mark style="background-color:blue;">**Enregistrer**</mark>

Dans les 2 cas, la ligne deviendra verte.&#x20;

{% embed url="https://www.screencast.com/t/lyKmo0AFXA" %}
Préparation avec référence en gestion quantité par référence
{% endembed %}

{% hint style="info" %}
Vous ne pouvez pas préparer une quantité supérieure à la quantité demandée.
{% endhint %}

**Référence en gestion quantité par article + ajout de la référence sur la demande par un utilisateur en ajout quantité par article**

Dans ce cas, la validation de la quantité est la même que dans le cas décrit précédemment.

**Référence en gestion quantité par article + ajout de la référence sur la demande par un utilisateur en ajout quantité par référence**

Dans ce cas, lorsque vous cliquez sur la ligne de la référence à préparer, une modale pour choisir les articles préparés va alors s'ouvrir. La modale contient une recherche rapide pour chercher directement l'article souhaité et un tableau avec les colonnes suivantes :&#x20;

| Colonne                    | Description                                                                                                                                                                                                                                                                                    |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Code barre**             | Code barre de l'article de la référence à préparer                                                                                                                                                                                                                                             |
| **Libellé**                | Libellé de l'article de la référence à préparer                                                                                                                                                                                                                                                |
| **Quantité**               | Quantité de l'article                                                                                                                                                                                                                                                                          |
| **Emplacement**            | <p>Emplacement de l'article<br>Si un emplacement de picking est indiqué sur la demande, les articles sur cet emplacement seront présentés en premier</p>                                                                                                                                       |
| Date **d'entrée en stock** | <p>Cette colonne apparait si la référence à préparer est gestion de stock FIFO. Date à laquelle l'article est entrée en stock<br>Les articles ayant la date d'entrée en stock la plus ancienne seront présentés en premier, après les articles sur l'emplacement de picking s'il y en a un</p> |
| **Date d'expiration**      | <p>Cette colonne apparait si la référence à préparer est gestion de stock FEFO. Date à laquelle l'article va périmer<br>Les articles ayant la date d'expiration la plus proche dans le temps seront présentés en premier, après les articles sur l'emplacement de picking s'il y en a un</p>   |
| **Quantité prélevée**      | Choix de la quantité à prendre de l'article                                                                                                                                                                                                                                                    |

Pour sélectionner l'article prélevée, allez dans la colonne Quantité prélevée. Si vous prenez toute la quantité de l'article, cochez le switch _Quantité totale ?_ sur la ligne de l'article voulu pour prendre tout l'article. Si vous ne prenez qu'une quantité de l'article, inscrivez la quantité prélevée dans le champ _Quantité_. Vous pouvez prendre plusieurs articles pour attendre la quantité totale également.&#x20;

Vous pouvez prélever une quantité inférieure à la quantité demandée et quand même valider la préparation.

{% hint style="info" %}
Vous ne pouvez pas préparer une quantité supérieure à la quantité demandée.&#x20;
{% endhint %}

Une fois les articles choisis, cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>. La ligne passera alors en vert.

{% embed url="https://www.screencast.com/t/9Eck0HHM3XM5" %}
Préparation avec référence en gestion quantité par article
{% endembed %}

#### Valider la préparation

Si au moins une ligne de votre préparation est passée en vert, vous pouvez cliquez sur <mark style="background-color:blue;">**Finir la préparation**</mark>.&#x20;

Une modale _**Valider la préparation**_ s'ouvre alors. Vous devez alors indiquer l'emplacement sur lequel les références ont été préparées.&#x20;

Suite à la validation de la préparation, il va alors se passer :&#x20;

* L'**ordre de préparation** passe au statut _**Préparé**_, ou _**Partiellement préparé**_ si toute la quantité n'est pas préparée ou toutes les références ne sont pas préparées
* La **demande de livraison** passe au statut **Préparé**, ou _**Partiellement préparé**_&#x20;
* Un **ordre de livraison** est généré au statut _**À traiter**_
* Si l'**ordre de préparation** de base est au statut _**Partiellement préparé**_, un **ordre de préparation** est généré au statut _**A traiter**_ contenant les références dans les quantités non préparées&#x20;
* Un **mouvement de transfert** est créé pour chaque référence/article de l'ordre de préparation allant de l'emplacement de stockage de la référence ou de l'article, jusqu'à l'emplacement de préparation indiqué (Ordre > mouvement de stock)

