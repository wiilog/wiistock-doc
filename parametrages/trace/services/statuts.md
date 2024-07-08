# Statuts

Pour traiter un service, il faut le faire passer par une succession de statuts. Ces statuts sont paramétrables.

<figure><img src="../../../.gitbook/assets/image (128).png" alt=""><figcaption><p>Paramétrage | Trace | Services | Statuts</p></figcaption></figure>

Lorsque vous arrivez sur la partie Statuts, vous avez 2 partie :&#x20;

* une section en haut avec les types des services (vous ne pouvez pas paramétrer les statuts si vous n'avez pas paramétré les types). Cliquez sur un type pour filtrer les statuts par rapport au type
* une section avec la liste des statuts. La liste des statuts est tous types confondus si vous n'avez pas cliquez sur un type. Vous pouvez faire une recherche rapide sur la liste si elle contient plus de 10 lignes. Les colonnes du tableau sont triables.&#x20;

**Ajouter des statuts**

Pour ajouter des statuts, cliquez sur le bouton **Ajouter des statuts**. La page va alors passer en mode ajout. Si vous souhaitez ajouter plusieurs statuts à la fois, appuyez sur le + en bas de la première ligne. Remplissez le tableau de cette façon :&#x20;

* **Libellé\*** : nom du statut qui apparaîtra dans l'application
* **Etat\*** : état du statut. L'état d'un statut conditionne les actions que l'on peut faire sur un service. 3 états sont disponibles :&#x20;
  * _**A traiter**_ : la demande est crée. Elle apparait sur le nomade (si Synchronisation nomade est cochée, voir plus loin). La date de la demande est renseignée au premier passage à un statut à cet état
  * _**En cours**_ : pour indiquer que le service a été pris en compte et est en cours de traitement. Un service avec un statut en cours apparait sur le nomade.
  * _**Traité**_ : le service est terminé. Il n'apparaît plus sur le nomade. Une date de réalisation lui est affectée avec la personne l'ayant traité
* **Type\*** : type du service. Les statuts dépendent du type, ce qui permet d'avoir des workflow différents en fonction du type du service
* **Statut par défaut** : si ce paramétrage est cochée, le service sera automatiquement à ce statut à sa création
* **Envoi d'emails au demandeur** : si ce paramétrage est cochée, un mail est envoyé au demandeur (personne ayant créée la demande) lorsque le service passe à ce statut
* **Envoi d'emails aux destinataires** : si ce paramétrage est cochée, un mail est envoyé aux destinataires du services (destinataires renseignés sur le service au moment de sa création) lorsque le service passe à ce statut
* **Synchronisation nomade** : si ce paramétrage est coché, un service qui est à ce statut sera visible sur le nomade. Ce paramétrage n'est disponible que pour les statuts en état A traiter ou En cours
* **Ordre\*** : ordre dans la liste des statuts sur le paramétrage

Pour qu'un service ait un workflow cohérent, il faut au minimum un statut en état A traiter, et un Traité. Si vous voulez indiquer que l'opérateur a commencé à traiter un service, paramétrer au moins un statut en état En cours.&#x20;

Une fois que vous avez ajouté tous les statuts que vous souhaitez, cliquez sur **Enregistrer**. Ils s'ajouteront dans la liste des statuts.

**Modifier des statuts**

Pour modifier des statuts, cliquez sur une ligne en mode visualisation pour passer en mode modification. Vous pouvez modifier les champs de la même façon qu'à la création, sauf le type qui ne peut plus être modifié.&#x20;

**Supprimer des statuts**

Pour supprimer des statuts, cliquez sur la poubelle de la ligne du statut que vous souhaitez supprimer, que ce soit en mode visualisation ou modification. Vous ne pouvez pas supprimer un statut s'il est utilisé sur un service.
