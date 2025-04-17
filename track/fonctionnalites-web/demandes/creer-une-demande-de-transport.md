# Créer une demande de transport

Pour créer une demande de transport (livraison ou collecte), cliquez sur le <mark style="background-color:blue;">**+**</mark> dans l’entête et sélectionnez <mark style="background-color:blue;">**Transport.**</mark>

## Demande de livraison

Le formulaire est distingué en 5 parties (les champs obligatoires sont indiqués par un astérisque\*). Livraison est sélectionné par défaut :

**Les informations Patient** : Renseignez l'identité du patient, sont numéro de dossier, son adresse, le contact, personne à prévenir puis la remarque.

**Service** : choix du type de livraison (selon ce que vous avez renseigné dans votre [paramétrage](../../parametrage/demandes/livraison-types-and-champs-libres.md)). Cliquez sur le service souhaité afin de faire apparaître les natures de colis possibles à la livraison pour ce service.

**Date** : choix de quand la livraison doit être effectuée ainsi que de son niveau d’urgence. Rentrez la date à laquelle la livraison doit être effectuée ainsi que l’heure. Si la livraison est urgente, sélectionnez le niveau d’urgence dans la liste déroulante « Urgence »

**Colis** : choisissez les différents éléments qui seront à livrer. En fonction des natures que vous cochez, une liste déroulante peut apparaître afin de sélectionner la température de conservation du colis.

* &#x20;Si vos colis sont déjà préparés, cochez « Imprimer les étiquettes » pour être redirigé vers la modale de colisage pour indiquer le nombre de colis de chaque nature et avoir les étiquettes correspondantes.
* Si vos colis ne sont pas préparés, ne cochez pas « Imprimer les étiquettes ». Vous pourrez indiquer le nombre de colis par nature et imprimer les étiquettes plus tard

**Autres informations** : informations complémentaires sur la livraison. Complétez les champs. Ils ne sont pas tous obligatoires. (selon ce que vous avez renseigné dans votre [paramétrage](../../parametrage/demandes/livraison-types-and-champs-libres.md)).

{% embed url="https://www.screencast.com/t/YkkFma9GX" %}
Demande de livraison
{% endembed %}

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider la création de votre demande de transport.

En fonction de la date que vous avez renseigné dans "Date et heure de livraison", vous pouvez voir apparaître différents messages au moment de l’enregistrement :&#x20;

* Votre **demande est à faire pour le jour même** : un message comme quoi votre demande est en attente de validation apparaîtra. Le responsable d’exploitation recevra un mail pour aller valider la livraison, ou la passer en sous-traitance si besoin.
* Votre **demande est à faire sur un horaire non ouvré** : un message apparaîtra vous informant que la demande ne dispose pas de suivi en temps réel car elle est sur un horaire non ouvré. Vous pouvez également faire une demande de livraison dans le passé si vous êtes directement passé par le sous-traitant et que vous souhaitez garder un suivi dans Wiilog. La procédure sera la même que pour une demande sur un horaire non ouvré.

## Demande de collecte

Le formulaire, comme celui de livraison, est distingué en 5 parties (les champs obligatoires sont indiqués par un astérisque \*). Sélectionnez <mark style="background-color:blue;">**Collecte**</mark> en haut :

**Les informations Patient** : Renseignez l'identité du patient, sont numéro de dossier, son adresse, le contact, personne à prévenir puis la remarque.

**Service** : choix du type de collecte (selon ce que vous avez renseigné dans votre [paramétrage](../../parametrage/demandes/collectes-types-et-champs-libres.md)). Cliquez sur le service souhaité afin de faire apparaître les natures de colis possibles à la collecte pour ce service.

**Date** : choix de quand la collecte doit être effectuée. Cette date est purement indicative. Elle devra être validée ensuite avec le patient. Il n’y a pas d’heure à indiquer contrairement aux livraisons, ou de niveau d’urgence. Vous ne pouvez pas sélectionner une date dans le passé.

**Colis** : choisissez les différents éléments qui seront à collecter.\
Lorsque vous cochez une nature de colis à collecter, un compteur apparaît. Si vous connaissez le nombre d’éléments à récupérer de la nature, vous pouvez donner l’indication au livreur. Si vous ne connaissez pas la quantité à collecter, laissez le champ vide

**Autres informations** : informations complémentaires sur la collecte. Complétez les champs. Ils ne sont pas tous obligatoires. (selon ce que vous avez renseigné dans votre [paramétrage](../../parametrage/demandes/collectes-types-et-champs-libres.md)).

{% embed url="https://www.screencast.com/t/aNY5WuQx1" %}
Demande de collecte
{% endembed %}

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider la création de votre demande de transport.

A la validation de votre demande de collecte vous pouvez voir apparaître 2 types de message :

* Vous avez indiqué une **date de collecte égale à la journée en cours** : un message apparaît comme quoi votre demande est en attente de validation. Le message est le même que pour une livraison. Le responsable d’exploitation recevra un mail pour aller valider la collecte.
* Il existe déjà une **demande de collecte non terminée pour ce patient** : un message comme quoi une demande de collecte pour ce patient existe déjà apparaîtra alors. Vous avez alors la possibilité d’annuler votre demande ou alors de confirmer la création de cette demande. L’application se base sur le numéro de dossier pour vérifier si une demande de collecte existe déjà pour un patient.

## Demande de livraison et collecte à faire en même temps

Vous avez la possibilité de créer une demande de livraison/collecte, c’est-à-dire de demander au livreur de réaliser une livraison et d’indiquer qu’il y a des objets à collecter chez le patient en réalisant la livraison.

Pour cela, commencez par créer une demande de livraison. Dans la partie « Service », cliquez sur « Fai<mark style="background-color:blue;">**re une collecte en même temps que la livraison**</mark> ».

Remplissez les différentes informations de la livraison, et cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>.

Vous serez alors redirigé vers le formulaire de création d’une demande de collecte. Les informations Patient ainsi que la date de collecte seront les mêmes que pour la livraison, sans possibilité de modification. Si vous vous êtes trompés dans les informations, vous devez refaire la demande.

Remplissez les informations propres à la collecte, et cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour créer la livraison/collecte.

{% hint style="info" %}
Une fois que vous avez créé les demandes de transport, vous pouvez les voir dans la page Demande | Transport.
{% endhint %}
