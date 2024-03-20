# Suivre le traitement d’une demande de livraison

## Livraison à faire pour le jour même

Si votre demande doit être faite le jour-même, elle passera par un premier statut « En attente de validation ».

Un responsable doit alors décider s’il la prend en charge ou s’il la délègue à un sous-traitant.

Si la demande est prise en charge, le workflow sera le même que pour le cas Livraison sur des jours futurs, sur un jour et horaire ouvré.

Si la demande est sous-traitée, le workflow sera le même que pour le cas Livraison à faire sur un jour et/ou un horaire non ouvré.

Vous pouvez imprimer des étiquettes même si la demande est « En attente de validation » (voir plus bas.

## Livraison à faire sur un jour et/ou un horaire non ouvré

Si vous faites une demande sur une journée ou un horaire non travaillé, la demande sera automatiquement passée en statut « Sous-traitée ».

Vous n’avez pas d’actions à effectuer dans ce cas. Il est néanmoins toujours possible de venir imprimer les étiquettes si nécessaires via le bouton Imprimer les étiquettes (voir plus bas pour l’explication plus poussée de la fonctionnalité).

Les horaires non ouvrés sont des horaires [paramétrés](../../../parametrages/global.md#heures-travaillees) dans l’application.

Lorsqu’une demande est sous-traitée, le responsable vient renseigner directement à la main la date et l’horaire du démarrage de livraison, ainsi que la date et l’horaire du traitement de la livraison, ou de la non-livraison si le sous-traitant a rencontré un souci. Il peut également venir ajouter des documents tel que le relevé des températures pour la livraison. Tout sera mis à disposition sur le détail de votre demande dans l’historique des transports.

<figure><img src="../../../.gitbook/assets/demande-sous-traité.png" alt=""><figcaption><p>Demande sous-traité</p></figcaption></figure>

Dans l’exemple ci-dessus, la demande a été directement sous-traitée et le responsable a renseigné les différents éléments du traitement :

1. La demande a été créé le lundi 06 juin à 12h45. Elle est à faire pour 22h et est donc directement passée au statut Sous-traitée sur l’historique des statuts. Dans l’historique de transport, on retrouve le message que vous avez à la validation de la création de la demande de livraison, ainsi que l’événement de création.
2. Il a été indiqué que le traitement de la demande a démarré à 19h10. On retrouve dans l’historique des transports l’événement qui a amené à cette indication de statut. On voit que c’est le lendemain qu’il a été indiqué que la demande était en cours à 19h10.
3. Il a été indiqué que le traitement de la demande a été effectué à 21h50. Idem pour le passage en statut En cours, on retrouve l’information de quand a été indiqué cet horaire dans l’historique du transport.
4. Le suivi des températures a été ajouté sous format PDF. Vous pouvez le télécharger en cliquant sur le nom de la pièce-jointe.
5. Comme la demande est sous-traitée, il n’y a pas de suivi de position GPS ou de température en direct.

## Livraison sur des jours futurs, sur un jour et horaire ouvré

### Livraison A préparer – Impression des étiquettes

Lorsque vous créez une demande de livraison pour une date à J+n, sur une heure ouvrée, la demande se crée au statut « A préparer ».

Cela signifie que vous avez une action à faire pour que la prise en compte de la demande puisse avancée : préparer les différents colis qui seront à livrer et imprimer les étiquettes à coller sur ces colis.

Le fait qu’une demande soit au statut « A préparer » ne bloque pas sa prise en compte pour la planification de tournée. Vous pouvez ainsi préparer les colis peu de temps avant que le livreur vienne les récupérer.

Pour imprimer les étiquettes, 2 accès :

* A partir de la liste des demandes de transport (Demande | Transport) : sur la demande de livraison pour laquelle vous souhaitez imprimer les étiquettes, cliquez sur les<img src="../../../.gitbook/assets/3-points.png" alt="" data-size="line">et sur <mark style="background-color:blue;">**Imprimer les étiquettes**</mark>
*   A partir du détail de la demande de transport (Demande | Transport | Détails) : dans la partie colis, cliquez sur <mark style="background-color:blue;">**Imprimer les étiquettes**</mark>

    Au clic sur le bouton, une modale de colisage va s’ouvrir. Vous devez alors renseigner le nombre de colis pour chaque nature indiquée à la création de la livraison. Cliquez ensuite sur <mark style="background-color:blue;">**Imprimer**</mark>. Les étiquettes vont alors se générer et se télécharger sous la forme d’un fichier PDF. Vous pouvez réimprimer les étiquettes en cliquant à nouveau sur le bouton.

{% embed url="https://www.screencast.com/t/wQgVs19B" %}
Impression d'étiquette depuis le détail d'une demande
{% endembed %}

{% hint style="info" %}
Si vous avez besoin d’ajouter une nature de colis, modifier la demande&#x20;
{% endhint %}

Une étiquette est constituée de :

{% embed url="https://www.screencast.com/t/xk73Bpeu" %}
Exemple d'étiquette
{% endembed %}

1. A gauche, le QR Code et le numéro de colis. Le numéro de colis est constitué d’un préfixe (CH pour les colis de chimiothérapie, M pour ceux de médicaments & DMS), du numéro de la demande, et d’un compteur (001)
2. Le nom du patient et son numéro de dossier
3. Le l’adresse du patient
4. La température de conservation du colis s’il y en a une
5. Le numéro du colis sur le nombre total de colis dans la livraison

L’impression des étiquettes fait passer la demande au statut « A livrer » et génère un événement dans l’historique des événements.

A partir de cette étape, vous n’avez plus d’actions à effectuer sur la demande.

### Estimation de l’horaire de passage

Dès que le responsable voit votre nouvelle demande de livraison, il l’a planifie sur une tournée afin d’avoir une estimation de l’heure de passage chez le patient.

C’est donc lorsque que votre demande est planifiée sur une tournée que vous avez une estimation de l’heure de passage. Vous retrouvez cette estimation dans la liste des demandes derrière le libellé « Estimée à : » et sur le détail d’une demande au niveau du statut « Terminée ».

Si la tournée n’a pas commencé, vous aurez seulement une notion de Matin ou Après-midi pour l’estimation. Dès que le livreur aura commencé sa tournée, vous obtiendrez l’heure précise estimée de l’horaire de passage.

### Livraison en cours

Une livraison passe « En cours » lorsque le livreur en charge à charger tous les colis et à indiquer avoir démarré sa tournée.

La demande passe alors au statut « En cours », et vous pouvez visualiser la dernière position GPS du livreur ainsi que le suivi des températures.

#### **Cas des colis écartés**

Il se peut qu’au chargement, le livreur écarte un colis car celui-ci est abîmé ou manquant. Il ne fera donc pas parti des colis qui seront livrés au patient.

Pour savoir qu’un colis a été écarté, vous aurez l’indication à 3 endroits :

* Sur la liste des demandes de transport (Demande | Transport) : un logo <img src="../../../.gitbook/assets/colis-écarté.png" alt="" data-size="line">apparaîtra en haut à droite de la vignette pour indiquer que la demande contient un colis écarté**.**
* Sur le détail d’une demande (Demande | Transport | Détails) : dans la section colis le même logo apparaîtra + sur la ligne du colis écarté, il sera marqué « oui » dans la colonne « Ecarté » ainsi que la raison de son écartement dans la colonne « Motif écartement ». Les colis non écartés auront « non » dans la colonne « Ecarté ». (motifs [paramétrable](../../parametrages/tournees.md#colis-ecartes))

{% embed url="https://www.screencast.com/t/CWjuWtw393" %}
Colis écatrés
{% endembed %}

### Livraison terminée

La livraison se termine lorsque le livreur a déposé tous les colis destinés au patient chez celui-ci. La demande passe alors du statut « En cours » à « Terminée ». Vous ne verrez alors plus la dernière position du livreur et le relevé de température pour cette livraison s’arrête.

Le livreur a la possibilité d’ajouter un commentaire, une photo et/ou une signature lors du traitement de la demande. Vous les verrez dans l’historique de transport de la demande. Vous pouvez télécharger la photo ou la signature en cliquant sur le lien du fichier sous la photo ou la signature.

#### Livraison non livrée

Il est possible que le livreur n’arrive pas à livrer les colis destinés au patient. Dans ce cas, il peut indiquer ne pas avoir livré. La demande sera alors au statut « Non livrée » et non pas «Terminée».

Vous serez averti de cette non-livraison via une notification web qui apparaitra en haut à droite.

Si vous l’avez manqué, vous verrez un petit 1 rouge sur la cloche de l’entête. Cliquez sur la cloche pour accéder à la liste des notifications. Vous pouvez cliquer sur la source pour être redirigé vers la livraison non livrée.

Vous retrouvez la raison de non-livraison dans l’historique des transports : le livreur est obligé d’indiqué la raison de la non-livraison.

Dans la partie Colis, une nouvelle colonne « Retourné le » apparaît : le livreur est obligé de retourner les colis non livrés. Lorsqu’il les aura retournés, l’horodatage de dépose sera indiqué dans cette colonne.

{% embed url="https://www.screencast.com/t/kl7ZTWPzzmtI" %}
Détails d'une livraison non livrée
{% endembed %}

#### Livraison rejetée

Il peut arriver également qu’une livraison soit rejetée, c’est-à-dire qu’elle ne soit pas du tout prise en compte dans la tournée initiale sur laquelle elle a été prévue.

Une livraison peut être rejetée pour 2 raisons :

* Tous les colis de la demande ont été écartés, aucun ne peut être livré en l’état. Dans ce cas, le statut de la demande qui était à « A livrer » passe à « A préparer » et il vous faut ré imprimer des étiquettes pour qu’elle soit planifier ensuite sur une autre tournée
* La livraison n’était pas préparée : aucun colis n’était disponible pour cette livraison. La demande reste alors au statut « A préparer » et elle sera planifiée sur une autre tournée dans la journée

{% embed url="https://www.screencast.com/t/afKCy43sKj" %}

