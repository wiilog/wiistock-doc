# Traçabilité I Mouvements I Prise & Dépose

La prise et la dépose sont les fonctionnalités de base de la traçabilité dans Wiilog afin de mouvementer les unités logistiques d'emplacement en emplacement.&#x20;

Ces 2 menus sont accessibles dans la partie **Traçabilité** du terminal mobile, sous le menu **Mouvements**.&#x20;

Dans le menu **Mouvements**, avant d'aller faire une prise ou une dépose, vous pouvez voir dans le bandeau en haut le nombre de prises en cours que vous avez.

## Prise

Pour faire une prise, c'est-à-dire indiquer que vous enlevez une unité logistique (colis, palette, etc.) d'un emplacement, allez dans le menu _**Prise**_.

### **Sélectionner un emplacement**

Vous devez d'abord venir scanner un emplacement pour indiquer où vous venez réaliser la prise.

Si le scanner à un souci, vous pouvez appuyer sur l'icône d'appareil photo avec un code barre pour accéder à l'appareil photo du terminal mobile et scanner le code barre ou le QR Code de l'emplacement avec celui-ci.&#x20;

<img src="../../.gitbook/assets/Screenshot_20220713-145349_Follow GT (1).jpg" alt="" data-size="original">

Si vous n'avez pas accès à un code barre ou QR Code, appuyez sur la loupe pour accéder à la sélection manuelle de l'emplacement. Vous accédez alors à l'écran de sélection d'emplacement. Vous pouvez rechercher l'emplacement concerné en tapant dans le champ Rechercher au moins 3 caractères. Appuyez sur le nom de l'emplacement voulu pour le sélectionner et passer à l'écran de sélection de l'unité logistique.&#x20;

### **Sélectionner des unités logistiques**

#### **Flash d'une UL**

Sur cet écran, scannez les codes barres ou les QR Codes des unités logistiques que vous souhaitez prendre sur cet emplacement.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220713-150332\_Follow GT.jpg>)

De même que pour la sélection de l'emplacement, vous pouvez scanner avec l'appareil photo en appuyant sur l'icône avec l'appareil photo et le code barre, ou taper à la main le nom de l'unité logistique souhaitée dans la zone "_Entrée manuelle ..._".

La traçabilité Wiilog est une traçabilité libre : l'unité logistique n'est pas obligée d'être connue par l'application pour être scanné. De plus, il n'y pas de contrôle effectué entre l'emplacement de prise de l'unité logistique et le dernier emplacement connue de celle-ci.&#x20;

Lorsqu'une unité logistique est scannée, elle apparaît dans une rectangle avec les informations suivantes :&#x20;

* **Objet** : nom de l'unité logistique
* **Quantité** : quantité contenue de l'unité logistique
* **Date / Heure** : date et heure du scan de l'unité logistique
* **nature** : nature de l'unité logistique. Ce champ apparaît si l'unité logistique est connue par l'application. Si l'unité logistique n'est pas connue, le champ n'apparaît pas. S'il y a une nature, à gauche du rectangle, un bandeau de couleur correspondant à la couleur de la nature apparaît.

![](<../../.gitbook/assets/Screenshot\_20220713-154223\_Follow GT2.jpg>)



Il existe également un paramétrage qui vous permet de voir toutes les unités logistiques en en cours sur l'emplacement flashé.

Pour cela, il faut aller activer le paramétrage "_En cours visible nomade?_" sur la modale de modification d'un emplacement.&#x20;

{% hint style="info" %}
Attention, pour des raisons de performance, il n'est pas conseillé d'activer ce paramétrage sur un emplacement ayant un encours important
{% endhint %}

Vous aurez alors sur l'écran de sélection de prise, une zone _ENCOURS_ qui apparaîtra avec les unités logistiques disponibles sur cet emplacement.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220722-113522\_Follow GT.jpg>)

#### Supprimer une unité logistique

Si vous vous êtes trompés en scannant, appuyez sur le poubelle rouge à droite dans le rectangle de l'unité logistique pour l'enlever des éléments en prise.&#x20;

#### Ajouter des informations sur un mouvements de prise

Appuyez sur le rectangle de l'unité logistique pour accéder à un écran permettant d'ajouter des informations sur le mouvement de prise. Les champs suivants sont disponibles sur l'écran :&#x20;

* **nature** : nature de l'unité logistique. Vous pouvez modifier la nature de l'unité logistique ici. Si l'unité logistique n'en a pas, vous pouvez ajouter une nature.
* **Quantité** : quantité contenue de l'unité logistique. Vous pouvez modifier cette quantité ici
* **Commentaire** : vous pouvez ajouter un commentaire sur le mouvement de prise
* **Signature** : vous pouvez ajouter une signature sur le mouvement de prise. En appuyant sur ce champ, vous ouvre une page de signature
* **Photo** : vous pouvez ajouter une photo sur le mouvement de prise. Si vous avez pris une photo et que vous souhaitez la supprimer pour en reprendre une autre ou ne pas en mettre du tout, appuyez sur la photo

Appuyez sur <mark style="background-color:blue;">**Valider**</mark> pour valider l'ajout des informations.&#x20;

Toutes les informations ajoutées ici pourront être visualisées sur la supervision sur la page _**Traçabilité | Mouvements**_.

![](<../../.gitbook/assets/Screenshot\_20220713-153139\_Follow GT.jpg>)

### Sélectionner un groupe&#x20;

#### Flash d'un groupe

Pour voir comment faire un groupe, voir [Groupage & Dégroupage](tracabilite-i-groupage-degroupage.md).&#x20;

Lorsque vous scannez un groupe, les informations dans le rectangle sont les suivantes :&#x20;

* **Objet** : nom du groupe
* **Nombre colis** : nombre d'unité logistique dans le groupe
* **Date / Heure** : date et heure du scan
* **nature** : nature du groupe. Le fonctionnement est le même que pour une unité logistique : si le groupe n'en a pas, le champ n'apparait pas

La prise d'un groupe va entrainer la prise de tous les éléments contenus dans le groupe.

![](<../../.gitbook/assets/Screenshot\_20220713-154223\_Follow GT.jpg>)



Vous pouvez aussi prendre seulement une unité logistique présente dans le groupe. Pour cela, flasher le code barre ou QR Code de cette UL sans flasher le groupe. Un message d'avertissement vous préviendra que l'UL sera alors retirée du groupe. Validez pour confirmer la prise.&#x20;

#### Ajouter des informations sur un mouvements de prise sur un groupe

Appuyez sur le rectangle du groupe pour accéder au même écran que celui décrit précédemment. Pour le groupe, vous ne pouvez pas changer la quantité.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220713-160024\_Follow GT.jpg>)

#### Voir le contenu du groupe

Appuyez sur le rectangle du groupe. Lorsque vous êtes sur la page pour ajouter des informations sur le mouvement, sélectionnez l'onglet _**Contenu colis**_ pour visualiser les unités logistiques contenues dans le groupe.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220713-160017\_Follow GT (1).jpg>)

### Sélection d'une unité logistique présente dans un groupe

Vous pouvez flasher directement une unité logistique qui est dans un groupe.&#x20;

A ce moment-là, vous aurez une modale d'avertissement qui vous préviendra que l'unité logistique scannée sera alors enlevée du groupe. Appuyez sur <mark style="background-color:blue;">**Confirmer**</mark> pour confirmer la prise.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220809-104320\_Follow GT.jpg>)

Le fonctionnement est ensuite le même que pour une prise d'une unité logistique classique.

### Valider la prise de tous les objets scannés

Lorsque vous avez scanné tous les objets souhaités, appuyez sur <mark style="background-color:blue;">**VALIDER**</mark> pour passer tous les éléments en prise.

Le numéro sur l'écran _**Mouvements**_ dans _Produits en prise_ s'incrémentera alors.&#x20;

Vous pouvez retrouvez les mouvements créés sur la supervision sur la page _**Traçabilité | Mouvements**_

## **Dépose**

Pour faire une dépose, c'est-à-dire indiquer que vous déposez une unité logistique (colis, palette, etc.) sur un emplacement, allez dans le menu _**Dépose**_.

### **Sélectionner un emplacement**

Comme sur la prise, vous devez d'abord venir scanner un emplacement pour indiquer où vous venez réaliser la dépose.

Si le scanner à un souci, vous pouvez appuyer sur l'icône d'appareil photo avec un code barre pour accéder à l'appareil photo du terminal mobile et scanner le code barre ou le QR Code de l'emplacement avec celui-ci.&#x20;

Si vous n'avez pas accès à un code barre ou QR Code, appuyez sur la loupe pour accéder à la sélection manuelle de l'emplacement. Vous accédez alors à l'écran de sélection d'emplacement. Vous pouvez rechercher l'emplacement concerné en tapant dans le champ Rechercher au moins 3 caractères. Appuyez sur le nom de l'emplacement voulu pour le sélectionner et passer à l'écran de sélection de l'unité logistique.&#x20;

### **Sélectionner des unités logistiques**

#### **Flash de l'UL**

Sur cet écran, vous disposez de la liste des unités logistiques en prise. Scannez le code barre ou QR Code de l'UL pour la passer dans la section _DEPOSE_.&#x20;

![](<../../.gitbook/assets/Screenshot\_20220722-112947\_Follow GT.jpg>)

De même que pour la sélection de l'emplacement, vous pouvez scanner avec l'appareil photo en appuyant sur l'icône avec l'appareil photo et le code barre, ou taper à la main le nom de l'unité logistique souhaitée dans la zone "_Entrée manuelle ..._". Vous pouvez aussi appuyez sur la flèche présente sur l'unité logistique ou bien appuyez sur la grande flèche à droite de l'appareil photo pour tout passer dans la section _DEPOSE_.&#x20;

Il peut y avoir des contraintes de dépose sur certains emplacements en fonction de la nature des unités logistiques. Si vous avez paramétré seulement quelques natures autorisées sur certains emplacements, si l'unité logistique n'a pas la bonne nature, un message d'erreur apparaîtra avec un avertissement sonore.

![](<../../.gitbook/assets/Screenshot\_20220722-120132\_Follow GT.jpg>)

#### Supprimer une unité logistique

Si vous vous êtes trompés en scannant, appuyez sur le poubelle rouge à droite dans le rectangle de l'unité logistique pour l'enlever des éléments en dépose et les repasser dans la zone _PRISE_.&#x20;

#### Ajouter des informations sur un mouvements de dépose

Pour ajouter des informations sur le mouvement de dépose d'une unité logistique, vous devez d'abord la passer dans la zone _DEPOSE_ pour pouvoir appuyez dessus et accéder au même écran de modification de mouvement qui présenté au dessus.&#x20;

### Déposer un groupe&#x20;

De même que pour la prise d'un groupe, la dépose d'un groupe va entrainer la dépose de tous les éléments contenus dans le groupe.

Vous pouvez choisir également de déposer une unité logistique seulement qui est présente dans le groupe. Pour cela, flasher directement le code barre ou QR Code de cette unité logistique pour la passer dans la section Dépose. Le nombre d'unités logistiques présent dans le groupe sera décrémenté.

Pour ajouter des informations sur la dépose du groupe ou voir le contenu du groupe, le fonctionnement est le même que lors de la prise.&#x20;

### Dépose une unité logistique contenue dans un groupe

Vous pouvez venir scanner une unité logistique qui est contenue dans un groupe.&#x20;

Pour cela, il faut que le groupe qui contient l'unité logistique soit en prise, et il faut venir scanner le QR Code ou Code-barre, ou taper le code dans "_Entrée manuelle ..._". Vous ne pouvez pas passer l'unité logistique contenue dans le groupe en dépose via la flèche.

L'unité logistique contenue dans le groupe viendra se placer dans la zone _DEPOSE_. A la validation du mouvement, elle sera enlevée du groupe. Le nombre d'UL contenue dans le groupe diminuera.&#x20;

### Valider la dépose de tous les objets scannés

Lorsque vous avez scanné tous les objets souhaités, appuyez sur <mark style="background-color:blue;">**VALIDER**</mark> pour déposer tous les objets.

Le numéro sur l'écran _**Mouvements**_ dans _Produits en prise_ diminuera alors.&#x20;

Vous pouvez retrouvez les mouvements créés sur la supervision sur la page _**Traçabilité | Mouvements.**_

{% hint style="info" %}
Un opérateur ne pourra pas se déconnecter de son terminal mobile s'il a toujours des objets en prise
{% endhint %}
