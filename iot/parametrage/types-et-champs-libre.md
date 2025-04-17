# Types et champs libre

Un type est une classification de vos entités. Sur les IoT, les types sont figés et se réfèrent à la catégorie d'objet connecté. Vous pouvez associer à un type des champs libres afin d'apporter des informations supplémentaires propres à cette classification. Cela vous permet de personnaliser votre application pour votre contexte d'utilisation.

Les types permettent de venir différencier des flux différents des Iot, qui auront chacun leur process de traitement différent.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

<figure><img src="../../.gitbook/assets/image (142).png" alt=""><figcaption></figcaption></figure>

La page des types et champs libres est constituée de 2 zones :&#x20;

* L'entête avec la liste des types. Chaque type est cliquable et permet de voir les caractéristiques des champs libres de ce type.
* La liste des champs libres du type

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

### **Supprimer un champ libre**

Vous pouvez supprimer un champ libre grâce aux poubelles  sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.
