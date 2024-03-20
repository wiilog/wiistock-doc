---
description: Ensemble des paramétrages pour les demandes de livraison
---

# Livraisons

## Livraisons

Cette partie sert à paramétrer le comportement de création d'une livraison

### Création livraison

* **Gérer le champ "Destination" en liste déroulante** : cochez ce paramétrage pour ne pas à avoir à taper une première lettre pour voir la liste des emplacements dans le champ Destination lors d'une création de demande de livraison (que ça soit via le +, le panier, ou une réception)
* **La livraison est directement préparée à sa validation** : L'ordre de livraison est directement mis en préparé et l'ordre de livraison est généré à la validation de la demande de livraison, sauf si les références / articles sur la demande sont sur des emplacements différents au moment de la validation de la demande livraison.
* Ne pas gérer les quantités en stock : Aucun contrôle de quantité ne sera effectué sur aucune des étapes de la livraison. Des articles seront générés automatiquement à la validation de la demande de livraison.

### Création livraison après réception

* **"Demande de livraison" coché par défaut sur réception :** Lors d'une réception, la création d'une demande de livraison sera sélectionnée par défaut.
* **Comportement de la demande de livraison** : lors d'une réception, vous pouvez choisir un des 3 comportements suivants concernant la demande de livraison
  * **Création seulement de la demande de livraison en "A traiter"** : La demande de livraison sera créée sans préparation.
  * **Création de la demande de livraison avec sa préparation** : la demande sera automatiquement créée au statut A traiter avec l'ordre de préparation associé aussi au statut À traiter.
  * **Livraison directe : passage direct à l'ordre de livraison** : la demande de livraison se crée, l'ordre de préparation généré soit directement au statut Préparé et ainsi qu'un ordre de livraison soit automatiquement généré au statut A traiter. Cela permet ainsi d'éviter l'étape de préparation
  *
* **Le demandeur est l'utilisateur de la session en cours** : activez ce paramétrage pour que, lors d'une demande de livraison créée via l'étape de conditionnement d'une réception, le demandeur soit automatiquement rempli avec l'utilisateur de la session en cours

### Ajout référence&#x20;

* **Faire apparaître l'emplacement cible de picking à l'ajout d'une référence et dans son traitement** : si vous activez ce paramétrage, lorsque vous ajoutez une référence gérée par article dans une demande de livraison, vous pourrez renseigner sur quel emplacement venir prélever la quantité demandée. Il sera présenté en priorité à l'opérateur qui effectue la préparation les articles présents sur l'emplacement de picking noté
* **Ajout d'unité logistique** : Deux possibilité de contenant dans les demandes de livraisons. Si ce paramétrage n'est pas coché, ce seront des références à ajouter, dans le cas contraire des unités logistiques.&#x20;
* **Préremplir le champ commentaire de la ligne si le code projet de la référence est défini avec :** Possibilité d'intégrer les variable @Projet et @Destinataire.&#x20;
* **Préremplir le champ comment commentaire de la ligne si le code projet de la référence n'est pas défini avec** : Possibilité d'intéfrer la variable @Destinataire.&#x20;

### Emplacements de livraison par défaut

Vous pouvez indiquer pour chaque type de livraison un emplacement par défaut. Ainsi, lorsque vous créez une demande de livraison, que ce soit via le +, le panier, ou une réception, la destination sera automatiquement remplie lorsque vous aurez renseigné le type.&#x20;

Pour paramétrer un emplacement de livraison par défaut, cliquez sur **Ajouter un emplacement**. Vous devez ensuite renseigner l'association _Type_ - _Emplacement_. Vous pouvez créer autant s'association qu'il y a de types de livraison.&#x20;

Supprimez une association en appuyant sur la poubelle à droite de la ligne souhaitée.&#x20;

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

## Livraisons - Modèles de demande

Les modèles de demande sont utilisés dans l'application Wiilog dans le cadre des objets connectés pour le moment. Ainsi, un objet connecté peut déclencher une demande de livraison directement au statut A traiter avec son ordre de préparation au statut A traiter en se basant sur un modèle de demande paramétré

La page des modèles de demande est constituée de 2 zones :&#x20;

* une entête avec le sélection du modèle de demande et le bouton Ajouter un modèle de demande
* Le détail du modèle de demande de livraison

{% embed url="https://www.screencast.com/t/Me8oHhSyj" %}
Page modèles de demande
{% endembed %}

### **Ajouter un modèle de demande**

Pour ajouter un modèle de demande, cliquez sur <mark style="background-color:blue;">**Ajouter un modèle de demande**</mark> à droite de l'entête. La page passe alors en mode ajout.

Il faut alors remplir les champs suivants :&#x20;

* **Nom du modèle\*** : libellé du modèle pour l'identifier lors de l'association à un objet connecté
* **Type de livraison\*** : type de la livraison lors de la création de la livraison
* **Destination\*** : emplacement de livraison
* **Commentaire** : commentaire sur la livraison. Cliquez sur le logo dans le champ pour avoir plus de possibilité dans l'édition de votre commentaire![](<../../../.gitbook/assets/Capture d’écran 2022-03-23 à 17.17.00.png>)
* Les **champs libres** : renseignez les champs libres liés au type

Renseignez ensuite la liste des articles à mettre sur la demande

{% hint style="info" %}
Sur une demande de livraison créée par modèle de demande, les références seront toujours ajoutées par référence même pour les références en gestion quantité par article. Le choix des articles à livrer sera fait au moment de la préparation par la personne qui traitera l'ordre
{% endhint %}

Renseignez le tableau de la façon suivante en cliquant sur la ligne avec le + pour ajouter une référence :&#x20;

| Colonne               | Description                                                                               |
| --------------------- | ----------------------------------------------------------------------------------------- |
| **Référence**         | Code de la référence à livrer lors de l'appel au modèle                                   |
| **Libellé**           | Libellé de la référence à livrer. Se renseigne tout seul une fois le code renseigné       |
| **Emplacement**       | Emplacement sur lequel est la référence. Se complète tout seul une fois le code renseigné |
| **Quantité à livrer** | Quantité demandée de la référence en livraison                                            |

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour ajouter le modèle.

### **Modifier un modèle de demande**

Pour modifier un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez modifier, et cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> dans la zone de détails d'un modèle de demande de livraison. La page passera alors en mode modification. Modifiez les champs comme pour la création.

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider les modifications.&#x20;

### **Supprimer un modèle de demande**

Pour supprimer un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez supprimer, et cliquez sur le bouton poubelle dans la zone de détails d'un modèle de demande de livraison.&#x20;

Vous pouvez supprimer un modèle s'il n'est pas utilisé dans une association avec un objet connecté.&#x20;

## Types et champs libres

Les types permettent de venir différencier des flux différents de demande de livraison.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton <mark style="background-color:blue;">**Modifier**</mark>, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

{% embed url="https://www.screencast.com/t/a4l0q9GOFor" %}
Page types et champs libres
{% endembed %}

### **Ajouter un type**

Pour ajouter un type, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
* **Notifications push** : choisissez de déclencher, ou non, des notifications sur le terminal mobile pour ce type
* **Envoi d'un email au demandeur** : si vous cochez ce paramétrage, un email sera envoyé au demandeur quand la demande sera traitée

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

{% embed url="https://www.screencast.com/t/stqaN1dQ" %}
Ajouter un types et ses champs libres
{% endembed %}

### **Modifier un type et ses champs libres**

Pour modifier un type et ses champs libres, cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> à droite des caractéristiques du type.

La page passe alors en mode modification. Vous pouvez modifier les caractéristiques et les champs libres de la même façon que décrit au-dessus. Le typage des champs libres ne peut pas être modifié.

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

{% embed url="https://www.screencast.com/t/fsGBeqCIUm" %}
Modifier un type et ses champs libres
{% endembed %}

### **Supprimer un type et ses champs libres**

Vous pouvez supprimer un type et ses champs libres grâce aux poubelles : une à gauche des caractéristiques du type pour supprimer le type, une sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.

{% hint style="info" %}
Pour supprimer un type, le type ne doit plus avoir des champs libres et ne pas être utilisé sur les livraisons.&#x20;
{% endhint %}

## Champs fixes

Les champs fixes permettent de choisir quels champs sont disponibles sur le formulaire de création d'un livraison, de modification, et s'il est possible de filtrer sur ce champ ou non.

Pour chaque champ, choisissez les éléments suivants :&#x20;

* **Formulaire de création :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de création d'une réception
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de créer une réception sans que ce champ soit renseigné sur le formulaire de création de réception
* **Formulaire d'édition :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de modification d'une réception
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de valider la modification d'une réception sans que ce champ soit renseigné sur le formulaire de modification d'une réception
* **Sur les filtres :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent dans la barre de filtres de la page des réceptions. Si la case est grisée, cela signifie que ce champ n'est pas disponible au filtrage

{% embed url="https://www.screencast.com/t/39L1WXHSN0jG" %}
Champs fixes livraison
{% endembed %}

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.
