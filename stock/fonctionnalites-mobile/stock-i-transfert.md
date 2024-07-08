---
description: >-
  Cette fonctionnalité sert à transférer une référence ou un article
  d'emplacement, sans sortie de stock.
---

# Stock I Transfert

L'ordre de transfert est généré suite à la validation de la demande de transfert. L'ordre est ce qui sera traité, et son traitement passera la demande en traité. Vous pouvez traiter l'orde sur le web et sur le nomade.

Vous avez la liste sous forme de "carte" avec plusieurs informations :&#x20;

* **Demandeur** : Utilisateur qui a créé la demande de transfert
* **Numéro** (ex : OT-202305100002) : Numéro de l'ordre de transfert avec le format OT-aaaammjj000n
* **Origine** : Emplacement de stockage des références ou article
* **Destination** : Emplacement de destination souhaité
* **Références contenues** _(option à afficher)_ : Liste des références du transfert. Elle peut être affiché avec le paramétrage "Afficher les références contenues sur les étiquettes de transfert" dans [parametrages/terminal-mobile/gestion-des-validations](../../parametrages/terminal-mobile/gestion-des-validations.md)

{% embed url="https://www.screencast.com/t/ytjuxcO2t37e" %}

## Traitement d'un transfert

Rentrer dans le détail d'un ordre de transfert, vous retrouvez le numéro de l'ordre de transfert, l'emplacement d'origine et de destination et le demandeur. Puis 2 encarts "Transféré" et "À transférer" qui contient la liste des références/articles à déplacer.&#x20;

**Informations encart d'un article** :&#x20;

* **Code barre** : Code barre de l'article (ex : ART230400001) &#x20;
* **Référence** : Code de référence de l'article
* **Libellé** : Libellé de la référence
* **Emplacement** : Emplacement de l'article&#x20;
* **Quantité** : Quantité total de l'article

**Informations encart d'une référence** :&#x20;

* **Code barre** : Code barre de la référence (ex : REF230400001) &#x20;
* **Référence** : Code de référence
* **Libellé** : Libellé de la référence
* **Emplacement** : Emplacement de la référence&#x20;
* **Quantité** : Quantité total de la référence

Au fur et à mesure que vous scannez vos références, elles vont se transférer dans "Transféré". Cela indique que vous les avez bien déplacés. Pour passer une référence / articles de "Transféré" à "À transférer" vous pouvez scanner ou prendre en photo (via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>)) le Code barre. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo.

La dernière étape est d'indiquer l'emplacement de destination. Il peut être différent de l'emplacement de destination si vous avez cocher "Autoriser la dépose des articles sur un emplacement libre" dans le paramétrage  [Paramétrage > Terminal Mobile > Transferts à traiter.](../../parametrages/terminal-mobile/transfert-a-traiter.md)

{% embed url="https://www.screencast.com/t/hRUoKk9f" %}

Suite à la validation du transfert, il va alors se passer :&#x20;

* L'**ordre de transfert** passe au statut _**Traité**_
* La **demande de transfert** passe au statut _**Traité**_
* Un **mouvement de transfert** est créé pour chaque référence/article de l'ordre de transfert allant de l'emplacement d'origine à l'emplacement de destination indiqué sur la demande de transfert

