# Traiter un demande

## Traiter une livraison

Pour traiter une livraison, appuyez sur la vignette de la livraison à traiter. Vous aurez alors les informations sur la livraison :

{% embed url="https://www.screencast.com/t/j1BoVSBJ5vH6" %}
Détails d'une livraison
{% endembed %}

1. Numéro de la livraison généré par l’application et type de la livraison
2. Date et heure à laquelle le demandeur a indiqué que la livraison doit se faire
3. Nom du patient
4. Numéro de dossier du patient
5. Contact du patient et personne à prévenir. Si vous appuyez sur les numéros de téléphone, vous serez redirigé vers l’application de téléphone du terminal mobile.
6. Adresse de livraison
7. Remarque que le demandeur a pu fournir sur la demande
8. Informations diverses. Ces informations peuvent varier, elle sont liées au champs libre d'un type de livraison ou collecte
9. Nombre de colis à livrer et répartition de la quantité de colis par contenu du colis

Pour indiquer que vous avez livré les colis chez le patient, appuyez sur le bouton <mark style="background-color:blue;">**Déposer les colis**</mark>.

Vous arriverez alors sur la liste des colis à livrer à ce patient. Flashez tous les colis à donner au patient pour déverrouiller le bouton <mark style="background-color:blue;">**VALIDER**</mark>. Validez la dépose chez le patient.

{% embed url="https://www.screencast.com/t/e49UiCHX" %}
Livraison des colis chez le patient
{% endembed %}

Vous aurez alors un écran récapitulatif de la livraison, avec le nombre de colis à livrer. Vérifiez les informations. Vous avez la possibilité de mettre un commentaire, de prendre une photo et de faire signer le patient si nécessaire. Cliquez sur <mark style="background-color:blue;">**TERMINER LA LIVRAISON**</mark> pour valider définitivement la livraison.

La livraison passe alors tout en bas de la liste des points de passage avec un check vert dessus attestant qu’elle a bien été effectuée.

### Impossibilité de livrer

Si vous n’êtes pas en mesure de livrer des colis pour un patient, allez sur la livraison, et au lieu de sélectionner Déposer les colis, appuyez sur <mark style="background-color:blue;">**Non livrée**</mark>.

Vous devez alors indiquer impérativement un motif de non-livraison. Les motifs de non livraison sont paramétable dans le paramétrage ([Track>tournée](../../parametrages/track/tournees.md)). Vous pouvez également mettre un commentaire ou encore prendre une photo si cela permet d’illustrer pourquoi vous ne pouvez pas livrer.

{% embed url="https://www.screencast.com/t/GHdTdcT6qT2G" %}
Livraison impossible
{% endembed %}

Appuyez sur <mark style="background-color:blue;">**TERMINER LA LIVRAISON**</mark> pour valider le fait que vous n’avez pas pu livrer.

Une notification web sera envoyée à tous les utilisateurs de l'application pour les informer du problème concernant cette livraison. Voir [ici](../fonctionnalites-web/demandes/suivre-le-traitement-dune-demande-de-livraison.md#livraison-non-livree) les autres impacts sur la demande.

Vous êtes redirigé alors vers la liste des transports à faire et la livraison non livrée passe tout en bas avec une croix dessus.

**Pour une livraison/collecte**, si vous n’arrivez pas à accéder au patient, procédez comme sur la livraison classique. La collecte à faire après la livraison sera automatiquement considérée comme non collectée.

## Traiter une collecte

Pour traiter une collecte, appuyez sur la vignette de la collecte à traiter.

Vous aurez alors les informations de la collecte à traiter. Les informations sont les mêmes que sur la livraison, excepté pour la date et heure de collecte prévue, où vous aurez seulement la notion de créneau de passage.

Sur la collecte, pas de colis à livrer. On parle d’objets à collecter :&#x20;

{% embed url="https://www.screencast.com/t/Pu309MjPA0IF" %}
Liste des objets à collecter
{% endembed %}

Vous avez une liste des natures des objets à collecter, et éventuellement une quantité si la personne ayant fait la demande connaissait cette quantité. Cette quantité reste toutefois indicative. Sinon un "/" apparaitra.

Pour effectuer la collecte, appuyez sur <mark style="background-color:blue;">**Collecter les objets**</mark>.

{% embed url="https://www.screencast.com/t/At7PtleCqAhC" %}
Traitement d'une collecte
{% endembed %}

Vous aurez la liste des objets à collecter. Indiquez la quantité collectée de chaque nature et appuyez sur <mark style="background-color:blue;">**VALIDER**</mark>.

Comme sur la livraison, vous arriverez au récapitulatif de la collecte. Vous avez la possibilité de mettre un commentaire, de prendre une photo à joindre, ou bien de faire signer le patient si nécessaire, comme sur la livraison.

Appuyez sur <mark style="background-color:blue;">**TERMINER LA COLLECTE**</mark> pour valider définitivement son traitement.

La collecte se positionne alors en bas des points de passage à traiter.

### Impossibilité de collecter

Si vous n’êtes pas en mesure de collecter les objets chez un patient, allez sur la collecte, et au lieu de sélectionner Collecter les objets, appuyez sur <mark style="background-color:blue;">**Non collectée**</mark>.

Vous devez alors indiquer impérativement un motif de non-collecte. Les motifs sont paramétable depuis le paramétrage ([Track>tournée](../../parametrages/track/tournees.md#collectes-livraisons)). Vous pouvez également mettre un commentaire ou prendre une photo si cela permet d’illustrer pourquoi vous ne pouvez pas collecter. S’il n’y a rien à collecter chez le patient, sélectionnez le motif renseigné dans "Fin du workflow collecte" pour indiquer que la collecte a déjà été effectué par une autre personne.

{% embed url="https://www.screencast.com/t/M2qVGhm4" %}
Collecte impossible
{% endembed %}

En fonction du motif que le livreur a renseigné, la collecte peut avoir 2 comportements \
possibles :

* Le motif implique de devoir repasser chez le patient : la demande repart dans le workflow. Elle passe directement du statut « Non collectée » à « En attente de planification ». Vous n’avez pas besoin de refaire la demande. le responsable recontactera le patient pour replanifier la demande sur une tournée
* Le motif implique de ne pas repasser chez le patient : la demande s’arrête au statut « Non collectée » et est définitivement terminée.

## Traiter une livraison/collecte

Lorsque vous avez une livraison/collecte, la vignette ressemblera à ça :

{% embed url="https://www.screencast.com/t/jonIeZjA" %}
Vignette de livraison/collecte
{% endembed %}

Dans le cas d’une livraison/collecte, le type de la livraison et de la collecte apparaîtront l’un en dessous de l’autre.

Appuyez dessus pour traiter la demande. Vous aurez d’abord à traiter d’abord la livraison, de la même façon que sur une livraison classique.

Vous verrez néanmoins sur le détail de la livraison l’indication qu’il faut prévoir de faire la collecte ensuite :&#x20;

{% embed url="https://www.screencast.com/t/3pycaMIb" %}

Traitez la livraison.

Vous serez alors redirigé automatiquement vers la collecte à effectuer. Le process est ensuite le même que pour traiter une collecte.

Une fois la collecte traitée, vous êtes redirigé vers la liste des transports à faire. La vignette de livraison/collecte est passée en bas, avec 2 checks dessus pour le bon traitement de la livraison et de la collecte.

### Impossibilité de livrer ou collecter

Si vous ne pouvez pas effectuer la livraison, procédez comme sur la livraison classique et cliquez sur <mark style="background-color:blue;">**Non livrée**</mark>. La collecte à faire après la livraison sera automatiquement considérée comme non collectée.

Si vous avez pu faire la livraison mais pas la collecte, effectuez le même process de non collecte que décrit au-dessus pour indiquer que vous n’avez pas pu collecter.&#x20;

Voir [ici](../fonctionnalites-web/demandes/suivre-le-traitement-dune-demande-de-livraison-collecte.md) les autres impacts sur la demande.

## Annulation d’un point de passage

Le demandeur a la possibilité d’annuler une demande sur votre tournée alors que vous avez commencé votre tournée.

S’il s’agit de votre prochain point de passage, vous aurez alors une notification pour vous en informer.

S’il s’agit d’une demande plus loin dans la liste, vous n’aurez pas de notification mais vous verrez que la demande est annulée.

{% embed url="https://www.screencast.com/t/G8VMRGEFLk" %}
Vignette de demande annulée
{% endembed %}

## Ajout d’une nouvelle tournée

Il est possible que vous ayez plusieurs tournées à faire sur une même journée.

Dans le cas où on vous rajouterait une tournée à faire sur la même journée alors que vous êtes déjà en train d’en faire une, vous aurez une notification.

Vous pouvez sortir de la tournée en cours pour voir la tournée qui vous attend.Il est possible de pouvoir traiter 2 tournées en parallèle sur l’application mobile.
