# Types et champs libres

Les types permettent de venir différencier des flux différents de demande d'acheminement, qui auront chacun leur process de traitement différent.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton <mark style="background-color:blue;">**Modifier**</mark>, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

<figure><img src="../../../.gitbook/assets/Capture d’écran 2025-08-14 à 15.08.29.png" alt=""><figcaption></figcaption></figure>

### **Ajouter un type**

Pour ajouter un type, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter un type**</mark>, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
* **Couleur :** Permet de définir une couleur spécifique à un type d'acheminement. Cette couleur sera utilisée sur l'interface web sous forme de badge dans le détail de chaque acheminement. Sur l'interface nomade, la même couleur permettra d'afficher les acheminements de manière visuelle et rapide, aidant les utilisateurs à reconnaître facilement le type d'acheminement à traiter.
* **Emplacement de prise par défaut** : vous pouvez renseigner pour ce type l'emplacement de prise systématique de ce flux
* **Emplacement(s) de prise suggéré(s)** :  Vous permet de définir une liste exhaustive d'emplacements. L'utilisateur ne pourra sélectionner que les emplacements renseignés dans les paramétrages "Emplacement de prise suggérés"
* **Emplacement de dépose par défaut** : vous pouvez renseigner pour ce type l'emplacement de dépose systématique de ce flux
* **Emplacements de dépose suggéré(s)** :  Vous permet de définir une liste exhaustive d'emplacements. L'utilisateur ne pourra sélectionner que les emplacements renseignés dans les paramétrages "Emplacement de dépose suggérés"
* **Notifications push** : choisissez de déclencher, ou non, des notifications sur le terminal mobile pour ce type. Vous pouvez choisir de déclencher les notifications seulement si la demande est urgente en sélectionnant "Activer seulement si urgence" et en choisissant les valeurs de l'urgence
* **Par défaut :** Ce type d'acheminement sera sélectionné par défaut lors de la création d'une demande d'acheminement par l'utilisateur si ce paramètre est activé.
* **Les statuts de ce type sont réutilisables :** Si votre workflow n'autorise pas la réutilisation des statuts déjà utilisés dans l'historique des acheminements, vous devez activer ce paramètre.
* **Actif :** Si cette coche n'est pas active ce type d'acheminement ne pourra pas être utilisé.

### Définition des Règles pour le Paramétrage des Emplacements de Prise et Dépose Suggérés

#### **Emplacements de Prise Suggérés et Emplacements de Dépose Suggérés** 

1.  **Aucun Champ Saisi** :&#x20;

    * Si les champs "Emplacement de prise par défaut", "Emplacement de dépose par défaut", "Emplacement de prise suggéré" et "Emplacement de dépose suggéré" ne sont pas saisis lors de la création d'un type d'acheminement, les champs "Emplacement de prise" et "Emplacement de dépose" ne seront pas remplis lors de la création d'une demande d'acheminement.&#x20;

    L'utilisateur pourra sélectionner n'importe quel emplacement enregistré dans le référentiel "Emplacement".
2.  **Champs Par Défaut Saisis** : &#x20;

    * Si les champs "Emplacement de prise par défaut" et "Emplacement de dépose par défaut" sont saisis, ces champs ne doivent pas influencer les champs "Emplacements de prise suggérés" et "Emplacements de dépose suggérés", qui ne sont pas obligatoires.&#x20;

    Lors de la création d'une demande d'acheminement, les champs "Emplacement de prise par défaut" et "Emplacement de dépose par défaut" seront pré-remplis, mais il sera toujours possible de les modifier et de sélectionner n'importe quel emplacement enregistré dans le référentiel "Emplacement".
3.  **Champs Suggérés Saisis** :&#x20;

    * Si les champs "Emplacements de prise suggérés" et "Emplacement de dépose suggérés" sont saisis, mais pas les champs "Emplacements de prise par défaut" et "Emplacement de dépose par défaut", alors lors de la création d'une demande d'acheminement, les champs "Emplacement de prise" et "Emplacement de dépose" ne seront pas pré-remplis.&#x20;

    L'utilisateur ne pourra sélectionner que les emplacements renseignés dans les paramétrages "Emplacement de prise suggérés" et "Emplacement de dépose suggérés".
4.  **Tous les Champs Saisis** :&#x20;

    * Si les champs "Emplacement de prise par défaut", "Emplacement de dépose par défaut", "Emplacements de prise suggérés" et "Emplacements de dépose suggérés" sont saisis, alors lors de la création d'une demande d'acheminement, les champs "Emplacement de prise" et "Emplacement de dépose" seront pré-remplis.&#x20;

    Si l'utilisateur souhaite les modifier, il ne pourra sélectionner que les emplacements renseignés dans les paramétrages "Emplacements de prise suggérés" et "Emplacements de dépose suggérés".



**Vous pouvez ensuite ajouter des champs libres sur ce type en cliquant sur la ligne avec le +, et en complétant le tableau de la façon suivante :**&#x20;

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
