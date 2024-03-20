# Réceptions

## Statuts

Les statuts ne sont pas paramétrables sur les réceptions mais vous pouvez personnaliser le nom de réception.&#x20;

**Emplacement de réception par défaut** : lorsque vous créez une réception, les articles créés seront automatiquement déposés sur l'emplacement de réception par défaut

**Renommer les statuts de réception** : 4 statuts sont possibles sur les réceptions

* _**En attente de réception**_ : la réception vient d'être créée
* _**Réception partielle**_ : la réception était terminée mais elle a été annulée
* _**Réception totale**_ : la réception est terminée (clic sur _**Fin réception**_)
* _**Anomalie**_ : switch Anomalie coché car anomalie relevée sur la réception

Vous pouvez renommer tous les statuts

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

## Champs fixes&#x20;

Les champs fixes permettent de choisir quels champs sont disponibles sur le formulaire de création d'une réception, de modification, et s'il est possible de filtrer sur ce champ ou non.

Pour chaque champ, choisissez les éléments suivants :&#x20;

* **Formulaire de création :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de création d'une réception
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de créer une réception sans que ce champ soit renseigné sur le formulaire de création de réception
* **Formulaire d'édition :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de modification d'une réception
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de valider la modification d'une réception sans que ce champ soit renseigné sur le formulaire de modification d'une réception
* **Sur les filtres :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent dans la barre de filtres de la page des réceptions. Si la case est grisée, cela signifie que ce champ n'est pas disponible au filtrage

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

{% embed url="https://www.screencast.com/t/2MCKa3CMF" %}
Page des champs fixes
{% endembed %}

## Champs libres

Il est possible d'ajouter des champs libres sur les réceptions. Les champs libres sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

### Ajouter et modifier des champs libres

Cliquez dans le tableau pour le passer en mode modification et ajout.&#x20;

Vous pouvez modifier les lignes déjà remplies.

Pour ajouter un champ libre, cliquez sur la dernière ligne avec le +, et remplissez les champs suivants :&#x20;

| Colonne                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Libellé**                       | Nom du champ libre.  Le nom doit être différent de tous les champs libres paramétrés sur l'application                                                                                                                                                                                                                                                                                                                                                                                           |
| **Typage**                        | <p>Typage du champ libre. 7 types sont possibles : <br>- Texte : champ de saisie libre<br>- Nombre : champ dans lequel il est seulement possible de saisir des nombres<br>- Oui/Non : choix entre 2 choix Oui et Non<br>- Date : le champ ouvrira un calendrier à la selection<br>- Date et heure : le champ ouvrira un calendrier à la sélection et un sélecteur d'heure<br>- Liste : sélection d'un choix parmi une liste<br>- Liste multiple : sélection de plusieurs choix par une liste</p> |
| **Eléments**                      | Eléments de la liste pour les types Liste et Liste multiple                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Valeur par défaut**             | Valeur par défaut du champ libre. En fonction du typage choisi, le modèle de choix du valeur par défaut change                                                                                                                                                                                                                                                                                                                                                                                   |
| **Affiché à la création**         | Cochez la case pour que le champ libre apparaisse à la création du mouvement                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Obligatoire à la création**     | Cochez la case pour que le champ libre soit obligatoire pour valider la création du mouvement                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Obligatoire à la modification** | Cochez la case pour que le champ libre soit obligatoire pour valider la modification de la réception                                                                                                                                                                                                                                                                                                                                                                                             |

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

{% embed url="https://www.screencast.com/t/VlChKsL71th" %}
Ajouter et modifier un champs libre
{% endembed %}

### **Supprimer des champs libres**

Vous pouvez supprimer des champs libres grâce aux poubelles, elles sont disposées à gauche sur chaque ligne de champs libres. Ces poubelles sont présentes en mode visualisation et mode modification.

## Litiges - Statuts

Lorsque vous créez un litige sur une réception, celui-ci doit passer par une liste de statuts afin d'indiquer sa progression jusqu'à sa clôture. Cette progression est paramétrable par le paramétrage de statut. Sur les litiges, les statuts ne dépendent pas du type.

### **Ajouter des statuts**

Pour ajouter des statuts de litige, cliquez sur le bouton **Ajouter** **des statuts** à droite. La page va alors passer en mode ajout. Si vous souhaitez ajouter plusieurs statuts à la fois, appuyez sur le + en bas de la première ligne. Remplissez le tableau de cette façon :&#x20;

* **Libellé\*** : nom du statut qui apparaîtra sur l'application
* **Etat\*** : état du statut. L'état du statut sur les litiges permet de savoir s'il est toujours en cours de résolution ou traité. 2 états sont disponibles :&#x20;
  * _**À traiter**_ : le litige n'est pas clôturé
  * _**Traité**_ : le litige est clôturé
* _**Commentaire litige**_ : commentaire qui apparaîtra automatiquement sur le litige à la sélection du statut
* _**Statut par défaut**_ : à la création du litige, le litige se mettra par défaut sur ce statut
* _**Envoi d'emails aux acheteurs**_ : cochez ce paramétrage pour qu'au passage à ce statut, un mail soit envoyé aux acheteurs de l'arrivage sur lequel il y a un litige
* _**Envoi d'emails au demandeur**_ : cochez ce paramétrage pour qu'au passage à ce statut, un mail soit envoyé au déclarant du litige&#x20;
* _**Ordre**_ : ordre du statut dans la liste des statuts dans le paramétrage

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

{% embed url="https://www.screencast.com/t/rktbMBTDV" %}
Ajouter des statuts
{% endembed %}

### Modifier des statuts

Pour modifier des statuts, cliquez sur une ligne en mode visualisation pour passer en mode modification. Vous pouvez modifier les champs de la même façon qu'à la création.

N'oubliez pas de cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider votre paramétrage.

{% embed url="https://www.screencast.com/t/bMohy6rRs" %}
Modifier des stauts
{% endembed %}

### **Supprimer des statuts**

Pour supprimer des statuts, cliquez sur la poubelle de la ligne du statut que vous souhaitez supprimer, que ce soit en mode visualisation ou modification. Vous ne pouvez pas supprimer un statut s'il est utilisé sur un litige.

## Litiges - Types

Les types de litige servent à venir caractériser votre litige.&#x20;

### &#x20;**Ajouter des types**

Pour ajouter un type de litige, cliquez sur le +. Si vous étiez en mode visualisation, vous passerez en mode modification. Si vous étiez en mode modification une ligne s'ajoutera juste.&#x20;

Remplissez alors les champs suivant :&#x20;

* **Libellé\*** : libellé du litige
* **Description** : description du litige

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour bien ajouter votre type.

{% embed url="https://www.screencast.com/t/ftWthMqN" %}
Ajouter des types
{% endembed %}

### **Modifier des types**

Pour modifier un type de litige, cliquez sur la ligne du type à modifier pour passer en mode modification, et <mark style="background-color:blue;">**enregistrer**</mark>.

### **Supprimer des types**

Pour supprimer un type, cliquez sur le bouton Poubelle de la ligne du type de litige que vous souhaitez supprimer. Ce type ne peut pas être supprimé s'il est utilisé.&#x20;
