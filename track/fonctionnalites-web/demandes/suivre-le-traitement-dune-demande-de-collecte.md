# Suivre le traitement d’une demande de collecte

## Collecte à faire pour le jour même

Si la date à laquelle votre demande de collecte doit être faite est le jour-même, elle passera par un premier statut « En attente de validation ».

Un email sera alors envoyé au responsable d’exploitation afin qu’il puisse valider la demande de collecte dans Ordre / Sous-traitance. La sous-traitance n’existe pas pour une demande de collecte.

Elle suivra ensuite le workflow classique.

## Collecte à faire pour des jours futurs

### Planification de la date de collecte avec le patient

Lorsque vous créez votre demande de collecte, elle est dans un premier temps au statut « En attente de planification ». Cela signifie que le responsable doit contacter le patient pour fixer la date de la collecte avec lui.

Une fois que cette date est validée et que le responsable d’exploitation l’a renseigné dans l'ordre de collecte, la demande passe au statut « A collecter ». Sur la liste des demandes, la date derrière « Planifiée le : » est complétée et sur le détail de la demande, la « Date validée avec le patient » est complétée.

### Estimation de l’horaire de passage

Comme sur les livraisons, dès que le responsable voit votre nouvelle demande de collecte et qu’il a contacté le patient, il l’a planifie sur une tournée afin d’avoir une estimation de l’heure de passage chez le patient.&#x20;

C’est donc lorsque que votre demande est planifiée sur une tournée que vous avez une estimation de l’heure de passage.Vous retrouvez cette estimation dans la liste des demandes derrière le libellé « Estimée à : » et sur le détail d’une demande au niveau du statut « Terminée ».\
Si la tournée n’a pas commencé, vous aurez seulement une notion de Matin ou Après-midi pour l’estimation. Dès que le livreur aura commencé sa tournée, vous obtiendrez l’heure précise estimée de l’horaire de passage.

### Collecte en cours

Une collecte passe « En cours » dès que le livreur a indiqué avoir commencé sa tournée. La demande passe alors au statut « En cours », et vous pouvez visualiser la dernière position GPS du livreur.

### Collecte Terminée

La collecte se termine lorsque le livreur a collecté tous les objets chez le patient. La demande passe alors au statut « Terminée ». Vous ne verrez alors plus la dernière position du livreur.

Le livreur a la possibilité d’ajouter un commentaire, une photo et/ou une signature lors du traitement de la demande. Vous les verrez dans l’historique de transport de la demande. Vous pouvez télécharger la photo ou la signature en cliquant sur le lien du fichier sous la photo ou la signature.

#### Objets collectés déposés

La collecte a un dernier statut après le statut « Terminée » contrairement à la livraison. Il s’agit du statut « Objets déposés ». Cela signifie que le livreur a bien indiqué avoir retourné les objets collectés.

{% embed url="https://www.screencast.com/t/DUqJT6B4" %}
Détail d'une collecte
{% endembed %}

#### Collecte non collectée

Il est possible que le livreur n’arrive pas à collecter les objets demandés. Dans ce cas, il peut indiquer ne pas avoir collecté. Vous retrouvez la raison de non-collecte dans l’historique des transports : le livreur est obligé d’indiqué la raison de la non-collecte.

En fonction du motif que le livreur a renseigné, la collecte peut avoir 2 comportements possibles :

* Le motif implique de devoir repasser chez le patient : la demande repart dans le workflow. Elle passe directement du statut « Non collectée » à « En attente de planification ». Vous n’avez pas besoin de refaire la demande. le responsable recontactera le patient pour replanifier la demande sur une tournée
* Le motif implique de ne pas repasser chez le patient : la demande s’arrête au statut « Non collectée » et est définitivement terminée.

{% embed url="https://www.screencast.com/t/JAdBIgWL" %}
Détail demande de collecte non collecté à reprogrammer
{% endembed %}
