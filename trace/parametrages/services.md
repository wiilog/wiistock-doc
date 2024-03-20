# Services

## Configurations

* **Enlever les heures de la date attendue** : cochez ce paramétrage pour ne pas à avoir à renseigner l'heure sur le champ Date attendue à la création d'un service

## Statuts

Pour traiter un service, il faut le faire passer par une succession de statuts. Ces statuts sont paramétrables.

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

## Champs fixes

Les champs fixes permettent de choisir quels champs sont disponibles sur le formulaire de création d'un service, de modification, et s'il est possible de filtrer sur ce champ ou non.

Pour chaque champ, choisissez les éléments suivants :&#x20;

* **Formulaire de création :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de création de service
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de créer un service sans que ce champ soit renseigné sur le formulaire de création de service
* **Formulaire d'édition :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent sur le formulaire de modification de service
  * **Obligatoire** : cochez la case pour qu'il ne soit pas possible de valider la modification d'un service sans que ce champ soit renseigné sur le formulaire de modification de service
* **Sur les filtres :**&#x20;
  * **Afficher** : cochez la case pour que le champ soit présent dans la barre de filtres de la page des services . Si la case est grisée, cela signifie que ce champ n'est pas disponible au filtrage

Certains champs fixes possèdent également un paramétrage des valeurs disponibles. C'est le cas du champ **Urgence**. Cliquez sur le libellé du champ fixe pour ouvrir une modale pour paramétrer les valeurs possibles du champ fixe.

![Paramétrage des valeurs du champ fixe](<../../.gitbook/assets/image (83).png>)

N'oubliez pas de cliquer sur **Enregistrer** pour valider votre paramétrage.

## Modèles de demande

Les modèles de demande sont utilisés dans l'application Wiilog dans le cadre des objets connectés pour le moment. Ainsi, un objet connecté peut déclencher une demande de service en se basant sur un modèle de demande paramétré

La page des modèles de demande est constituée de 2 zones :&#x20;

* une entête avec le sélection du modèle de demande et le bouton Ajouter un modèle de demande
* Le détail du modèle de demande de service

**Ajouter un modèle de demande**

Pour ajouter un modèle de demande, cliquez sur Ajouter un modèle de demande à droite de l'entête. La page passe alors en mode ajout.

Il faut alors remplir les champs suivants :&#x20;

* **Nom du modèle\*** : libellé du modèle pour l'identifier lors de l'association à un objet connecté
* **Type de service\*** : type du service lors de la création du service
* **Objet\*** : objet du service
* **Statut\*** : statut du service à la création du service par l'objet connecté
* **Date attendue\*** : **H+ " " à la création**. Renseignez un nombre derrière "H+". Ainsi, lors de la création du service par l'objet connecté, la date attendue aura comme date la date de création + le nombre d'heure renseigné ici dans le paramétrage
* **Urgence** : niveau d'urgence de la demande
* **Chargement** : champ texte informatif
* **Déchargement** : champ texte informatif
* **Nombre d'opération(s) réalisée(s)** : champ nombre informatif
* Les **champs libres** : renseignez les champs libres liés au type
* **Commentaire** : commentaire sur le service
* **Pièce-jointe** : pièce-jointe sur le service

Le caractère obligatoires des champs **Chargement**, **Déchargement**, **Nombre d'opération(s) réalisée(s)**, **Urgence**, et des **champs libres**, dépendent du paramétrage fait sur les champs fixes et les champs libres.

Cliquez sur **Enregistrer** pour ajouter le modèle.

**Modifier un modèle de demande**

Pour modifier un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez modifier, et cliquez sur le bouton Modifier dans la zone de détails d'un modèle de demande de service. La page passera alors en mode modification. Modifiez les champs comme pour la création

Cliquez sur **Enregistrer** pour valider les modifications.&#x20;

**Supprimer un modèle de demande**

Pour supprimer un modèle demande, sélectionnez dans la liste Modèle de demande le modèle que vous souhaitez supprimer, et cliquez sur le bouton poubelle dans la zone de détails d'un modèle de demande de service.&#x20;

Vous pouvez supprimer un modèle s'il n'est pas utilisé dans une association avec un objet connecté.&#x20;

## Types et champs libres

Les types permettent de venir différencier des flux différents de demande de service, qui auront chacun leur process de traitement différent.

Chaque type possède également des champs libres, qui sont des champs permettant d'amener de l'information supplémentaire propre à chaque flux.

La page des types et champs libres est constituée de 3 zones :&#x20;

* L'entête avec la liste des types et le bouton **Ajouter un type**. Chaque type est cliquable et permet d'aller voir les caractéristiques du type et ses champs libres
* Les caractéristiques du type et le bouton **Modifier**, pour modifier les caractéristiques et les champs libres
* La liste des champs libres du type

**Ajouter un type**

Pour ajouter un type, cliquez sur le bouton **Ajouter un type**, à droite de la liste des types.

Remplissez ensuite les champs des caractéristiques de cette façon :&#x20;

* **Libellé\*** : nom du type, apparaîtra partout dans l'application
* **Description** : description du type, non obligatoire
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

Une fois que vous avez rempli les caractéristiques et les champs libres du type (vous n'êtes pas obligé d'avoir des champs libres), cliquez sur **Enregistrer** pour voir le nouveau type apparaître à la suite des autres.

**Modifier un type et ses champs libres**

Pour modifier un type et ses champs libres, cliquez sur le bouton **Modifier** à droite des caractéristiques du type.

La page passe alors en mode modification. Vous pouvez modifier les caractéristiques et les champs libres de la même façon que décrit au-dessus. Le typage des champs libres ne peut pas être modifié.

**Supprimer un type et ses champs libres**

Vous pouvez supprimer un type et ses champs libres grâce aux poubelles : une à gauche des caractéristiques du type pour supprimer le type, une sur chaque ligne de champs libres pour supprimer un champ libre. Ces poubelles sont présentes en mode visualisation et mode modification.

Pour supprimer un type, le type ne doit plus avoir des champs libres et ne pas être utilisé sur les services.&#x20;
