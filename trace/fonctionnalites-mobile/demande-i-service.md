# Demande I Service

Pour accéder à la liste des services à traiter, allez dans **Demande** puis **Service**

### Liste des services

**Informations sur la vignette de service**

Chaque service est représenté par un vignette rectangulaire qui contient les informations suivantes :&#x20;

* **Demandeur** : placé dans l'entête de couleur, personne ayant créée la demande de service
* **Numéro** : numéro de la demande de service généré par l'application
* **Date attendue** : date et heure auxquelles la demande doit être traitée
* **Chargement** : champ fixe texte Chargement
* **Déchargement** : champ fixe texte Déchargement
* **Objet** : objet de la demande de service
* **Nombre d'opération(s) réalisée(s)** : champ fixe de type nombre pour renseigner combien d'opération ont été nécessaire pour le traitement de demande de service
* **Type** : type de la demande de service
* **Urgence** : niveau d'urgence du service. Ce champ apparaîtra seulement si un niveau d'urgence a été renseigné sur le service

**Couleur d'entête**&#x20;

Les services sont présentés de celui à faire le plus rapidement à celui le moins pressant.&#x20;

Chaque vignette a une entête colorée. Cette couleur peut varier en fonction de la date d'échéance renseignée sur l'acheminement. Cette couleur se paramètre au préalable dans [Terminal mobile > Services](../../parametrages/terminal-mobile/services.md)

Sur l'exemple montré en bas, les services dont la date attendue est une date dans le passé sont en rouges, ceux dont la date attendue est pour le jour même sont en bleu, et ceux à faire dans le futur sont en vert clair.&#x20;

Les services n'ayant pas de date attendue auront une entête couleur vert sapin.

![](<../../.gitbook/assets/service (1).jpg>)

**Filtre sur l'objet**

Si vous avez un QR Code ou un code barre avec l'objet du service, vous pouvez le flasher, ou le scanner en appuyant sur l'appareil photo, pour arriver directement sur le détail du service pour le traiter.

### Indiquer qu'un service est en cours

Accédez au détail du service pour modifier le statut en appuyant sur la vignette du service souhaité. Vous pouvez aussi y accéder via scan du numéro de l'objet du service comme expliquer ci-dessus ou bien en appuyant sur la notification de nouveau service si vous avez paramétré les notifications (notifications à paramétrer sur le paramétrage du type du service).

**Détails du service**

Appuyez sur les ![](../../.gitbook/assets/fleche.PNG)pour visualiser tous les champs fixes du service.

En dessous vous avez ensuite les champs _**Statut**_, _**Commentaire**_, et _**Photo(s)**_ qui sont des champs modifiables. Si vous avez paramétré des champs libres, ils seront disposés sous ces champs et seront modifiables également si vous les avez mis visibles à la modification. Si vous avez déjà renseigné une valeur lors de la création de la demande, le champ libre sera déjà rempli avec la valeur renseignée du champ libre.&#x20;

**Modifier le statut**

Pour modifier le statut du service, appuyez sur la loupe dans le champ _**Statut**_.&#x20;

Il vous serez alors proposé une liste de statut en état _En cours_ ou _Traité_.

Sélectionnez un statut en état _En cours,_ renseignez les autres champs si besoin_,_ et appuyez sur <mark style="background-color:blue;">**VALIDER**</mark>. Le service sera toujours disponible sur la liste des services sur le nomade.

> Selon le paramétrage du statut (voir [Paramétrages > Trace >  Services > Statuts](../../parametrages/trace/services/statuts.md) ) , il est possible qu'il soit obligatoire de saisir un commentaire pour valider le changement de statut et d'informations du service.&#x20;

Sur la supervision, vous verrez le changement de statut sur le détail du service.&#x20;

### Traiter un service

Pour traiter un service, le fonctionnement est le même que pour passer un service en statut _En cours_.&#x20;

Appuyez sur la loupe pour accéder aux statuts en état _En cours_ ou _Traité_, et sélectionnez cette fois-ci un statut en état _Traité_. Vous pouvez également renseigner les différents champs à l'écran avant de valider.&#x20;

Idem que précédemment, il est possible qu'il soit obligatoire de mettre un commentaire pour valider le passage en traité selon le paramétrage du statut.&#x20;

Le service sera considéré comme terminé et n'apparaîtra plus dans la liste des services sur le nomade.&#x20;

