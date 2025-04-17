# Notifications push

Les notifications push se déclenchent sur le terminal mobile. Un texte de base vous est proposé, vous pouvez le modifier. En fonction de la demande, des variables vous sont proposées pour avoir les informations contextuelles de la demande qui a déclenché la notification.

### Paramétrer les notifications sur la supervision

### 1. Activer les notifications sur les types

Vous pouvez décider d'activer les notifications en fonction des types. Ainsi certains types acheminements déclencheront des notifications alors que les autres types non. \
Les notifications sont disponibles pour les types :

* Livraisons&#x20;
* Collectes
* Transferts
* Services
* Acheminements

**Pour les types de livraison, collecte et transfert** choisissez le type dont vous souhaitez activer les notifications, cliquer sur le bouton "**Modifier**" et activez la coche "**Notifications Push**".

{% hint style="info" %}
Activer les notifications sur les livraisons, les collectes, et les transferts revient à les activer pour la demande et ensuite l'ordre qui en découle.
{% endhint %}

**Pour les types d'acheminements et de services**, vous avez en plus la possibilité d'activer les notifications seulement si une demande identifiée comme urgente est validée. \
Vous avez le choix entre ces 3 possibilités :

1. **Désactiver :** Aucune notification
2. **Activer** : Les demandes urgentes et non urgentes déclencheront des notifications.
3. **Activer seulement si urgence** : Seulement les demandes urgentes déclencheront des notifications. Choisissez la ou les valeur(s) d'urgence(s) qui déclencheront les urgences.

### 2. Activer les doits et vérifier votre utilisateur

Pour que les notifications fonctionnent, il faut activer le droit sur le rôle des personnes qui auront besoin des notifications sur le terminal mobile. Dans le paramétrage allez dans Rôles (sous menu d'utilisateurs), sélectionner le menu nomade et activer le droit "**Activer les notifications**".

_Img_

Vérifiez aussi que les types de demande auxquels vous avez ajouté les notifications sont paramétrés pour l'utilisateur qui utilise le terminal mobile. Pour cela, allez dans Utilisateurs (sous menu d'utilisateurs), sélectionner un utilisateur et ajouter dans les champs **Type de livraison**, **Type d'acheminement** et **Types de service** les types souhaités.

_Img_

{% hint style="info" %}
Pour que le paramétrage de la supervision se répercue sur le nomade, il faut déconnecter et reconnecter l'utilisateur pour que les modifications soit bien prise en compte.
{% endhint %}

### 3. Paramétrer le texte de la notification

Pour accéder et modifier le texte, allez dans le **menu Notifications push** (sous-menu de modèle de notification). Un texte de base vous est proposé pour chaque type de demande/ordre, cliquez sur la ligne pour le modifier.

En fonction de la demande ou de l'ordre sélectionné, des variables vous sont proposées. Ces variables vous permettent d'avoir des informations contextuelles sur la demande qui a déclenché la notification. Une zone d'exemple vous permet d'avoir une idée de ce à quoi va ressembler votre notification sur le nomade. Attention, l'affichage de la notification dépend néanmoins du matériel et peut donc varier par rapport à ce que vous voyez.

#### Les variables

{% tabs %}
{% tab title="Ordre de préparation" %}
_@numordrepreparation_ : Numéro de l'ordre \
&#xNAN;_@typelivraison_ : Type de la livraison \
&#xNAN;_@destination_ : Destination de la livraison \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la livraison \
&#xNAN;_@datevalidation_ : Date de validation de la demande de livraison
{% endtab %}

{% tab title="Ordre de livraison" %}
_@numordrelivraison_ : Numéro de l'ordre \
&#xNAN;_@typelivraison_ : Type de la livraison \
&#xNAN;_@destination_ : Destination de la livraison \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la livraison \
&#xNAN;_@datevalidation_ : Date de validation de la demande de livraison
{% endtab %}

{% tab title="Ordre de collecte" %}
_@numordrecollecte_ : Numéro de l'ordre de collecte \
&#xNAN;_@typecollecte_ : Type de la collecte \
&#xNAN;_@destination_ : Mise en stock ou destruction \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la collecte \
&#xNAN;_@pointdecollecte_ : Emplacement où collecter les références demandées \
&#xNAN;_@objet_ : Objet de la collecte \
&#xNAN;_@datevalidation_ : Date de validation de la demande de collecte
{% endtab %}

{% tab title="Ordre de transfert" %}
_@numordretransfert_ : Numéro de l'ordre de transfert \
&#xNAN;_@origine_ : Origine du transfert \
&#xNAN;_@destination_ : Destination du transfert \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la demande \
&#xNAN;_@datevalidation_ : Date de validation de la demande de transfert
{% endtab %}

{% tab title="Demande d'acheminement" %}
_@numacheminement_ : Numéro de l'acheminement \
&#xNAN;_@typeacheminement_ : Type de l'acheminement \
&#xNAN;_@statut_ : Statut de la demande d'acheminement \
&#xNAN;_@empprise_ : Emplacement prise \
&#xNAN;_@empdepose_ : Emplacement dépose \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la demande d'acheminement \
&#xNAN;_@datevalidation_ : Date de validation de la demande d'acheminement \
&#xNAN;_@dateecheance_ : Date d'échéance de la demande d'acheminement \
&#xNAN;_@numcommande_ : Numéro de commande de la demande d'acheminement \
&#xNAN;_@nbcolis_ : Nombre de colis (lignes) dans la demande d'acheminement
{% endtab %}

{% tab title="Demande de service" %}
_@numservice_ : Numéro de la demande de service \
&#xNAN;_@typeservice_ : Type de service \
&#xNAN;_@statut_ : Statut de la demande de service \
&#xNAN;_@chargeme&#x6E;_&#x74; : Endroit de chargement \
&#xNAN;_@dechargement_ : Endroit de déchargement \
&#xNAN;_@demandeur_ : Utilisateur ayant créé la demande de service \
&#xNAN;_@datecreation_ : Date de création de la demande de service \
&#xNAN;_@dateattendue_ : Date attendue de la demande de service \
&#xNAN;_@objet_ : Objet de la demande de service \
&#xNAN;_@nboperations_ : Nombre d'opérations à réaliser
{% endtab %}
{% endtabs %}

### 4. Les notifications sur le terminal mobile&#x20;

Quand une demande est validée (passage d'un état "Brouillon" à "à traiter"), une notification se déclenchera alors si les différents paramétrages vus précédemment se mettent en place. &#x20;

Quand vous appuyez sur la notification, vous êtes alors redirigez vers la demande en question.

Les notifications de demande urgente possèdent une indication visuelle en plus.

_capture nomade notification_
