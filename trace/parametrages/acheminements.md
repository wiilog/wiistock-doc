# Acheminements

## Configurations

Cette section sert à paramétrer le comportement de création d'un acheminement et lors de l'ajout de colis dans un acheminement.

* **Pré-remplir la date du jour dans le champ à échéance Du et échéance Au** : même si vous n'avez pas paramétré d'afficher le champ fixe Date d'échéance sur le formulaire de création d'acheminement, la date d'échéance sera automatiquement remplie avec la date du jour, que cela soit pour la borne basse ou la borne haute des dates d'échéances
* **Ajouter le numéro d'acheminement en préfixe du colis lors de l'ajout de colis :** lorsque vous ajoutez un colis sur un acheminement, le colis aura automatiquement en préfixe le numéro d'acheminement
* **Le colis ajouté dans l'acheminement ne peut pas exister en base (doit être nouveau) :** lorsque vous ajouter un colis dans un acheminement, celui-ci doit être nouveau, il ne doit pas déjà être dans la liste des colis

Lorsque vous avez modifié un des paramétrages, n'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider vos changements.

## Statuts

Pour traiter un acheminement, il faut le faire passer par une succession de statuts. Ces statuts sont paramétrables.

Lorsque vous arrivez sur la partie Statuts, vous avez 2 partie :&#x20;

* une section en haut avec les types des acheminements (vous ne pouvez pas paramétrer les statuts si vous n'avez pas paramétré les types). Cliquez sur un type pour filtrer les statuts par rapport au type
* une section avec la liste des statuts. La liste des statuts est tous types confondus si vous n'avez pas cliquez sur un type. Vous pouvez faire une recherche rapide sur la liste si elle contient plus de 10 lignes. Les colonnes du tableau sont triables.&#x20;

{% embed url="https://www.screencast.com/t/mM5mCCskkI" %}
Page statuts
{% endembed %}

### **Ajouter des statuts**

Pour ajouter des statuts, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter des statuts**</mark>. La page va alors passer en mode ajout. Si vous souhaitez ajouter plusieurs statuts à la fois, appuyez sur le + en bas de la première ligne. Remplissez le tableau de cette façon :&#x20;

* **Libellé\*** : nom du statut qui apparaîtra dans l'application
* **Etat\*** : état du statut. L'état d'un statut conditionne les actions que l'on peut faire sur un acheminement. 4 états sont disponibles :&#x20;
  * _**Brouillon**_ : la demande est en cours de construction et pas encore validée. Elle n'apparaitra pas sur le nomade. Il est possible d'ajouter des colis sur une demande en brouillon. Une date de création est affectée à la demande avec la personne l'ayant créée. Vous ne pouvez avoir qu'un seul statut en état Brouillon par type d'acheminement
  * _**A traiter**_ : la demande est validée. Elle apparait sur le nomade (si Synchronisation nomade est cochée, voir plus loin). Il n'est plus possible d'ajouter de colis sur la demande. Une date de validation est affectée sur la demande
  * _**Partiel**_ : si seulement une partie des colis a été transférée sur le nomade, il est possible de sélectionner un statut en état Partiel
  * _**Traité**_ : l'acheminement est terminé. Il n'apparaît plus sur le nomade. Une date de traitement lui est affectée avec la personne l'ayant traité
* **Type\*** : type de l'acheminement. Les statuts dépendent du type, ce qui permet d'avoir des workflow différents en fonction du type de l'acheminement
* **Envoi d'emails au demandeur** : si ce paramétrage est cochée, un mail est envoyé au demandeur (personne ayant créée la demande) lorsque l'acheminement passe à ce statut
* **Envoi d'emails aux destinataires** : si ce paramétrage est cochée, un mail est envoyé aux destinataires de l'acheminement (destinataires renseignés sur l'acheminement au moment de sa création) lorsque l'acheminement passe à ce statut
* **Synchronisation nomade** : si ce paramétrage est coché, un acheminement qui est à ce statut sera visible sur le nomade. Ce paramétrage n'est disponible que pour les statuts en état A traiter ou Partiel
* **Ordre\*** : ordre dans la liste des statuts sur le paramétrage

Pour qu'un acheminement ait un workflow cohérent, il faut au minimum un statut en état Brouillon, un A traiter, et un Traité. S'il est possible qu'une partie seulement des colis soient acheminés sur une demande, il faut faudra avoir un statut en état Partiel.

Une fois que vous avez ajouté tous les statuts que vous souhaitez, cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>. Ils s'ajouteront dans la liste des statuts.

{% embed url="https://www.screencast.com/t/ojqwdnns" %}
Ajouter des tatuts
{% endembed %}

### **Modifier des statuts**

Pour modifier des statuts, cliquez sur une ligne en mode visualisation pour passer en mode modification. Vous pouvez modifier les champs de la même façon qu'à la création, sauf le type qui ne peut plus être modifié.&#x20;

{% embed url="https://www.screencast.com/t/t3LgmKon9UQ" %}
**Modifier des statuts**
{% endembed %}

### **Supprimer des statuts**

Pour supprimer des statuts, cliquez sur la poubelle de la ligne du statut que vous souhaitez supprimer, que ce soit en mode visualisation ou modification. Vous ne pouvez pas supprimer un statut s'il est utilisé sur un acheminement.

## Champs fixes

Les champs fixes permettent de choisir quels champs sont disponibles sur le formulaire de création d'un acheminement, de modification, et s'il est possible de filtrer sur ce champ ou non.

Pour chaque champ, choisissez les éléments suivants :&#x20;

* **Formulaire de création :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de création d'acheminement
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de créer un acheminement sans que ce champ soit renseigné sur le formulaire de création d'acheminement
* **Formulaire d'édition :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de modification d'acheminement
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de valider la modification d'un acheminement sans que ce champ soit renseigné sur le formulaire de modification d'acheminement
* **Sur les filtres :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent dans la barre de filtres de la page des acheminements. Si la case est grisée, cela signifie que ce champ n'est pas disponible au filtrage

{% embed url="https://www.screencast.com/t/nTBDZKBHwikU" %}
Page champs fixes
{% endembed %}

Certains champs fixes possèdent également un paramétrage des valeurs disponibles. C'est le cas du champ **Urgence** et **Business unit**. Cliquez sur le libellé du champ fixe pour ouvrir une modale pour paramétrer les valeurs possibles du champ fixe.

![Paramétrage des valeurs du champ fixe](../../.gitbook/assets/2022-02-04\_14-47-55.png)

N'oubliez pas de cliquer sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre modification

## Types & champs libres

Les types permettent de venir différencier des flux différents de demande d'acheminement, qui auront chacun leur process de traitement différent.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton <mark style="background-color:blue;">**Modifier**</mark>, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

{% embed url="https://www.screencast.com/t/syieN28l" %}
Page Types et champs libres
{% endembed %}

### **Ajouter un type**

Pour ajouter un type, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
* **Emplacement de prise par défaut** : vous pouvez renseigner pour ce type l'emplacement de prise systématique de ce flux
* **Emplacement de dépose par défaut** : vous pouvez renseigner pour ce type l'emplacement de prise systématique de ce flux
* **Notifications push** : choisissez de déclencher, ou non, des notifications sur le terminal mobile pour ce type. Vous pouvez choisir de déclencher les notifications seulement si la demande est urgente en sélectionnant "Activer seulement si urgence" et en choisissant les valeurs de l'urgence

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

{% embed url="https://www.screencast.com/t/tJh9Tvvjb" %}
&#x20;Ajouter un type et des champs libres
{% endembed %}

### **Modifier un type et ses champs libres**

Pour modifier un type et ses champs libres, cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> à droite des caractéristiques du type.

La page passe alors en mode modification. Vous pouvez modifier les caractéristiques et les champs libres de la même façon que décrit au-dessus. Le typage des champs libres ne peut pas être modifié.

{% embed url="https://www.screencast.com/t/eMDxQ2jswFr" %}
Modifier un type et ses champs libres
{% endembed %}

### **Supprimer un type et ses champs libres**

Vous pouvez supprimer un type et ses champs libres grâce aux poubelles : une à gauche des caractéristiques du type pour supprimer le type, une sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.

Pour supprimer un type, le type ne doit plus avoir des champs libres et ne pas être utilisé sur les acheminements.&#x20;

## Lettre de voiture

La lettre de voiture est un document qui peut être généré à partir d'un acheminement pour que le transporteur justifie des marchandises qu'il transporte.

Ce paramétrage sert à régler des éléments par défaut sur ce document afin de ne pas avoir à les ressaisir sur la modale de génération de lettre de voiture.

Choisissez le logo à mettre sur la lettre de voiture, et remplissez les différents champs où vous souhaitez avoir des valeurs par défaut dans la modale de configuration de lettre de voiture.

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

## Bon de surconsommation

Cette section de paramétrage sert à paramétrer un document généré sur les acheminements&#x20;

* **Génération bon de surconsommation pour type \[] passe acheminement au statut \[] :** choisissez le type de votre acheminement sur lequel vous utilisez le bon de surconsommation et choisissez le statut auquel votre acheminement doit passer quand vous cliquez sur Générer le bon de surconsommation
* **Logo du bon de surconsommation :** choisissez le logo qui apparaitra en haut à droite du bon de surconsommation

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.
