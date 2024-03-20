---
description: Ensemble des paramétrages pour les demandes de collectes
---

# Collectes

## Collectes

Cette partie sert à paramétrer le comportement de création d'une demande de collecte.

* **Gérer le champ "Point de collecte" en liste déroulante** : cochez ce paramétrage pour ne pas à avoir à taper une première lettre pour voir la liste des emplacements dans le champ Point de collecte lors d'une création de demande de collecte (que ça soit via le +,ou le panier).

## Collectes - Modèles de demande

Les modèles de demande sont utilisés dans l'application Wiilog dans le cadre des objets connectés pour le moment. Ainsi, un objet connecté peut déclencher une demande de collecte directement au statut A traiter avec son ordre de collecte au statut A traiter en se basant sur un modèle de demande paramétré

La page des modèles de demande est constituée de 2 zones :&#x20;

* une **entête** avec la sélection du modèle de demande et le bouton Ajouter un modèle de demande
* Le **détail du modèle** de demande de collecte

{% embed url="https://www.screencast.com/t/7LfO1dkWY5" %}
Page modèles de demande
{% endembed %}

### **Ajouter un modèle de demande**

Pour ajouter un modèle de demande, cliquez sur <mark style="background-color:blue;">**Ajouter un modèle de demande**</mark> à droite de l'entête. La page passe alors en mode ajout.

Il faut alors remplir les champs suivants :&#x20;

* **Nom du modèle\*** : libellé du modèle pour l'identifier lors de l'association à un objet connecté
* **Objet\*** : objet de la demande de collecte
* **Type de la collecte\*** : type de la collecte lors de la création de la collecte
* **Point de collecte\*** : emplacement de la collecte
* **Commentaire** : commentaire sur la collecte. Cliquez sur le logo dans le champ pour avoir plus de possibilité dans l'édition de votre commentaire
* Les **champs libres** : renseignez les champs libres liés au type
* **Destination\*** : est-ce que les références/articles collectés doivent être détruits ou remis en stock

Renseignez ensuite la liste des articles à mettre sur la demande

{% hint style="info" %}
Sur une demande de collecte créée par modèle de demande, les références seront toujours ajoutées par référence même pour les références en gestion quantité par article. Le choix des articles à collecter sera fait au moment de la collecte par la personne qui traitera l'ordre
{% endhint %}

Renseignez le tableau de la façon suivante en cliquant sur la ligne avec le + pour ajouter une référence :&#x20;

| Colonne                  | Description                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------- |
| **Référence**            | Code de la référence à collecte lors de l'appel au modèle                                 |
| **Libellé**              | Libellé de la référence à livrer. Se renseigne tout seul une fois le code renseigné       |
| **Emplacement**          | Emplacement sur lequel est la référence. Se complète tout seul une fois le code renseigné |
| **Quantité à collecter** | Quantité demandée de la référence en collecte                                             |

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour ajouter le modèle.

### **Modifier un modèle de demande**

Pour modifier un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez modifier, et cliquez sur le bouton Modifier dans la zone de détails d'un modèle de demande de collecte. La page passera alors en mode modification. Modifiez les champs comme pour la création

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider les modifications.&#x20;

### **Supprimer un modèle de demande**

Pour supprimer un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez supprimer, et cliquez sur le bouton poubelle dans la zone de détails d'un modèle de demande de collecte.&#x20;

Vous pouvez supprimer un modèle s'il n'est pas utilisé dans une association avec un objet connecté.&#x20;

## Types et champs libres

Les types permettent de venir différencier des flux différents de demande de collecte.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton <mark style="background-color:blue;">**Modifier**</mark>, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

{% embed url="https://www.screencast.com/t/AWyKPGdYEK" %}
Page types et champs libres
{% endembed %}

### **Ajouter un type**

Pour ajouter un type, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
* **Notifications push** : choisissez de déclencher, ou non, des notifications sur le terminal mobile pour ce type

Vous pouvez ensuite ajouter des champs libres sur ce type en cliquant sur la ligne avec le +, et en complétant le tableau de la façon suivante :&#x20;

* **Libellé\*** : nom du champ libre. Le nom doit être différent de tous les champs libres paramétrés sur l'application&#x20;
* **Typage\*** : contenu du champ. A choisir parmi la liste suivante :&#x20;
  * **Texte** : champ pouvant contenir n'importe quel caractère
  * **Nombre** : champ pouvant contenir seulement des chiffres
  * **Oui/Non** : champ où le choix de réponse est entre Oui ou Non
  * **Date** : champ pouvant contenir seulement une date. Il ouvre un calendrier pour sélectionner une date
  * **Date et heure**: champ pouvant contenir seulement une date et une heure. Il ouvre un calendrier pour sélectionner une date et un sélecteur d'heure
  * **Liste** : valeur du champ à sélectionner parmi une liste de valeurs paramétrée à la colonne suivante. Il sera seulement possible de sélectionner une valeur
  * **Liste multiple** : valeurs du champ à sélectionner parmi une liste de valeurs paramétrée à la colonne suivante. Il sera possible de sélectionner plusieurs valeurs
* **Eléments** : valeurs possibles pour les champs de type Liste et Liste multiple. Ecrivez ici les éléments de la liste, en les séparant par un ;&#x20;
* **Valeur par défaut** : valeur par défaut du champ libre. Selon le type du champ libre, la sélection de la valeur par défaut s'adapte
* **Affiché à la création** : cochez ce paramétrage pour que le champ apparaisse à la création d'un acheminement
* **Obligatoire à la création** : cochez ce paramétrage pour qu'il ne puisse pas être possible de créer un acheminement sans avoir saisi ce champ
* **Obligatoire à la modification** : cochez ce paramétrage pour qu'il ne puisse pas être possible de modifier un acheminement sans avoir saisi ce champ

Une fois que vous avez rempli les caractéristiques et les champs libres du type (vous n'êtes pas obligé d'avoir des champs libres), cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour voir le nouveau type apparaître à la suite des autres.

{% embed url="https://www.screencast.com/t/qUjsEY6O" %}
Ajouter un type et ses champs libres
{% endembed %}

### **Modifier un type et ses champs libres**

Pour modifier un type et ses champs libres, cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> à droite des caractéristiques du type.

La page passe alors en mode modification. Vous pouvez modifier les caractéristiques et les champs libres de la même façon que décrit au-dessus. Le typage des champs libres ne peut pas être modifié.

{% embed url="https://www.screencast.com/t/D2p3R5t3Edai" %}
Modifier un type et ses champs libres
{% endembed %}

### **Supprimer un type et ses champs libres**

Vous pouvez supprimer un type et ses champs libres grâce aux poubelles : une à gauche des caractéristiques du type pour supprimer le type, une sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.

{% hint style="info" %}
Pour supprimer un type, le type ne doit plus avoir des champs libres et ne pas être utilisé sur les collectes.
{% endhint %}
