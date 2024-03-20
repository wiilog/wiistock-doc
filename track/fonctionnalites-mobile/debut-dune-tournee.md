# Début d'une tournée

## Liste des tournées

Les tournées sont rangées sous la date à laquelle la tournée doit être faite.

{% hint style="info" %}
Si des tournées apparaissent sur des dates qui sont passées, cela signifie que la tournée n’a pas été terminée ou qu’il reste des colis non livrés ou objets collectés à déposer.
{% endhint %}

Une vignette de tournée est constituée de&#x20;

<figure><img src="../../.gitbook/assets/Formations CLB16.png" alt=""><figcaption><p>Vignette de tournée</p></figcaption></figure>

1. **Numéro de la tournée**. Le numéro est constitué du préfixe T, de l’année, du mois, et du jour à laquelle la tournée doit être faite, et d’un compteur
2. **Nombre de livraisons** qui ont été préparées sur le nombre de livraisons total
3. **Nombre de colis chargé** dans le camion sur le nombre de colis total présent dans les livraisons
4. **Nombre de transports traité** sur le nombre de transports total dans la tournée
5. **Statut** de la tournée. La tournée a 3 statuts possibles :
   *   En attente livreur : la tournée n’a pas démarré. Les colis ne sont pas

       chargés
   * En cours : les colis ont été chargé et vous avez indiqué avoir débuté la tournée. Les transports sont en cours de traitement
   * Terminée : tous les transports ont été traités et l’emplacement de fin de livraison a été flashé
6. **Kilométrage** total estimé sur la tournée
7. **Temps** total estimé de la tournée
8. Bouton <mark style="background-color:blue;">**Charger**</mark> pour accéder à l’écran de chargement des colis
9. Bouton <mark style="background-color:blue;">**Débuter la tournée**</mark>. Ce bouton est disponible quand vous avez chargé tous colis. Il sert à démarrer la tournée et à passer tous les transports contenus dans la tournée à « En cours »

## Détails de la tournée et liste des points de passage

Vous pouvez visualiser les étapes de votre tournée en appuyant sur la vignette de la tournée. Vous pouvez ainsi voir la liste des patients chez lesquels vous devez passer.\
Vous pouvez voir précisément leur localisation en appuyant sur Voir le circuit de la tournée.

Les vignettes grisées sont les vignettes des livraisons qui n’ont pas encore été préparées, et qui seront rejetées de la tournée si vous devez commencer votre tournée alors que le demandeur ne les a toujours pas préparées (voir plus bas).

Vous avez également la possibilité d’avoir plus d’informations sur la livraison ou la collecte en appuyant sur la vignette de la livraison ou collecte.

## Démarrer la tournée

### Charger les colis

Pour charger les colis, appuyer sur le bouton Charger les colis.\
Vous verrez alors la liste de tous les colis à charger sous la zone « Colis à charger ».

{% embed url="https://www.screencast.com/t/e49UiCHX" %}
&#x20;Liste de colis à charger
{% endembed %}

Sur la vignette d’un colis à charger, vous avez l’information du numéro de tracking du colis (Colis), de la nature de ce qu’il contient (Nature), et de la plage de température à laquelle il doit rester (Température).

Scanner les étiquettes des colis à mettre dans le camion. Les vignettes des colis scannés passent alors dans la zone « Colis scannés ». Vous devez procéder par étape pour charger les colis en scannant les colis en même temps qui doivent être conservés à la même température. Une fois que les colis devant être conservés à la même plage de température sont scannés, appuyez sur <mark style="background-color:blue;">**VALIDER**</mark>. Vous êtes alors dirigés vers un écran permettant de sélectionner l’emplacement sur lequel vous déposer les colis. Si vous scannez un emplacement n’ayant pas la bonne plage de température, vous aurez un message d’erreur et vous ne pourrez pas charger les colis sur l’emplacement sélectionné. Les colis sans températures peuvent être déposés sur n'importe quel emplacement.

Si le scan du zebra ne fonctionne plus, vous pouvez passer par l’appareil photo du terminal disponible dans la zone « Colis à charger ».

Si l’appareil photo a aussi un souci, vous pouvez appuyer sur les flèches présentes sur chaque vignette de colis pour les passer dans la zone « Colis scannés ». La grande flèche dans la zone « Colis à charger » permet de passer tous les colis présents dans cette zone dans la zone « Colis scannés ».&#x20;

{% hint style="warning" %}
Néanmoins, le fait de scanner via le flash ou l’appareil photo est fortement préconisé pour diminuer le risque d’erreur de chargement.
{% endhint %}

### Ecarter un colis

Si un des colis que vous devez charger à un souci ou est inexistant, vous avez la possibilité de l’écarter pour qu’il ne soit pas pris en compte pour la tournée.

Pour cela, dans la liste des colis à charger, sur la vignette du colis à écarter, faite un glisser de la gauche vers la droite pour faire apparaître un bouton <mark style="background-color:blue;">**Ecarter**</mark>. Appuyez sur le bouton Ecarter. Une modale apparaîtra alors avec les différents motifs possibles de pourquoi le colis doit être écarté. Sélectionnez le motif et validez (la liste doit être paramétré dans [Track/tournées](../parametrages/tournees.md#colis-ecartes)). Le colis n’apparaîtra plus alors dans la liste des colis à charger. Sur les demandes de transport, l’information que le colis a été écarté et le motif remontera.

{% embed url="https://www.screencast.com/t/vJIhwpY1nTzI" %}

### Débuter la tournée

Une fois tous les colis chargés, le bouton <mark style="background-color:blue;">**Débuter la tournée**</mark> est disponible.

Vous devez appuyer dessus pour déclencher le début de la tournée et pour pouvoir traiter les demandes. Une fois que vous aurez appuyé dessus, vous serez redirigé vers la liste des transports à traiter et la flèche de navigation qui ouvre Google maps sera disponible.

#### Rejet d’une livraison non préparée de la tournée

Si une livraison n’a toujours pas ses colis préparés quand vous devez débuter la tournée, vous pouvez quand même commencer votre tournée. Pour cela, cliquez sur <mark style="background-color:blue;">**Débuter la tournée**</mark>, un message apparaîtra, vous prévenant que des livraisons vont être rejetées de la tournée si vous confirmez. Confirmez pour que la livraison ne fasse plus partie de la tournée. Elle sera alors à replanifier sur une autre tournée par le responsable d’exploitation.

#### Nouveaux colis ajoutés

Il est possible également qu’entre le moment où vous ayez charger tous les colis indiqués et où vous appuyez sur Débuter la tournée, le responsable est ajouté des nouveaux colis sur les livraisons. Lorsque vous appuyez sur <mark style="background-color:blue;">**Débuter la tournée**</mark>, l’application vérifie la présence ou non de nouveaux colis. Dans le cas où des nouveaux colis ont été ajouté, vous aurez un message d’alerte et vous serez redirigé vers l’écran de chargement des colis avec les nouveaux colis à charger. Chargez les nouveaux colis pour pouvoir débuter la tournée.

## Pendant la tournée

### Liste des transports

Après avoir appuyez sur <mark style="background-color:blue;">**Débuter la tournée**</mark>, vous êtes redirigé vers la liste des différents transports à traiter.

Vous pouvez voir maintenant que la tournée est en cours, ainsi que toutes les demandes contenues dedans.

Vous pouvez voir où vous en êtes de votre tournée grâce au compteur sous <mark style="background-color:blue;">**Voir le circuit de la tournée**</mark>.

Chaque transport est représenté par une vignette qui contient les informations suivantes :&#x20;

{% embed url="https://www.screencast.com/t/1C9rZaad" %}
Vignette d'une livraison
{% endembed %}

1. Numéro dans la tournée de ce transport et nom et prénom du patient
2. Type du transport. Dans l’exemple, il s’agit d’une livraison. Il peut aussi y avoir une collecte ou alors une livraison/collecte. Dans ce cas, lorsque vous faites une livraison chez un patient, vous devez également effectuer une collecte à la suite.
3. Nombre de colis destiné au patient. Dans le cas d’une livraison ou d’une livraison/colis, vous verrez apparaître combien de colis sont à livrer au patient
4. Type de la livraison, ou type de la collecte. Dans le cas d’une livraison/collecte, le type de la livraison et de la collecte apparaîtront l’un en dessous de l’autre.
5. Heure de passage maximale obligatoire pour la livraison. Pour une collecte, vous aurez le créneau validé avec le patient (matin ou après-midi)
6. Estimation de l’heure de passage chez le patient. Attention, l’estimation ne prend pas en compte les conditions de trafique routier.
7. Adresse du patient
8. Bouton permettant d’ouvrir une application de navigation GPS déjà positionné sur l’adresse du patient
