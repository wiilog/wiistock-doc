# Détail réception

En cliquant sur une ligne de réception, vous arriverez sur le détail de la réception.

Le détail de la réception contient 3 zones :&#x20;

* L'**entête** de réception
* La **liste des articles**
* La [**liste des litiges**](litiges-qualite.md) (voir page suivante)

{% embed url="https://www.screencast.com/t/INhRR3BSp" %}
Détails d'une réception
{% endembed %}

## Entête de réception

L'entête de réception contient tous les différents champs renseignés sur le formulaire de création de réception.&#x20;

Elle va contenir également la mention _"Cette réception est URGENCE"_ si le switch _**Urgence**_ a été coché sur le formulaire de création de réception, ou la mention _"Une ou plusieurs références liées à cette réception sont urgentes"_ si une des références ajoutée à la réception est urgente (voir [Stock | Références](../../references.md) pour mettre une référence en urgence).&#x20;

Elle contient également les boutons suivants :&#x20;

* **Réception :** disponible seulement si la réception n'est pas en statut _Réception totale_. Ce bouton ouvre la modale de conditionnement des articles (voir explications plus bas sur le conditionnement)
* **Fin Réception :** disponible seulement si la réception n'est pas en statut _Réception totale_. Ce bouton sert à indiquer que la réception est terminée et ainsi à la passer en statut Réception totale. La date de fin est alors remplie avec l'horodatage de passage à ce statut
* **Modifier :** sous la flèche à droite de **Fin Réception**. Disponible seulement si la réception n'est pas en statut Réception totale. Ce bouton ouvre une modale permettant de modifier les champs fixes et libres de la réception. La modification des champs libres est soumise à des paramétrages ([Paramétrage | Stock | Réceptions | Champs fixes](broken-reference)). Ainsi, vous pouvez décider de ne pas rendre modifiable certains champs ou alors de les rendre obligatoires.&#x20;
* **Voir les demandes de livraison :** sous la flèche à droite de **Fin Réception**. Apparaît seulement si la réception à générer une ou des demandes de livraison. En cliquant dessus vous serez redirigé vers la liste des demandes de réceptions créées suite à la livraison
* **Supprimer :** sous la flèche à droite de **Fin Réception**. Disponible seulement si la réception n'est pas en statut _Réception totale._ Cliquez dessus pour supprimer la réception. Vous ne pouvez pas supprimer la réception si elle contient des articles, ils doivent être supprimés au préalable
* **Annuler cette réception** : sous la flèche. Disponible seulement si la réception est en statut _Réception totale_. Permet de passer la réception en Statut Réception partielle et de pouvoir la modifier à nouveau, et réceptionner des nouvelles références et/ou articles

## Liste des articles

La liste des articles contient :&#x20;

* La **recherche rapide** : pour chercher rapidement une référence
* Un bouton **Ajouter une référence** : pour ajouter des références à réceptionner
* Un bouton **Générer des étiquettes** : sous la flèche à droite de Ajouter une référence. Pour relancer une impression d'étiquette, de références ou d'articles
* Un **tableau**, regroupant les références à réceptionner / réceptionnées :&#x20;

| Colonne        | Description                                 |
| -------------- | ------------------------------------------- |
| **Référence**  | Référence à réceptionner / réceptionnée     |
| **Commande**   | Numéro de commande de la ligne de réception |
| **A recevoir** | Quantité de la référence à réceptionner     |
| **Reçu**       | Quantité réceptionnée                       |

Sur chaque ligne du tableau, un bouton<img src="../../../../.gitbook/assets/3points" alt="" data-size="line">donne accès à :&#x20;

* **Voir mouvements de traçabilité** : _bouton disponible seulement si des quantités ont déjà été réceptionnées et que la référence est une référence en gestion quantité référence_. Ce bouton redirige vers la page Traçabilité | Mouvements, avec le filtre _Colis_ remplis avec le code barre de la référence. La page des mouvements de traçabilité montre ainsi tous les mouvements de prise et dépose qu'il y a eu sur cette référence
* **Voir les articles** : _bouton disponible seulement si des quantités ont déjà été réceptionnées et que la référence est une référence en gestion quantité article._ Ce bouton ouvre une modale de tous les articles qui ont été créés suite à la réception. Nous décrirons cette modale plus bas dans l'explication du processus de réception
* **Imprimer** : _bouton disponible seulement si des quantités ont déjà été réceptionnées et que la référence est une référence en gestion quantité référence._ Pour lancer l'impression d'une étiquette de référence.&#x20;
* **Supprimer** : pour supprimer la ligne de réception. Dans le cas d'une référence en gestion quantité article sur laquelle vous avez déjà réceptionné des quantités, il faudra d'abord supprimer tous les articles générés suite à la réception avant de pouvoir supprimer la ligne de réception.

## Ajouter des références&#x20;

Pour ajouter des articles, cliquez sur le bouton <mark style="background-color:blue;">**Ajouter article**</mark> pour ouvrir la modale _**Ajouter une ligne**_. Sélectionner la référence pour faire apparaître tous les champs. Remplissez les champs suivants :&#x20;

* **Référence** : premier champ à remplir pour faire apparaître les autres champs. Tapez les premiers caractères pour rechercher la référence que vous souhaitez réceptionner. Si la référence que vous voulez réceptionner n'existe pas, vous pouvez créer une nouvelle référence en cliquant sur le + à droite de la référence.&#x20;
  * Si vous sélectionnez une référence en gestion quantité par article, un bouton <mark style="background-color:blue;">**Enregistrer et Réception**</mark> apparaîtra en bas
* **Numéro de commande d'achat** : numéro de commande de la référence à réceptionner. Si vous avez déjà renseigné un numéro de commande sur l'entête de réception, ce champ sera automatiquement rempli avec le numéro renseigné. Vous pouvez néanmoins mettre un numéro de commande différent sur la ligne de réception
* **Quantité à recevoir** : quantité à réceptionner de la référence
* **Quantité reçue** : champ indisponible. Par défaut à 0 à l'ajout de la ligne.&#x20;
* **Anomalie** : switch pour indiquer que la ligne de réception a une anomalie
* **Commentaire** : pour ajouter un commentaire sur la ligne de réception

{% embed url="https://www.screencast.com/t/jujQtdpNJbUn" %}
Ajouter une référence
{% endembed %}

## Réception d'articles (référence en gestion quantité article)

Si la référence ajoutée dans la liste des articles est une référence en gestion quantité par article, il faut passer par l'étape de réception des articles (conditionnement). Vous pouvez y accéder quand vous ajoutez une ligne de réception en cliquant sur <mark style="background-color:blue;">**Enregistrer et Réception**</mark>, ou alors en cliquant sur <mark style="background-color:blue;">**Réception**</mark> dans l'entête. Il faut alors remplir les champs suivants (nous verrons Demande de livraison et Demande de transfert plus bas) :&#x20;

* **Référence** : référence à réceptionner. Le champ est rempli du code de la référence - le numéro de commande de la ligne de réception
  * Si vous accédez à cette page via le bouton <mark style="background-color:blue;">**Enregistrer et Réception**</mark>, le champ _**Référence**_ est automatiquement rempli avec la référence et le numéro de commande indiqué sur la modale Ajouter article
  * Si vous accédez à cette page via le bouton <mark style="background-color:blue;">**Réception**</mark>, cliquez sur le champ pour afficher la liste des références sur lesquelles vous pouvez faire une réception d'articles. Cette liste va chercher dans les lignes de réception contenant des références en gestion par article dont la quantité reçue est inférieure à la quantité à recevoir
* **Référence fournisseur** : code de la référence chez le fournisseur. Tapez une première lettre pour aller sélectionner la référence fournisseur
* **Article(s)\*** : Renseigner le nombre d'article que vous avez à réceptionner, soit le nombre d'étiquettes qui sera imprimé
* **Quantité\*** : la quantité qu'il va y avoir dans chaque article

{% hint style="info" %}
Ainsi, ce nombre d'article \* quantité dans chaque article donnera la quantité totale réceptionnée.&#x20;
{% endhint %}

Par défaut, il sera renseigné dans le champ **Quantité** la quantité que vous avez renseigné dans **Quantité à recevoir** lors de l'ajout de référence. Vous pouvez évidemment changer les ces valeurs lors du conditionnement.

* **Lot** : numéro de lot de l'article
* **Date de péremption** : date de péremption de l'article
* **Champs libres** : si vous avez paramétré des champs libres qui s'appliquent sur l'article, ils apparaîtront ici

{% embed url="https://www.screencast.com/t/tvzeQ0N3Ll4" %}
Modale de conditionnement
{% endembed %}

Quand tous ces champs sont renseignés, cliquez sur <mark style="background-color:blue;">**Ajouter des articles**</mark> pour faire le conditionnement.&#x20;

Pour faire à un nouveau un conditionnement cliquer à nouveau sur <mark style="background-color:blue;">**Ajouter des articles**</mark>. Vous pouvez changer la référence, la référence fournisseur et les informations à réceptionner.

Il y aura ensuite une ligne par article. Chaque ligne contient 3 rectangles :&#x20;

{% embed url="https://www.screencast.com/t/5XQD2Z59lzPB" %}
Ligne article
{% endembed %}

Le 1er rectangle :

* **Article(s) :** le nombre d'article que vous avez à réceptionner

Le 2e rectangle :

* **Type** : Type de la référence de l'article qui va être créé
* **Référence** : Code de la référence de l'article qui va être créé
* **Nom** : Libellé de la référence de l'article qui va être créé
* **Référence fournisseur** : code de la référence chez votre fournisseur.

Le 3e rectangle reprend les informations renseignées au dessus

* **Quantité** : quantité renseignée dans le champ en haut. Quantité totale de l'article.&#x20;
* **Lot** : numéro de lot de l'article
* **Date de péremption** : date de péremption de l'article
* **Champs libres** : si vous avez paramétré des champs libres qui s'appliquent sur l'article
* Bouton **Supprimer** : vous pouvez supprimer le conditionnement

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> ensuite. La modale se fermera, et il se passera :&#x20;

* Génération d'étiquette pour chaque article créé
* Création des articles&#x20;
* Création de mouvements d'entrée en stock pour chaque article créé
* Incrémentation du stock de la référence
* Création des mouvements de traçabilité des articles
* Changement du nombre inscrit dans la colonne Reçu du tableau de la liste des articles par la quantité réceptionnée

{% hint style="info" %}
Vous ne pouvez pas réceptionner plus que la quantité indiquée dans A recevoir.
{% endhint %}

{% embed url="https://www.screencast.com/t/RpqBvlX3PmvW" %}
Processus de réception
{% endembed %}

Vous pouvez voir les articles réceptionnés en allant sur les<img src="../../../../.gitbook/assets/3points" alt="" data-size="line">de la ligne de réception que vous venez de réceptionner et en cliquant sur <mark style="background-color:blue;">**Voir les articles**</mark>. Une modale **Articles de référence** s'ouvrira alors. Elle contient un tableau avec les colonne suivantes :&#x20;

<table><thead><tr><th>Colonne</th><th width="420.5">Description</th></tr></thead><tbody><tr><td><strong>Code article</strong></td><td>Code barre de l'article créé</td></tr><tr><td><strong>Statut</strong></td><td>Statut de l'article créé (voir la description de la page <a href="../../articles.md">Articles </a>pour le statut)</td></tr><tr><td><strong>Libellé</strong></td><td>Libellé de la référence de l'article</td></tr><tr><td><strong>Référence article</strong></td><td>Code de la référence de l'article</td></tr><tr><td><strong>Quantité</strong></td><td>Quantité contenue dans l'article</td></tr></tbody></table>

Sur chaque ligne du tableau, vous pouvez accéder aux boutons via les<img src="../../../../.gitbook/assets/3points" alt="" data-size="line">:&#x20;

* **Imprimer** : lancer la génération d'une étiquette article
* **Accéder à la demande** : si lors de la réception des article cet article, une demande de livraison ou de transfert a été générée, ce bouton apparaîtra. Il permet d'accéder à la demande en question qui contient l'article
* **Voir mouvement de traçabilité** : ce bouton redirige vers la page Traçabilité | Mouvements, avec le filtre _Colis_ remplis avec le code barre de l'article. La page des mouvements de traçabilité montre ainsi tous les mouvements de prise et dépose qu'il y a eu sur cet article
* **Supprimer** : suppression de l'article. La suppression de l'article supprimera également tous les mouvements de stock lié à l'article, et les demandes liées si l'article a été mis dans une demande (livraison ou transfert)

En cliquant sur une ligne d'article, vous accédez à la modale de modification de l' article

### Demande de livraison via réception&#x20;

Pour mettre en livraison les articles que vous êtes en train de réceptionner, cliquer sur <mark style="background-color:blue;">**Livraison**</mark> dans la partie **Création d'une demande**. Vous pouvez faire en sorte que Livraison soit toujours sélectionné à l'ouverture de cette modale en allant cocher _"Créer une demande de livraison après réception"_ dans le paramétrage.

{% embed url="https://www.screencast.com/t/QEqIlGHQ" %}
Information demande de livraison
{% endembed %}

Les champs suivants apparaissent ensuite :&#x20;

* **Demandeur\*** : personne pour qui la demande est. Si vous souhaitez que par défaut ce champ soit rempli avec l'utilisateur de la session en cours, allant activer le paramétrage _"Le demandeur est l'utilisateur de la session en cours"_.
* **Type\*** : type de la livraison
* **Destination\*** : emplacement de livraison. Cet emplacement peut être rempli automatiquement selon plusieurs paramétrages&#x20;
  * Le demandeur a une drop zone associée : la destination est remplie automatiquement avec la dropzone de l'utilisateur
  * Le type de la livraison a un emplacement par défaut : la destination est remplie automatiquement avec l'emplacement par défaut associé à ce type de livraison
* **Champs libres** : champs libres du type de la demande de livraison
* **Commentaire** : commentaire sur la demande de livraison

Lorsque vous avez fini votre conditionnement et que vous cliquez sur <mark style="background-color:blue;">**Enregistrer.**</mark> Selon votre paramétrage la demande de livraison aura différent impact.&#x20;

Dans le [paramétrage](broken-reference) des demandes de livraison vous avez 3 choix :

* **Création seulement de la demande de livraison en "A traiter"** : Il est possible que la demande de livraison soit créée sans une préparation en suivant.
* **Création de la demande de livraison avec sa préparation** : la demande sera automatiquement créée au statut A traiter avec l'ordre de préparation associé aussi au statut À traiter.
* **Livraison directe : passage direct à l'ordre de livraison** : la demande de livraison se crée, l'ordre de préparation généré soit directement au statut Préparé et ainsi qu'un ordre de livraison soit automatiquement généré au statut A traiter. Cela permet ainsi d'éviter l'étape de préparation

### Demande de transfert via réception

Pour faire une demande de transfert des articles réceptionnés automatiquement vers leur emplacement de transfert suite à la réception, sélectionner <mark style="background-color:blue;">**Transfert**</mark>.&#x20;

{% embed url="https://www.screencast.com/t/GsrkwPPt2G" %}
Information demande de transfert
{% endembed %}

Les champs suivants apparaitront :&#x20;

* **Emplacement de stockage** : emplacement de destination de la demande de transfert. Si vous avez renseignez le champ Emplacement de stockage sur l'entête de réception, ce champ sera rempli automatiquement avec l'emplacement renseigné
* **Emplacement d'origine** : emplacement d'origine de la demande de transfert. Ce champ sera rempli automatiquement avec l'emplacement de réception

Lorsque vous avez fini votre conditionnement et que vous cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>, la demande de transfert sera automatiquement créée au statut A traiter avec l'ordre de transfert associé et contiendra les articles générés.

## Réception de références (référence en gestion quantité référence)

Après avoir ajouter votre référence en gestion quantité référence dans le tableau des articles, cliquez sur la ligne de votre référence. La modale Modifier une ligne de réception s'ouvrira alors avec le champ _**Quantité reçue**_ disponible cette fois-ci. Renseignez la quantité reçue et cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark>.&#x20;

{% embed url="https://www.screencast.com/t/8I5MeZiFj" %}
Réception d'une référence
{% endembed %}

Il sera alors créé :&#x20;

* Un mouvements d'entrée en stock de la quantité indiquée pour la référence
* Une incrémentation du stock de la référence
* Un mouvement de traçabilité de la référence
* Changement du nombre inscrit dans la colonne Reçu du tableau de la liste des articles par la quantité réceptionnée
