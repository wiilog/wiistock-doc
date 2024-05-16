# Articles

## Étiquettes

Indiquez ce que vous voulez afficher sur les étiquettes des articles. Pour paramétrer le format de l'étiquette retourner dans le paramétrage "Global".

Vous avez la possibilité d'afficher sur l'étiquette :

* **Afficher l'emplacement** de destination ou dropzone (un des 2 choix possible)
  * **Destination** : Destination de l'article, cette information apparait sur l'étiquette si l'article est lié à une demande de livraison&#x20;
  * **Dropzone** : liée à la dropzone paramétrée sur l'utilisateur qui fait la demande de livraison sur la réception
* **Afficher date de péremption** : pour afficher la date de péremption renseignée sur les articles au moment du conditionnement
* **Afficher la date d'entrée en stock** : pour afficher la date à laquelle l'article est entrée en stock
* **Afficher le destinataire :** pour afficher le nom de la personne ayant effectué une demande de livraison sur cet article suite à la réception
* **Afficher la quantité** : affiche la quantité contenue dans l'article
* **Afficher le numéro de lot :** pour afficher le numéro de lot renseigné sur les articles au moment du conditionnement
* **Un champ libre** : vous pouvez afficher un champ libre sur l'étiquette. Ce champ libre se choisit parmi tous les champs libres paramétrés sur les articles

![Étiquette d'article (via réception)](../../.gitbook/assets/ETQ\_articles\_reception.png)

**Dans l'ordre d'apparition :**

QR code (ou barre code)\
Code barre article\
Destinataire / emplacement de destination (ou dropzone)\
L/R : Libellé de la référence\
C/R : Code référence\
L/A : Libellé de l'article\
Numéro de lot\
Date de péremption\
Quantité\
Champs libre&#x20;

##

## Champs fixes

Contrairement aux champs libres, les champs fixes ne peuvent ni être supprimés, ni ajoutés. Vous pouvez paramétrer leur visibilité ou leur caractère obligatoire.

Les champs fixes suivants sont disponibles à la création et / ou édition d'un article. Vous pouvez sélectionner si vous souhaitez juste les "Afficher" ou bien les rendre "Obligatoires".

* Anomalie
* Commentaire
* Date de fabrication
* Date de péremption
* Date de production
* Ligne bon de livraison
* Ligne commande d'achat
* Lot
* Pays d'origine
* Prix unitaire



## Types et champs libres

Un type est une classification de vos entités. Vous pouvez associer à un type des champs libres afin d'apporter des informations supplémentaires propres à cette classification. Cela vous permet de personnaliser votre application pour votre contexte d'utilisation.&#x20;

Dans un premier encadré, vous avez tous les **types** que vous avec créé, par défaut le 1er type est sélectionné, pour naviguer entre les différents types cliquer sur le libellé. Vous avez la possibilité d'en créer un nouveau en cliquant sur le bouton "<mark style="background-color:blue;">**Ajouter un type**</mark>".

Sur le 2e encadré, vous avez la description du type et ces champs libres associés. Cliquez sur "<mark style="background-color:blue;">**Modifier**</mark>**"** pour modifier l'ensemble des informations du type et de ces champs libres.

<figure><img src="../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

**Informations liées aux types** :

* **Description** : Ajoutez un complément d'information au type.
* **Couleur** : Vous pouvez associer une couleur à un type, elle apparaîtra dans la partie références et dans le panier. Un choix de 8 couleurs vous est proposé, en cliquant sur "Autre..." vous avez accès à un color picker pour choisir la couleur que vous voulez.

**Informations liés aux champs libres :**

* **Libellé** : Nom du champ libre, il doit être unique
* **S'applique à** : Vous avez le choix entre Article et Référence article, cela indiquera si votre champ libre doit apparaître au niveau de votre référence ou des articles de votre référence.
*   **Typage** :&#x20;

    <table><thead><tr><th width="150">Type</th><th width="150">Format</th><th>Exemple et détail</th></tr></thead><tbody><tr><td>Date</td><td>JJ/MM/AAAA</td><td>25/03/2022 : L'année peut être reprise facilement sous excel</td></tr><tr><td>Texte</td><td>texte de 250 caractères</td><td>Le texte peut être limité en affichage sur la taille des champs</td></tr><tr><td>Oui/Non</td><td>Coche</td><td>Article fragile : "Oui" ou "Non"</td></tr><tr><td>Date et heure</td><td>JJ/MM/AAAA HH:MM</td><td>25/03/2022 17:53</td></tr><tr><td>Liste</td><td>Choix unique</td><td>La donnée se sélectionne dans une liste et est disponible en import ou export via une valeur de la liste : "Valeur"</td></tr><tr><td>Liste multiple</td><td>Choix multiple</td><td>La donnée se sélectionne dans une liste multiple et est disponible en import et export via une chaine avec séparateur point virgule : "Valeur1;Valeur2"</td></tr><tr><td>Nombre</td><td>NNNN</td><td>Exemple : 12345</td></tr></tbody></table>
* **Éléments** : Ce champ est disponible que pour les types : liste et liste multiple. Indiquez les valeurs qui vont se retrouver dans votre liste. Attention les mots doivent être séparés par des ";".
* **Nb caractères (Min)**: Le nombre de caractères minimum du champ.
* **Nb caractères (Max)**: Le nombre de caractères maximum du champ.
* **Valeur par défaut** : Ce champ est disponible pour tous les types sauf liste multiple. La  valeur choisie s'affichera en permanence lors de la création d'article, vous pourrez évidement la changer.
* **Afficher à la création** : Cochez pour afficher ce champ libre à la création d'une référence.
* **Obligatoire à la création** : Cochez pour rendre ce champ obligatoire à la création d'une référence, l'utilisateur sera obligé de saisir cette donnée.
* **Affiché à la modification**: Cochez pour afficher ce champ libre à la modification d'une référence.
* **Obligatoire à la modification** : Cochez pour rendre ce champ obligatoire à la modification de la référence, l'utilisateur sera obligé de saisir cette donnée.

### Ajouter un type

Cliquez sur le bouton "<mark style="background-color:blue;">**Ajouter un type**</mark>", vous allez pouvoir remplir les informations et créer des champs libres si besoin.

Pour le type vous allez indiquer son **libellé**, sa **description** et sa **couleur**. Pour ajouter un champ libre cliqué sur la ligne "**+**" du tableau, cela vous ajoutera la ligne avec les champs à remplir décrits au-dessus. Ajouter de la même manière autant de ligne que souhaité.

{% hint style="info" %}
Les éléments avec une astéries "\*" sont les champs obligatoire à remplir pour valider la création ou la modification.
{% endhint %}

### Modifier un type et des champs libres

Si vous voulez modifier un type déjà créé, cliquez sur le type souhaité puis sur le bouton "<mark style="background-color:blue;">**Modifier**</mark>" cela vous permettra de modifier le libellé, la description et la couleur du type. Vous allez aussi pouvoir changer les informations des champs libres et aussi en ajouter.

### Supprimer un type

En mode modification vous pouvez supprimer le type et ces champs libres associés en cliquant sur la poubelle à coté du champ Libellé. **Attention, il est impossible de supprimer un type s'il est lié à des références.**

### Ajouter des champs libres

Lors de la modification du type expliqué juste au dessus vous avez la possibilité d'ajouter des champs libres, pour cela, cliqué sur la dernière ligne du tableau avec un "**+**", cela vous ajoutera une ligne avec les champs à remplir décrites plus haut. Ajouter de la même manière autant de ligne que souhaité.

### Supprimer un champ libre

Vous pouvez les supprimer des champs libres en cliquant sur la poubelle en début de ligne. **Attention : Il est très important de savoir que la suppression d'un champ est irréversible, les données saisies seront perdues.**

Penser à exporter vos données avant d'effectuer une éventuelle suppression de champ.



## Création nomade RFID

