---
description: >-
  Cette fonctionnalité sert à déplacer une référence, un article ou une unité
  logistique d'un emplacement à un autre, sans sortie de stock, sans passer par
  une demande.
---

# Stock I Transfert manuel

Cette fonctionnalité permet de faire des transfert facilité sans avoir besoin de passer par les demandes et les ordres de transfert. Il se compose de 2 sous menu :&#x20;

<figure><img src="../../.gitbook/assets/Capture d’écran 2023-06-27 164926.png" alt=""><figcaption><p>Sous-menu du transfert manuel</p></figcaption></figure>

## Prise

Sélectionnez l'emplacement de stockage de vos références, articles ou unités logistiques, ils doivent être sur cet emplacement, sinon la prise ne sera pas possible.

Scanner le code barre de référence, d'article ou d'unité logistique à prendre. Vous pouvez aussi le prendre en photo (via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>)) ou faire une entrée manuelle, si vous ne pouvez pas utiliser le scan ou la photo.

Un encart par référence ou article apparaitra avec :&#x20;

* **Objet** : le code barre de la référence (REF2305000079) ou article (ART2303000016)
* **Quantité** : quantité totale de la référence ou de l'article sur cet emplacement
* **Date / Heure** : Date et heure de scan

Un encart par unité logistique apparaîtra avec :&#x20;

* **Objet** : L'identifiant de l'unité logistique _(ex : PAL12340000056)_
* **Nombre d'article** : la quantité totale de référence ou d'article contenu dans cette UL.&#x20;
* **Date / Heure** : Date et heure de scan
* **Nature** : La nature de l'unité logistique _(ex : Palette, carton, etc)_

Si vous vous être trompé, vous pouvez cliquer sur la poubelle d'un encart pour supprimer la prise de l'objet.

### Particularité de la prise d'Unité Logistique

Lors de la prise d'une unité logistique via la fonctionnalité "Transfert manuel", il est possible d'ajouter des informations sur l'unité logistique et son mouvement. Il est également possible de visualiser les articles ou références contenus dans l'unité logistique.

Pour cela, cliquez sur l'unité logistique que vous voulez visualiser. Vous pourrez switcher entre les affichages via les boutons "<mark style="background-color:blue;">**Mouvement**</mark>" et "<mark style="background-color:blue;">**Contenu UL**</mark>".

Les éléments suivants s'enregistreront sur le mouvement de prise : **Commentaire, Signature, Photo** tandis que **le Projet** s'enregistrera sur l'unité logistique.

<figure><img src="../../.gitbook/assets/Capture d’écran 2023-06-27 161107.png" alt=""><figcaption><p>Détail d'une UL sur une prise de transfert manuel</p></figcaption></figure>

Une fois toutes les références/articles scannés, valider la prise en cliquant sur le bouton <mark style="background-color:blue;">**Valider**</mark>.

L'application vous indique le nombre de produits en prise.

<figure><img src="../../.gitbook/assets/Capture d’écran 2023-06-27 162926.png" alt=""><figcaption><p>Finalisation d'une prise de transfert manuel</p></figcaption></figure>

## Dépose

Sélectionner l'emplacement de dépose, qui sera le nouvel emplacement de stockage de vos références, articles ou unités logistiques.

L'application vous donne la liste des objets en prise, pour passer une référence/article/UL de "Prise" à "Dépose" vous pouvez scanner ou prendre en photo (via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>)) du code barre. Vous pouvez aussi utiliser la flèche, si vous ne pouvez pas utiliser le scan ou la photo. Si vous vous être trompé, vous pouvez cliquer sur la poubelle d'un encart.

Une fois toutes les références/articles scannés, valider la dépose en cliquant sur le bouton <mark style="background-color:blue;">**Valider**</mark>.

<figure><img src="../../.gitbook/assets/Capture d’écran 2023-06-27 163457.png" alt=""><figcaption><p>Validation d'une dépose d'un transfert manuel</p></figcaption></figure>

## Mouvements

Suite à la validation du transfert, on verra les éléments suivants sur le web :&#x20;

* Un **mouvement de transfert** créé pour chaque référence/article allant de l'emplacement d'origine à l'emplacement de destination.
  * Les articles et références contenus dans l'unité logistique transférée portent eux aussi un mouvement de transfert.
* Deux **mouvements de traçabilité** créé pour chaque unité logistique transférée. _(Prise et dépose)_
