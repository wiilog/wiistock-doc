# Statuts

Pour traiter un acheminement, il faut le faire passer par une succession de statuts. Ces statuts sont paramétrables par type d'acheminement.

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
