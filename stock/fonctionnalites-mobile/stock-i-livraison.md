# Stock I Livraison

Suite au traitement de l'ordre de préparation l'ordre de livraison arrive sur ce menu. C'est la dernière étape pour valider la demande de livraison.

Vous avez la liste sous forme de "carte" avec plusieurs informations :&#x20;

* **Demandeur** : Utilisateur qui a créé la demande de livraison
* **Numéro** (ex : L-20230414170506-01) : Numéro de l'ordre de livraison avec le format L-aaaammjjhhmmss-n
* **Flux** : Indication du type de livraison
* **Destination** : Emplacement de destination de la demande de livraison
* **Commentaire** : commentaire de la livraison
* **Emplacement de préparation** : Emplacement de fin de préparation
* **Date attendue** : Date souhaitée de livraison (en fonction de la date la couleur de l'entête change voir [Paramétrage > Terminal mobile > Préparations/Livraisons](../../parametrages/terminal-mobile/preparation-livraison.md))
* **Projet** : Indication du projet de la livraison issu du référentiel projet

La loupe et l'appareil photo servent à filtrer sur les emplacements de préparation.

{% embed url="https://www.screencast.com/t/ki8luERjGGN" %}
Page Stock / Livrasion
{% endembed %}

## Traitement de la livraison

Rentrer dans le détail d'un ordre de livraison, vous allez avoir le numéro de l'ordre de livraison et la destination de la demande de livraison. Puis 2 encarts "Livré" et "À livrer" qui contient la liste des références / articles / unités logistiques à déplacer. Au fur et à mesure que vous scannez vos références, elles vont se transférer dans "Livré". Cela indique que vous les avez bien déplacés.

Pour passer une référence / articles / unités logistiques de "À livrer" à "Livré" vous pouvez scanner ou prendre en photo (via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>)) le Code barre. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo.

{% embed url="https://www.screencast.com/t/IEOQgFZJTlD" %}

Une fois vos références ou articles scannés, vous devez valider la quantité prise.

Quand vous avez fini cliqué sur <mark style="background-color:blue;">**Valider**</mark>, vous devez alors choisir un emplacement de livraison, <mark style="background-color:blue;">**Valider**</mark> à nouveau. La livraison est traitée, elle va donc disparaitre de la liste des livraisons à traiter.

Avec l'activation du paramétrage _"Autoriser la dépose des articles sur un emplacement libre"_ dans [Pramétrage > Terminal mobile > Livraison](../../parametrages/terminal-mobile/livraisons.md)  vous pourrez déposer vos références ou articles sur n'importe quel emplacement. Sinon l'application vous obligera à les déposer sur l'emplacement de destination de la demande de livraison.

### Références

Sur une carte de référence vous avez comme info :&#x20;

* **Label** : Libellé de la référence
* **Code barre** : Code barre de la référence (ex : REF230400001)&#x20;
* **Emplacement** : Emplacement de la référence&#x20;
* **Quantité** : Quantité préparée (à l'étape Préparation)

### Articles

Sur une carte d'article vous avez comme info :&#x20;

* **Label** : Libellé de l'article
* **Code barre** : Code barre de l'article (ex : ART230400001)&#x20;
* **Emplacement** : Emplacement de préparation de l'article&#x20;
* **Quantité** : Quantité demandée

Avec l'activation du paramétrage _"Afficher le code référence et le rendre scannable. Enlever le code article."_ dans [Pramétrage > Terminal mobile > Livraison](../parametrage/demandes/livraisons/)  vous pourrez scanner le code de référence à la place du code barre.

### Unités logistiques (avec Articles)

Sur une étiquette carte d'unité logistique vous avez comme info :&#x20;

#### Carte unité logistique

* **Objet** : Numéro de l'unité logistique
* **Nombre d'article** : nombre d'article contenu dans l'unité logistique&#x20;
* **Emplacement** : Dernier emplacement de l'UL

#### Carte article contenu

* **Libellé** : Libellé de la référence
* **Code barre** : _Code barre de l'article (ex : ART230400001)_&#x20;
* **Emplacement** : Dernier emplacement de l'UL&#x20;
* **Quantité** : Quantité de l'article
* **Référence** : Code de référence de l'article

## Mouvement de stock

À la validation de la livraison, il y a un mouvement de sortie de stock entre l'emplacement de préparation et l'emplacement de destination.&#x20;

* La référence sera alors décrémentée de la quantité livrée.&#x20;
* L'article sera passé en "consommé" et la quantité livrée sera décrémentée sur la référence.
*
* **Libellé** : Libellé de la référence
* **Code barre** : _Code barre de l'article (ex : ART230400001)_&#x20;
* **Emplacement** : Dernier emplacement de l'UL&#x20;
* **Quantité** : Quantité de l'article
* **Référence** : Code de référence de l'article
