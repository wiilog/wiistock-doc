# Statuts

Pour traiter un achat, il faut le faire passer par une succession de statuts. Ces statuts sont paramétrables.

Lorsque vous arrivez sur la partie Statuts, vous avez la liste des statuts de demande d'achat.&#x20;

### **Ajouter des statuts**

Pour ajouter des statuts, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter des statuts**</mark>. La page va alors passer en mode ajout. Si vous souhaitez ajouter plusieurs statuts à la fois, appuyez sur le + en bas de la première ligne. Remplissez le tableau de cette façon :&#x20;

* **Libellé\*** : nom du statut qui apparaîtra dans l'application
* **Etat\*** : état du statut. L'état d'un statut conditionne les actions que l'on peut faire sur un achat. 4 états sont disponibles :&#x20;
  * _**Brouillon**_ : la demande est en cours de création et n'est pas encore validée. Il est encore possible d'ajouter des références dans la demande. Il sera seulement possible de passer la demande à un statut en état A traiter.&#x20;
  * _**A traiter**_ : la demande est validée. Elle doit être prise en compte par l'acheteur. Il sera seulement possible de passer la demande à un statut en état _En cours_. Une date de validation est indiquée sur la demande.&#x20;
  * _**En cours**_ : pour indiquer que la demande d'achat a été pris en compte par l'acheteur et est en cours de traitement. Il sera seulement possible de passer la demande à un statut en état _Traité_. Une date de prise en compte est indiquée sur la demande.&#x20;
  * _**Traité**_ : la demande d'achat est terminé. Un statut a cet état peut entrainer la création d'une réception. Une date de traitement est indiquée sur la demande
* **Statut par défaut** : si ce paramétrage est cochée, la demande d'achat sera automatiquement à ce statut à sa création
* **Envoi d'emails à l'acheteur** : si ce paramétrage est cochée, un mail est envoyé à l'acheteur des références de la demande lorsque la demande d'achat passe à ce statut
* **Envoi d'emails au demandeur** : si ce paramétrage est cochée, un mail est envoyé au demandeur de la demande d'achat lorsque la demande d'achat passe à ce statut
* **Création automatique d'une réception** : ce paramétrage est disponible seulement pour un état de statut Traité. Si il est coché, quand la demande d'achat passe à ce statut, une réception sera créée automatiquement avec les informations renseignées sur la demande d'achat
* **Ordre\*** : ordre dans la liste des statuts sur le paramétrage

Pour qu'une demande d'achat ait un workflow cohérent, il faut au minimum un statut en état Brouillon, un en état A traiter, un en état En cours et en état Traité.&#x20;

Une fois que vous avez ajouté tous les statuts que vous souhaitez, cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>. Ils s'ajouteront dans la liste des statuts.

{% embed url="https://www.screencast.com/t/OlBWfn0lIm" %}
Ajout d'un statut
{% endembed %}

### **Modifier des statuts**

Pour modifier des statuts, cliquez sur une ligne en mode visualisation pour passer en mode modification. Vous pouvez modifier les champs de la même façon qu'à la création.

{% embed url="https://www.screencast.com/t/uHOzO6hL" %}
Modifier des statuts
{% endembed %}

### **Supprimer des statuts**

Pour supprimer des statuts, cliquez sur la poubelle de la ligne du statut que vous souhaitez supprimer, que ce soit en mode visualisation ou modification. Vous ne pouvez pas supprimer un statut s'il est utilisé sur une demande d'achat.
