---
description: Livraison et collecte planifié sur un jour et/ou un horaire non ouvré
---

# Sous-traitance

Si le demandeur crée une demande (livraison ou collecte) à traiter dans la journée sur vos horaires ouvrés, ou sur un horaire non ouvré ou une journée non travaillée, la demande arrive directement dans Ordre | Sous-traitance.

La page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Les **vignettes de sous-traitance**

{% embed url="https://www.screencast.com/t/SwOvAPdsgL" %}
Page ordre Sous traitance
{% endembed %}

### **Contenue filtre**

* **Date Du-Au** : filtre de date. Par défaut la date du jour est sélectionné dans le filtre "Du". La tranche basse filtrant sur la date de demande renseigné lors de la création.
* **Demandeurs** : Personne ayant crée la demande
* **Numéros de dossier** : Numéro de dossier du patient à livrer
* **Patient** : Nom et prénom du patient à livrer
* **Statut** : Statut des demandes de sous-traitance&#x20;
* **Type** : Le type de la demande de livraison&#x20;

## Valider la demande

En haut de la page, toutes les demandes à valider se placent dans la zone « A valider ».

{% embed url="https://www.screencast.com/t/26ylYCWMd" %}
Vignette de demande à accepter ou sous-traiter
{% endembed %}

#### Chaque vignette contient les informations suivantes :

1. **Numéro de la demande** de transport
2. **Date et heure de création** de la demande de transport
3.  **Heure de livraison** souhaitée pour la demande. Dans le cas d’une collecte,

    le **jour de collecte** souhaité est indiqué
4. **Type** de la demande
5. **Patient**
6. **Numéro de dossier** du patient
7. **Adresse** du patient
8. Si vous pouvez **prendre en compte cette demande**, cliquez sur ce bouton <mark style="background-color:blue;">**Accepter**</mark> la demande. L’ordre sera alors créé dans Ordre | Transport et vous devez ensuite la traiter par le workflow classique
9. Si la demande **ne peut pas être prise en compte** par un de vos livreurs, cliquez sur <mark style="background-color:blue;">**Sous-traiter**</mark> pour la confier à un sous-traitant. La demande passe alors en dessous, sous la date à laquelle il faut faire la demande. \
   _Pour une collecte, ce bouton n’est pas disponible. Vous pouvez seulement Accepter une demande de collecte._

## Demande sous traitée

{% embed url="https://www.screencast.com/t/ivy3OXtw" %}
Vignette demande de livraison sous-traitée
{% endembed %}

Une fois que vous avez sous-traité la demande elle se retrouve dans la lite des demandes en dessous de "À valider". Vous retrouver les même info que sur la vignette dans "à valider", avec 5 information en plus :&#x20;

* **Commencée le** : Date et heure à laquelle le livreur a commencé à la traiter
* **Livrée le** : Date et heure à laquelle le livreur à fini de la traiter
* **Sous-traitant** : nom du sous-traitant
* **Immatriculation** : immatriculation du camion
* **Sous-traité** : Statut de la demande, il y a 4 statuts disponibles :&#x20;
  * Sous traitée : statut par défaut après avoir indiqué que la demande est sous traité
  * En cours : le sous-traitant a commencé la livraison
  * Terminé : le sous-traitant a terminé la livraison
  * Non livrée : le sous-traitant n'a pas pu effectuer la livraison

Vous pouvez ensuite renseigner à la main les informations de traitement de la demande par votre sous-traitant. Pour cela, cliquez sur la vignette ou sur ![](../../../.gitbook/assets/3-points.png)et <mark style="background-color:blue;">**Modifier**</mark>.

Une modale s’ouvre, vous pouvez renseigner dans un premier temps le nom du sous-traitant et son immatriculation.

Pour indiquer l’heure à laquelle le sous-traitant a commencé la livraison, dans\
« Statut », sélectionner « En cours » et renseignez la date et l’heure du début de la livraison.

Pour indiquer l’heure à laquelle le sous-traitant a terminé la livraison, sélectionnez le statut « Terminée » et renseignez la date et heure de fin de livraison. Vous pouvez directement indiquer la date et heure de début de livraison et de fin de livraison en même temps sans passer par la sélection du statut « En cours ».

Si le sous-traitant n’a pas pu livrer, sélectionnez le statut « Non livrée ». Il est obligatoire de mettre un commentaire dans ce cas.

Vous pouvez également ajouter une pièce-jointe sur la livraison, tel que le relevé des températures. Tous ces éléments seront visibles sur la demande.

{% embed url="https://www.screencast.com/t/WDXKD6d50Nr" %}
Formulaire pour indiquer les informations de traitement d'une demande sous-traitée
{% endembed %}

Une fois la demande terminée les informations renseignées sur la modale s'ajoute sur la vignette, le statut change. Si vous avez ajouté une pièce jointe, elle se retrouve sous forme de lien en dessous du statut, vous pouvez cliquer dessus pour la télécharger.

{% embed url="https://www.screencast.com/t/suZOzgnPp" %}
Détails d'une vignette de demande sous-traitée
{% endembed %}

{% hint style="info" %}
Vous pouvez retrouver le déroulé d'une demande [ici](../demandes/suivre-le-traitement-dune-demande-de-livraison.md#livraison-a-faire-sur-un-jour-et-ou-un-horaire-non-ouvre)
{% endhint %}
