# Fonctionnalités web

#### 👀 Aller voir notre [vidéo de présentation](../../general/videos-explicatives/nouvelles-fonctionnalites-track.md) général sur la brique track 👀

## Workflow général d'une demande de livraison

_Les statuts de la <mark style="background-color:orange;">demande</mark> sont en <mark style="background-color:orange;">orange</mark>, les statuts de <mark style="background-color:green;">l'ordre</mark> sont en <mark style="background-color:green;">vert.</mark>_

Lors de la création d'une demande livraison, **si votre demande doit être faite le jour-même**, elle passera par un premier statut «<mark style="background-color:orange;">En attente de validation</mark>».

Le responsable doit alors décider s’il la prend en charge ou s’il la délègue à un sous-traitant. Si la demande est prise en charge, le workflow sera le même que pour le cas **Livraison sur des jours futurs, sur un jour et horaire ouvré**. Si la demande est sous-traitée, le workflow sera le même que pour le cas **Livraison à faire sur un jour et/ou un horaire non ouvré**.

### Livraison sur des jours futurs, sur un jour et horaire ouvré

Lorsque vous créez une demande de livraison pour une date à J+n, sur une heure ouvrée, la demande se crée au statut «<mark style="background-color:orange;">A préparer</mark>».Cela signifie que vous avez une action à faire pour que la prise en compte de la demande puisse avancée : préparer les différents colis qui seront à livrer et imprimer les étiquettes à coller sur ces colis.

{% hint style="info" %}
Le fait qu’une demande soit au statut «A préparer» ne bloque pas sa prise en compte pour sa planification de tournée.Vous pouvez ainsi préparer les colis peu de temps avant que le livreur vienne les récupérer.
{% endhint %}

À la création de la demande, l'ordre est au statut "<mark style="background-color:green;">À affecter</mark>". À partir de ce moment vous pouvez positionner la demande sur une tournée. Une fois la demande affectée à une tournée l'ordre passe au statut "<mark style="background-color:green;">Affectée</mark>", sur la demande l'information remontra.

Il est possible de **supprimer** une demande tant que la demande n’a pas été <mark style="background-color:green;">affectée</mark> à une tournée. La demande a été affectée à une tournée si vous avez un créneau horaire derrière «Estimée à :».

Une fois que la demande est affectée à une tournée, vous ne pouvez plus la supprimer. Il vous est alors possible **d’annuler** la demande.

L’impression des étiquettes fait passer la demande au statut «<mark style="background-color:orange;">A livrer</mark>» et génère un événement dans l’historique des événements. Le responsable verra aussi de son côté (sur l'ordre) que les colis sont prêts.

#### La livraison est en cours

Une livraison passe «<mark style="background-color:orange;">En cours</mark>» lorsque le livreur en charge à charger tous les colis et à indiquer avoir démarré sa tournée. Sur l'ordre elle passe aussi au statut «<mark style="background-color:green;">En cours</mark>»

#### La livraison est terminée

La livraison se termine lorsque le livreur a déposé tous les colis destinés au patient chez celui-ci. La demande passe alors du statut «<mark style="background-color:orange;">En cours</mark>» à «<mark style="background-color:orange;">Terminée</mark>». Sur l'ordre elle passe aussi au statut «<mark style="background-color:green;">Terminée</mark>»

Vous ne verrez alors plus la dernière position du livreur et le relevé de température pour cette livraison s’arrête.

#### Livraison non livrée

Il est possible que le livreur n’arrive pas à livrer les colis. Dans ce cas, il peut indiquer ne pas avoir livré. La demande sera alors au statut «<mark style="background-color:orange;">Non livrée</mark>». L'ordre sera aussi au statut «<mark style="background-color:green;">Non livrée</mark>».

### **Livraison à faire sur un jour et/ou un horaire non ouvré**

Si vous faites une demande sur une journée ou un horaire non travaillé, la demande sera automatiquement passée en statut «<mark style="background-color:orange;">Sous-traitée</mark>». Il est toujours possible de venir imprimer les étiquettes si nécessaires via le bouton Imprimer les étiquettes. Les horaires non ouvrés sont des horaires [paramétrés](../../parametrages/global.md#heures-travaillees) dans l’application.

Pour continuer ce workflow il faut allez dans la page [Ordre / sous-traitance](ordres/sous-traitance.md)

Pour indiquer l’heure à laquelle le sous-traitant a commencé la livraison, dans\
« Statut », sélectionner « <mark style="background-color:green;">En cours</mark> » et renseignez la date et l’heure du début de la livraison.

Pour indiquer l’heure à laquelle le sous-traitant a terminé la livraison, sélectionnez le statut « <mark style="background-color:green;">Terminée</mark> » et renseignez la date et heure de fin de livraison. Si le sous-traitant n’a pas pu livrer, sélectionnez le statut « <mark style="background-color:green;">Non livrée</mark> ». Il est obligatoire de mettre un commentaire dans ce cas.

## Workflow général d'une demande de collecte

### Collecte à faire pour le jour même

Si la date à laquelle votre demande de collecte doit être faite est le jour-même, elle passera par un premier statut « <mark style="background-color:orange;">En attente de validation</mark> ».

Un email sera alors envoyé au responsable afin qu’il puisse valider la demande de collecte. La sous-traitance n’existe pas pour une demande de collecte. Elle suivra ensuite le workflow classique.

#### **Planification de la date de collecte**

Lorsque vous créez votre demande de collecte, elle est dans un premier temps au statut « <mark style="background-color:orange;">En attente de planification</mark> ». Cela signifie que un responsable doit contacter le patient pour fixer la date de la collecte avec lui.

Afin de pouvoir planifier une collecte sur une tournée, il vous faut valider la date de collecte et le créneau de passage avec le patient. Sur l'ordre la collecte est au statut « <mark style="background-color:green;">Patient à contacter</mark> »&#x20;

Une fois que cette date est validée et que le responsable d’exploitation l’a renseigné dans l'ordre de collecte, la demande passe au statut « <mark style="background-color:orange;">A collecter</mark> ». Sur la liste des demandes, la date derrière « Planifiée le : » est complétée et sur le détail de la demande, la « Date validée avec le patient » est complétée.
