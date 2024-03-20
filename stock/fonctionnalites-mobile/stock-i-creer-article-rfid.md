# Stock I Créer Article (RFID)

## Présentation RFID

La RFID ou encore la **Radio Frequency Identification** est une technologie permettant sauvegarder et récupérer des données à distance sur ce que l’on appelle ici des **tags RFID**. La technologie RFID repose sur des **transferts d’énergie par électromagnétisme**. Pour mettre en application sur notre application Wiilog, il est nécessaire de **disposer tags RFID et d’un lecteur RFID.**

\-        Le lecteur RFID émet des radiofréquences activant les tag RFID qui passent à proximité. Pour il leur envoie à coutre distance l’énergie nécessaire.

<figure><img src="../../.gitbook/assets/image (26).png" alt="" width="375"><figcaption></figcaption></figure>

\-        Les radio-étiquettes sont dites passives car elles utilisent uniquement l’énergie fournie par le lecteur. En fonction de la configuration du lecteur, elles peuvent être lues à une distance allant de 200 mètres. Ces étiquettes RFID peuvent contenir plusieurs types d’informations : identification, base de données.

<div data-full-width="false">

<figure><img src="../../.gitbook/assets/image (28).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

### Pour qui ?&#x20;

L’application de cette fonctionnalité RFID sur Wiilog conviendrait notamment aux industriels utilisant actuellement le **processus DLF (Direct Line Feed)** qui est un **mode d’approvisionnement dans lequel la détection des besoins de réapprovisionnement est réalisée par le fournisseur.**

### Comment ?

Notre **processus RFID s’applique avec les fournisseurs en charge de générer et d’imprimer les étiquettes RFID pré encodées avec une préfixe standard**, ainsi que leur datamatrix contenant informations suivantes (solution actuelle + bin).

### Pourquoi ?&#x20;

Pour résumer, la réalisation de création d'article et d’un inventaire automatique avec la technologie RFID vous permettra de réduire considérablement le temps de vos réceptions et inventaires.&#x20;

&#x20;Votre inventaire sera plus précis également, et avec le développement supplément que nous avons ajouté il vous sera possible d’avertir vos fournisseurs automatiquement par mail du besoin d’approvisionnement.

## Processus de création d'article RFID

Cette nouvelle fonctionnalité de création d’article RFID a été pensée pour un processus rapide et de masse de création d’article lors d’une réception. Nous avons intégré une nouvelle page des paramètres par défaut dans **Paramétrage | Stock | Articles | Création nomade RFID** afin de ne pas avoir à saisir tous les champs obligatoires pour une création d’article.&#x20;

<figure><img src="../../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

Liste des champs par défaut paramétrables :&#x20;

* **Type de la référence**
* **Référence** : Code de la référence
* **Libellé** de la référence
* **Quantité** de la référence
* **Fournisseur de la référence**
* **Référence fournisseur**
* **Emplacement de destination :** Un emplacement de destination par défaut peut être paramétré par défaut, mais **cette donnée peut être écrasée et remplacée par l'emplacement de destination indiqué sur le datamatrix.**&#x20;

C'est dans le sous menu **Stock | Créer article** que vous pourrez appliquer ces paramétrages par défaut et donc de **créer des articles que l’on va associé à des tag RFID**, qui par la suite seront **reliés à un datamatrix**.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Pour associer un tag RFID à un article, il vous suffit sur cet écran de **Balayer une étiquette RFID** soit en **utilisant la gachette** ou par **entrée manuelle** en cas de problème de détection. Dès l’appuie de la gachette, le scan RFID est lancé.

Dès lors que le scan à détecter un tag RFID sur votre étiquette, vous serez dirigé vers un formulaire de création d’article avec les champs pré remplis en fonction du paramétrage par défaut.&#x20;

<figure><img src="../../.gitbook/assets/image (21).png" alt="" width="384"><figcaption></figcaption></figure>

En scrollant en page de l’écran, vous verrez apparaître des nouveaux champs donnant plus d’informations sur l’article. Vous pourrez soit les saisir manuellement, ou à l’appui du bouton <mark style="background-color:blue;">**Scan 2D**</mark>, les faire remplir automatiquement en scannant un QR Code associé à un datamatrix.&#x20;

![](<../../.gitbook/assets/image (12).png>)![](<../../.gitbook/assets/image (48).png>)

Nous avons pris un modèle de datamatrix qui renseigne les informations suivantes :&#x20;

* **Prix unitaire**
* **Date de péremption**
* **Numéro de lot**
* **Numéro de commande**
* **Ligne de bon de livraison**&#x20;
* **Pays d'origine** : Dans **Paramétrage | Stock | Articles | Pays d'origine**, il vous renseigner le(s) pays d'origine(s)  dans le tableau.
* **Date de production**
* **Commentaire**

Ainsi, lorsque vous aurez scanné votre datamatrix, votre article est créé, enrichit des nouvelles informations issu du datamatrix et vous serez redirigé sur l’écran de balayage d’étiquette RFID pour en recréer d’autres.

Pour avoir de la visibilité, en vous connectant l’application sur le web, dans **Stock | Articles,** vous pourrez retrouver votre article en faisant une **recherche rapide avec votre TAG RFID** par exemple. Vous verrez apparaître la ligne de votre article, avec son **statut en disponible** et sa **date d’entrée en stock**. Puis en rentrant dans le détail de l’article, vous verrez apparaître les nouveaux champs dans l'encart Description complété par les informations du datamatrix.&#x20;

Enfin sur la timeline de ses mouvements de traçabilité, vous verrez apparaître un **mouvement de dépose** de l’article sur l’emplacement concerné. Et dans Stock | Mouvements de stock, une **entrée en stock** de votre article.&#x20;
