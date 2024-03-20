# Demandes

## Configurations

### Demande sous-traitée

**Message paramétrable si la date et heure de la demande sont hors horaires travaillés** : Renseigner le message qui apparaîtra si une demande de livraison est créée sur des horaires non travaillés.

### Bon de transport

Le bon de transport est disponible pour les livraisons et les livraisons/collectes à partir du statut À livrer, il se compose de plusieurs infos paramétrable :

* Coordonnées société
* Donneur d'ordre
* Coordonnées expéditeur
* Logo sur bon de transport

### Demande de livraison

**Valeurs du champ Urgence** : renseignez les notions d'urgence que vous voulez mettre en place, elles apparaîtront sur la demande et l'ordre de transport.

### Demande à valider

**Destinataire(s) mail** : ajouter les utilisateurs qui recevront un mail lorsque des demandes de transport seront au statut **En attente de validation**.

##

## Livraisons - Types et champs libres

Les types permettent de venir différencier des flux différents de demande de livraison.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton <mark style="background-color:blue;">**Modifier**</mark>, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

{% embed url="https://www.screencast.com/t/swJl4Chtlkt" %}
Page des types et Champs libres
{% endembed %}

### **Ajouter un type**

Pour ajouter un type, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
* **Logo\*** : Choisissez un logo/icone qui va représenter le type, cela permettra de reconnaître plus facilement et rapidement les différentes demandes de livraison

Vous pouvez ensuite ajouter des champs libres sur ce type en cliquant sur la ligne avec le <mark style="background-color:blue;">**+**</mark>, et en complétant le tableau de la façon suivante :&#x20;

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

### **Modifier un type et ses champs libres**

Pour modifier un type et ses champs libres, cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> à droite des caractéristiques du type.

La page passe alors en mode modification. Vous pouvez modifier les caractéristiques et les champs libres de la même façon que décrit au-dessus. Le typage des champs libres ne peut pas être modifié.

{% embed url="https://www.screencast.com/t/uW8COToxNPV" %}
Page en mode modification
{% endembed %}

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

### **Supprimer un type et ses champs libres**

Vous pouvez supprimer un type et ses champs libres grâce aux poubelles : une à gauche des caractéristiques du type pour supprimer le type, une sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.

{% hint style="info" %}
Pour supprimer un type, le type ne doit plus avoir des champs libres et ne pas être utilisé sur les livraisons.&#x20;
{% endhint %}



## Collectes - Types et champs libres

Les types permettent de venir différencier des flux différents de demande de collecte.

Cette page fonctionne de la même façon que pour les types et champs libres que la livraison. Nous vous invitons à la consulter pour savoir comment ajouter, modifier et supprimer les types et champs libres d'une collecte.

{% embed url="https://www.screencast.com/t/XnLfid6CG" %}
Page types et champs libres de collectes
{% endembed %}
