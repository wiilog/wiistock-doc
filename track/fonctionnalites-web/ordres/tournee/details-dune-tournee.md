# Détails d'une tournée

Le détail d’une tournée est constitué de 3 zones :

* **Zone Tournées** : elle récapitule des informations sur la tournée
* **Zone Transports** : cette zone permet de savoir les patients chez qui le livreur doit passer durant sa tournée et les différentes informations de traitement
* **Zone Données** : cette zone récapitule les points de passage sur une carte et la dernière position du livreur si la tournée est en cours, ainsi que le suivi de la température sur les différents frigos présents dans le camion du livreur sur toute la durée de la tournée.

<figure><img src="../../../../.gitbook/assets/Formations CLB12.png" alt=""><figcaption><p>Détails d'une tournée</p></figcaption></figure>

## Zone Tournée

{% embed url="https://www.screencast.com/t/Xb3WwfhZet1" %}

1. **Numéro** de la tournée
2. **Personne ayant créée la tournée**
3. **Date à laquelle la tournée doit se faire**
4. **Livreur** en charge de la tournée
5. **Dernier** **statut** de la tournée
6. **Historique des statuts de la tournée.** Si le statut est vert, cela signifie que c’est le statut actuel. Si le statut est bleu, cela signifie qu’il est passé. S’il est gris, cela signifie que la tournée n’est pas encore passée par ce statut, il n’y aura aucun horodate face à ce statut dans ce cas. L’horodatage correspond à la date et heure auxquelles la tournée est passée sur le statut
7.  **Indication du temps estimé** lors de la planification de la tournée et **temps réel** calculé de la tournée lorsque la tournée est terminée.\
    L’estimation est calculée depuis le point de départ calcul horaire jusqu’au point de fin de tournée. Le temps pris en compte chez le patient dépend du [paramétrage](../../../parametrages/tournees.md#calcul-kilometrage-et-duree).

    Le temps réel se base sur l’horodate de début de tournée (horodatage devant le statut « En cours ») et sur l’horodatage de fin de tournée (horodatage devant le statut « Terminée »)
8. **Indication du kilométrage estimé** lors de la planification de la tournée et **kilométrage réel** lorsque la tournée est terminée.\
   Le kilométrage estimé se base sur le kilométrage entre le "Point de départ km" et le "Point de départ calcul des horaires", puis entre le "Point de départ calcul des horaires" et le 1er point de passage, puis entre chaque point de passage jusqu’au retour au dépôt. Le kilométrage réel se base sur les positions GPS relevées par le hub Koovea durant tout le trajet de la tournée. (si vous utiliser un objet connecté pour suivre vos livreurs)
9.  La partie « **Eléments rejetées** » apparaît seulement si au moins 1 colis a été écarté sur la tournée et/ou si au moins 1 livraison a été rejetée de la tournée. \
    **Un colis peut être écarté** de la tournée par le livreur s’il ne trouve pas le colis ou s’il estime que le colis n’est pas conforme. Sur la liste des transports, l’icône de colis écarté apparaît sur le transport en question.

    **Une livraison peut être rejetée** d’une tournée si tous les colis contenus dans la livraison sont écartés, ou si aucun colis n’a été préparé pour la livraison. La livraison n’apparaîtra plus alors dans la liste des transports mais vous aurez l’information de cette section transport qu’une livraison normalement prévue sur cette tournée devra être replanifiée sur une autre tournée.

## Zone Transport

{% embed url="https://www.screencast.com/t/VBZ0Gwy0" %}
Détails d'une tournée, partie Transport
{% endembed %}

1. Accès à des **boutons d’actions.** Les boutons qui apparaissent changent selon le statut de la tournée quand vous cliquez sur les ![](<../../../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>)&#x20;
   * Dans l’exemple, la tournée est en statut « Terminée ». Vous avez seulement accès au bouton <mark style="background-color:blue;">**Générer un bon de transport**</mark> qui apparaît à n’importe quel statut de la tournée. Ce bouton permet de générer un PDF contenu une feuille de bon de transport pour chaque livraison de la tournée.
   * Si la tournée est au statut « En attente livreur », vous aurez le bouton <mark style="background-color:blue;">**Ajouter un transport**</mark> en plus du bouton précédent. Cliquez dessus pour accéder à la page de planification de tournée. Vous pouvez modifier la tournée en ajoutant une livraison ou une collecte et en modifiant l’ordre des points de passage. Vous pouvez également changer le livreur et refaire le calcul des estimations. Il ne sera pas possible de revanche de supprimer des points de passage.
   * Si la tournée est au statut « En cours », le bouton Ajouter un transport se change en <mark style="background-color:blue;">**Ajouter une collecte**</mark>. Cliquez dessus pour accéder à la page de planification de tournée. Vous pouvez alors seulement ajouter des collectes sur la tournée en cours.
2.  **Indication sur l’ordre de transport**

    * Sur l’exemple, le logo ![](<../../../../.gitbook/assets/colis écarté>)vient indiquer que la livraison contient un ou des colis qui ont été écartés par le livreur quand il a chargé les colis dans son camion. Vous pouvez retrouver quels colis ont été écarté et pour quelle raison en allant sur le détail de l’ordre en cliquant sur le nom de la personne
    * Il est possible également qu’il y est un logo rouge avec une croix. Ce logo signifie que le transport a été annulé.\
      &#x20;

    <figure><img src="../../../../.gitbook/assets/Capture d’écran 2023-02-03 à 16.55.40.png" alt=""><figcaption></figcaption></figure>
3. Indication si le transport est une **livraison ou une collecte**
4. **Numéro du transport** dans la tournée
5.  **Nom du patient**. Le nom du patient est cliquable et renvoie sur la page du

    détail d’un ordre de transport
6. Couleur du transport en fonction de son avancement :
   * Transport en vert : point de passage en cours de traitement
   * Transport en gris : point de passage futur
   * Transport en bleu : point de passage traité
7. **Heure d’estimation** de passage suite à la planification sur la tournée
8. **Heure réelle de traitement** de la demande suite au traitement de l’ordre sur la tournée par le livreur

## Zone Données

<figure><img src="../../../../.gitbook/assets/Formations CLB15.png" alt=""><figcaption><p>Détails d'une tournée, partie Données</p></figcaption></figure>

### Sur la carte :

1. **Point de départ de la tournée** : Sur l’exemple, il s’agit aussi du point de d’arrivée. Vous pouvez dissocier les 2. Ces 2 points permettent de calculer le kilométrage de la tournée (estimé et réel)
2. **Point de départ du calcul des horaires** de passage
3. **Point de passage** chez le patient, avec le numéro de passage dans la tournée
4. **Dernière position du livreur**. Cette position apparaît si la tournée est en cours

### Sur la courbe de température :&#x20;

5. **Nom de la sonde de température** et de l’emplacement sur lequel est la sonde
6. **Borne haute** de température à ne pas dépasser
7. **Courbe de la température** relevée
8. **Borne basse** de température à ne pas dépasser
9. **Horodatage** des relevés de température. Cet horodatage commence au début de la tournée et s’arrête à la fin

Si le camion du livreur contient plusieurs frigos, vous aurez autant de graphique que de frigos (si vous avez associé une sonde à chaque frigo.)

## Modifier une tournée

Pour modifier une tournée **non démarrée**, vous pouvez :

* Cliquer sur les ![](<../../../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>) à côté de Transports et cliquez sur <mark style="background-color:blue;">**Ajouter un transport**</mark>
*   Soit aller dans [Ordre | Planning](../planning.md), cliquez sur <mark style="background-color:blue;">**Planifier une tournée**</mark>, puis sélectionnez « <mark style="background-color:blue;">**Ajouter à la tournée**</mark> » et choisissez le numéro de la tournée que vous souhaitez modifier.

    Vous arrivez alors sur la page de planification de tournée. Vous pouvez :

    * Modifier l’ordre des points de passage
    * Ajouter des points de passage
    * Changer les points de début et fin de tournée, et de début de calcul horaire
    * Changer le livreur
    *   Changer l’heure de départ

        Effectuez vos modifications et cliquez sur « Valider la tournée » pour que les changements soient pris en compte.

        **Si une tournée est en cours**, vous serez en mesure d’ajouter seulement des collectes sur la tournée en cours.

{% hint style="info" %}
Si un livreur doit effectuer des nouvelles livraisons, vous devez lui créer une nouvelle tournée avec ces livraisons.
{% endhint %}
