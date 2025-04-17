# Types et champs libres

Un type est une classification de vos entités qui vous permet de personnaliser votre application en fonction de votre contexte d'utilisation. Vous pouvez associer des champs libres à un type pour ajouter des informations supplémentaires propres à cette classification.

Dans un premier encadré, vous pouvez voir tous les types que vous avez créés. Le premier type est sélectionné par défaut, mais vous pouvez naviguer entre les différents types en cliquant sur leur libellé. Vous pouvez également créer un nouveau type en cliquant sur le bouton "Ajouter un type".

Sur le 2e encadré, vous avez la description du type et ces champs libres associés. Cliquez sur "**Modifier"** pour modifier l'ensemble des informations du type et de ces champs libres.

![](https://wiilog.gitbook.io/\~gitbook/image?url=https%3A%2F%2F806097355-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fid6mpmGgIXZ3CFWUO3AX%252Fuploads%252FWEDpjbUTkisXVCLMTebB%252Fimage.png%3Falt%3Dmedia%26token%3D32aaf412-012e-4e5d-9c02-e046855c0c2b\&width=768\&dpr=4\&quality=100\&sign=03f3f669f6bde2a61ee23998e7e7317a1ffb9b324dd3bb40174d7fc23f9a7684)

**Informations liées aux types** :

* **Description** : Ajoutez un complément d'information au type.
* **Couleur** : Vous pouvez associer une couleur à un type, elle apparaîtra dans la partie références et dans le panier. Un choix de 8 couleurs vous est proposé, en cliquant sur "Autre..." vous avez accès à un color picker pour choisir la couleur que vous voulez.

**Informations liés aux champs libres :**

* **Libellé** : Nom du champ libre, il doit être unique
* **S'applique à** : Vous avez le choix entre Article et Référence article, cela indiquera si votre champ libre doit apparaître au niveau de votre référence ou des articles de votre référence.
*   **Typage** :

    | Type           | Format                  | Exemple et détail                                                                                                                                       |
    | -------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | Date           | JJ/MM/AAAA              | 25/03/2022 : L'année peut être reprise facilement sous excel                                                                                            |
    | Texte          | texte de 250 caractères | Le texte peut être limité en affichage sur la taille des champs                                                                                         |
    | Oui/Non        | Coche                   | Article fragile : "Oui" ou "Non"                                                                                                                        |
    | Date et heure  | JJ/MM/AAAA HH:MM        | 25/03/2022 17:53                                                                                                                                        |
    | Liste          | Choix unique            | La donnée se sélectionne dans une liste et est disponible en import ou export via une valeur de la liste : "Valeur"                                     |
    | Liste multiple | Choix multiple          | La donnée se sélectionne dans une liste multiple et est disponible en import et export via une chaine avec séparateur point virgule : "Valeur1;Valeur2" |
    | Nombre         | NNNN                    | Exemple : 12345                                                                                                                                         |
* **Éléments** : Ce champ est disponible que pour les types : liste et liste multiple. Indiquez les valeurs qui vont se retrouver dans votre liste. Attention les mots doivent être séparés par des ";".
* **Nb caractères (Min)**: Le nombre de caractères minimum du champ.
* **Nb caractères (Max)**: Le nombre de caractères maximum du champ.
* **Valeur par défaut** : Ce champ est disponible pour tous les types sauf liste multiple. La valeur choisie s'affichera en permanence lors de la création d'article, vous pourrez évidement la changer.
* **Afficher à la création** : Cochez pour afficher ce champ libre à la création d'une référence.
* **Obligatoire à la création** : Cochez pour rendre ce champ obligatoire à la création d'une référence, l'utilisateur sera obligé de saisir cette donnée.
* **Affiché à la modification**: Cochez pour afficher ce champ libre à la modification d'une référence.
* **Obligatoire à la modification** : Cochez pour rendre ce champ obligatoire à la modification de la référence, l'utilisateur sera obligé de saisir cette donnée.

#### Ajouter un type <a href="#ajouter-un-type" id="ajouter-un-type"></a>

Cliquez sur le bouton "**Ajouter un type**", vous allez pouvoir remplir les informations et créer des champs libres si besoin.

Pour le type vous allez indiquer son **libellé**, sa **description** et sa **couleur**. Pour ajouter un champ libre cliqué sur la ligne "**+**" du tableau, cela vous ajoutera la ligne avec les champs à remplir décrits au-dessus. Ajouter de la même manière autant de ligne que souhaité.

Les éléments avec une astéries "\*" sont les champs obligatoire à remplir pour valider la création ou la modification.

#### Modifier un type et des champs libres <a href="#modifier-un-type-et-des-champs-libres" id="modifier-un-type-et-des-champs-libres"></a>

Si vous voulez modifier un type déjà créé, cliquez sur le type souhaité puis sur le bouton "**Modifier**" cela vous permettra de modifier le libellé, la description et la couleur du type. Vous allez aussi pouvoir changer les informations des champs libres et aussi en ajouter.

#### Supprimer un type <a href="#supprimer-un-type" id="supprimer-un-type"></a>

En mode modification vous pouvez supprimer le type et ces champs libres associés en cliquant sur la poubelle à coté du champ Libellé. **Attention, il est impossible de supprimer un type s'il est lié à des références.**

#### Ajouter des champs libres <a href="#ajouter-des-champs-libres" id="ajouter-des-champs-libres"></a>

Lors de la modification du type expliqué juste au dessus vous avez la possibilité d'ajouter des champs libres, pour cela, cliqué sur la dernière ligne du tableau avec un "**+**", cela vous ajoutera une ligne avec les champs à remplir décrites plus haut. Ajouter de la même manière autant de ligne que souhaité.

#### Supprimer un champ libre <a href="#supprimer-un-champ-libre" id="supprimer-un-champ-libre"></a>

Vous pouvez les supprimer des champs libres en cliquant sur la poubelle en début de ligne. **Attention : Il est très important de savoir que la suppression d'un champ est irréversible, les données saisies seront perdues.**

Penser à exporter vos données avant d'effectuer une éventuelle suppression de champ.
