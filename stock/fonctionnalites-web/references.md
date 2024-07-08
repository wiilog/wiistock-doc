# Références

Cette page est disponible dans le menu **Stock**, puis **Références**. Cette page contient plusieurs éléments :&#x20;

* Une **zone de filtre paramétrable**
* Une **recherche rapide**, permettant de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Nouvel article de référence**</mark> pour créer un nouvel article&#x20;
* Un bouton <mark style="background-color:blue;">**Impression des étiquettes**</mark>, sous le bouton Nouvel article de référence, pour imprimer les étiquettes des références. Ce bouton n'est disponible qu'après une recherche rapide
* Un bouton <mark style="background-color:blue;">**Gestion des colonnes**</mark>, sous le bouton Nouvel article de référence, pour gérer les colonnes affichées à l'écran
* Un bouton <mark style="background-color:blue;">**Recherche rapide**</mark>**,** pour choisir dans quelles colonnes la recherche rapide va chercher
* Un **tableau**, regroupant les différentes références

{% embed url="https://www.screencast.com/t/NSI6msZnrlJ" %}
Page des références
{% endembed %}

**Contenu des filtres**

La zone des filtres des références est différente des autres filtres de l'application. Pour appliquer un filtre sur le tableau des références, cliquez sur <mark style="background-color:blue;">**Ajouter un filtre**</mark>.

Une modale s'ouvre alors. Sélectionnez alors le champ sur lequel vous souhaitez filtrer. En fonction de la nature du champ, vous serez amener à renseigner la valeur différemment :&#x20;

* _Contient_ : tapez un texte. A l'application du filtre, le filtre ira chercher toutes les valeurs contenant l'ensemble de caractères tapé dans la colonne choisie
* _Valeur_ : tapez quelques lettres ou cliquez dans le champ pour choisir le filtre parmi un ensemble de valeurs déjà définies ou dans la liste d'un référentiel&#x20;
* _Date_ : le champ sur lequel vous souhaitez filtrer est une date. Tapez la date souhaitée pour avoir seulement les références avec la date indiquée
* _Date et heure_ : le champ sur lequel vous souhaitez filtrer est une date et une heure
* _Oui/Non_ : champ de type oui ou non. Cochez pour avoir les valeurs en oui, ne cochez pas pour les valeurs en non

Cliquez sur <mark style="background-color:blue;">**Appliquer**</mark> pour filtrer le tableau. Le filtre se positionne alors dans la zone de filtre. Cliquez sur la croix à droite de l'étiquette de filtre pour enlever le filtre

### Contenu du tableau

Toutes les colonnes sont décrites, à vous de choisir celles qui vous souhaitez avoir à l'écran via la gestion des colonnes

Vous pouvez choisir l'ordre des colonnes par glisser-déposer.&#x20;

| Colonne                      | Description                                                                                                                                                                                                                                                                                                                                           |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Image**                    | Image de la référence paramétrée                                                                                                                                                                                                                                                                                                                      |
| **Libellé**                  | Libellé de la référence                                                                                                                                                                                                                                                                                                                               |
| **Référence**                | Code de la référence                                                                                                                                                                                                                                                                                                                                  |
| **Code barre**               | Code barre de la référence                                                                                                                                                                                                                                                                                                                            |
| **Urgence**                  | Référence en urgence, disponible seulement pour les références en gestion quantité à l'article                                                                                                                                                                                                                                                        |
| **Type**                     | Type de la référence                                                                                                                                                                                                                                                                                                                                  |
| **Statut**                   | <p>Statut de la référence . La référence peut avoir ces statuts : <br>- <em>Brouillon</em> : la référence est en brouillon, elle ne peut pas être utilisée<br>- <em>Actif</em> : la référence peut être utilisée <br>- <em>Inactif</em> : la référence n'est plus utilisée sur votre instance. Elle ne peut plus être utilisée dans l'application</p> |
| **Quantité stock**           | Quantité en stock de la référence                                                                                                                                                                                                                                                                                                                     |
| **Quantité disponible**      | Quantité disponible de la référence (quantité non demandée sur des demandes de livraison ou transfert)                                                                                                                                                                                                                                                |
| **Acheteur**                 | Acheteur de la référence                                                                                                                                                                                                                                                                                                                              |
| **Emplacement**              | Emplacement de stockage de la référence, pour les références gérées en quantité à la référence                                                                                                                                                                                                                                                        |
| **Seuil de sécurité**        | Seuil de quantité qui déclenche une première alerte                                                                                                                                                                                                                                                                                                   |
| **Seuil d'alerte**           | Seuil de quantité qui déclenche une dernière alerte                                                                                                                                                                                                                                                                                                   |
| **Prix unitaire**            | Prix d'une quantité de la référence. Pour les inventaires                                                                                                                                                                                                                                                                                             |
| **Synchronisation nomade**   | Oui ou Non. Si la référence est synchronisée, il est possible de faire des demandes de livraison dessus à partir du nomade                                                                                                                                                                                                                            |
| **Nom fournisseur**          | Nom des fournisseurs de la référence                                                                                                                                                                                                                                                                                                                  |
| **Code fournisseur**         | Code des fournisseurs de la référence                                                                                                                                                                                                                                                                                                                 |
| **Dernier inventaire**       | Date de dernier inventaire de la référence, pour les références en gestion quantité référence                                                                                                                                                                                                                                                         |
| **Gestion de stock**         | Gestion de stock de la référence. FIFO ou FEFO. Disponible seulement pour les références en gestion quantité Article                                                                                                                                                                                                                                  |
| **Gestionnaire(s)**          | Gestionnaires de la référence. Ils recevront des mails en cas de seuil atteint ou d'alerte de péremption                                                                                                                                                                                                                                              |
| **Commentaire**              | Commentaire sur la référence                                                                                                                                                                                                                                                                                                                          |
| **Commentaire d'urgence**    | Commentaire qui apparaitra sur la réception si la référence est en urgence. Disponible seulement pour les références en gestion quantité par article                                                                                                                                                                                                  |
| **Créée** **le**             | Date de création de la référence                                                                                                                                                                                                                                                                                                                      |
| **Créée par**                | Utilisateur ayant créé la référence                                                                                                                                                                                                                                                                                                                   |
| **Dernière modification le** | Date de dernière modification de la référence                                                                                                                                                                                                                                                                                                         |
| **Dernier modification par** | Utilisateur ayant effectué la dernière modification sur la référence                                                                                                                                                                                                                                                                                  |
| **Dernière entrée le**       | Date du dernier mouvement d'entrée en stock pour la référence                                                                                                                                                                                                                                                                                         |
| **Dernière sortie** **le**   | Date du dernier mouvement de sortie de stock de la référence                                                                                                                                                                                                                                                                                          |
| **Groupe de visibilité**     | Groupe de visibilité de la référence                                                                                                                                                                                                                                                                                                                  |

2 légendes sont également présentes en haut du tableau :&#x20;

* **Demande d'achat en cours** : les références de cette couleur sont dans une demande d'achat non clôturée
* **En attente de réception** : les références de cette couleur sont dans une réception et les quantités à recevoir n'ont pas encore été reçues

### Ajouter une nouvelle référence

Pour créer une nouvelle référence, cliquez sur <mark style="background-color:blue;">**Nouvel article de référence**</mark> pour ouvrir une nouvelle page permettant de créer une référence.&#x20;

{% embed url="https://www.screencast.com/t/FvsHrORmi" %}
Page de création d'une référence
{% endembed %}

Remplissez les différents champs de la façon suivante :&#x20;

**Zone Référence**

* **Image** : cliquez sur le bouton avec le stylo pour aller chercher dans votre explorateur de fichier une image correspond à la référence
* **Référence\*** : rentrez le code de votre référence&#x20;
* **Libellé\*** : rentrez le libellé de la référence
* **Type\*** : type de la référence. Des types de référence doivent avoir été au préalable paramétrés (dans [Paramétrage > Stock > Articles > Types & champs libres](broken-reference)). Le choix du type donnera une couleur à la référence si vous avez attribué des couleurs lors du paramétrage de vos types
* **Statut\*** : état de la référence. 3 statuts possibles :&#x20;
  * **Brouillon** : ce statut sert principalement si une personne a des droits de création de référence seulement en brouillon. Ainsi, quand la référence sera créée, elle pourra être créée seulement en brouillon et ne pourra pas être utilisée dans le reste de l'application tant qu'un valideur de référence ne l'aura pas passée en statut Actif. Une création en brouillon d'une référence envoi un mail aux personnes ayant un rôle contenant le droit _Valideur de référence_. Si vous sélectionnez le statut _Brouillon_, les champs suivants seront remplis avec les informations suivantes sans pouvoir les modifier :&#x20;
    * **Référence** : le champ sera rempli avec la valeur ADEFINIRn, n étant le nombre de référence ayant déjà leur code en ADEFINIRn, +1
    * **Emplacement**, pour les **références en gestion quantité à la référence** : le champ sera rempli avec l'emplacement paramétré (dans [Stock > Configurations](../../parametrages/stock/configurations.md))
    * **Quantité**, pour les **références en gestion quantité à la référence** : le champ sera rempli par 0
  * **Synchronisation nomade** : cochez cette case afin de pouvoir des demandes de livraison hors ligne à partir du terminal mobile

**Zone Informations**

* **Groupe de visibilité** : associez un groupe de visibilité à la référence afin que seul les utilisateurs ayant ce groupe attribué puisse la voir dans la liste des références. Les groupes de visibilité se paramètrent dans [Stock > Paramétrage > Groupe de visibilité](broken-reference)
* **Pièces jointes** : pour associer des documents à la référence
* **Nomenclature :** pour mettre un commentaire sur la référence &#x20;

**Zone Gestion quantité**

Dans cette zone, les champs ne sont pas les mêmes selon si l'on choisit la gestion quantité à la référence et l'article.

**Gestion quantité à la référence** : ce mode de gestion permet de gérer de manière globale une référence sans distinguer de manière unique chaque pièce de la référence. Toute la quantité de la référence sera alors stockée sur un seul et même emplacement. Les champs disponibles pour cette gestion de quantité sont :&#x20;

* **Emplacement\*** : emplacement de stockage de la référence
* **Quantité\*** : quantité totale de la référence
* **Gestionnaires** : gestionnaires de la référence. Ils recevront un mail dans le cas où l'envoi de mail est paramétré lorsque le seuil d'alerte ou de sécurité est atteint
* **Acheteur** : acheteur en charge de la référence. Pour faire les demandes d'achat&#x20;
* **Prix unitaire (€)** : prix de chaque unité de la référence. Ce prix est utilisé ensuite pour le calcul de fiabilité monétaire sur les composants de dashboard correspondant (Voir [Dashboard > Liste des composants)](../../parametrages/dashboards/liste-des-composants/)
* **Seuil d'alerte** : premier seuil d'alerte de quantité. Si le seuil est atteint, une alerte est déclenchée dans la page Stock > Alerte et un mail est envoyé au gestionnaire si le paramétrage est activé
* **Seuil de sécurité** : deuxième seuil d'alerte de quantité. Si le seuil est atteint, une alerte est déclenchée dans la page Stock > Alerte et un mail est envoyé au gestionnaire si le paramétrage est activé

{% embed url="https://www.screencast.com/t/PDOCmJSRdDPi" %}

**Gestion quantité à l'article** : ce mode de gestion permet de gérer de manière unique chaque élément ou conditionnement de la référence. Il est possible ainsi de stocker des pièces de la référence à plusieurs endroits, d'indiquer des dates de péremption ou des numéros de lot sur les différents articles de la référence. Les champs disponibles pour cette gestion de quantité sont :&#x20;

* **Gestionnaires** : même fonctionnement que sur la gestion quantité à la référence. Dans le cas de la gestion à l'article, le gestionnaire peut aussi recevoir un mail d'alerte de péremption
* **Acheteur** : même fonctionnement que sur la gestion quantité à la référence
* **Gestion de stock** : 2 modes de gestion de stock sont disponibles
  * **FIFO** : _First in first out_. L'article qui a la date d'entrée en stock la plus ancienne est choisi en priorité pour être sorti du stock
  * **FEFO** : _First expired first out_. L'article qui a la date de péremption la plus proche est choisi en priorité pour être sorti du stock
* **Seuil d'alerte** : même fonctionnement que sur la gestion quantité à la référence
* **Seuil de sécurité** : même fonctionnement que sur la gestion quantité à la référence
* **Urgence** : cochez cette case pour indiquer que vous attendez en urgence cette référence. Sur la prochaine réception qui contiendra la référence, il y aura alors la mention de l'urgence à l'ajout de la référence sur la réception, et sur le détail de la réception, et la ligne de réception de la référence sera en rouge
* **Commentaire de l'urgence**, apparaît seulement quand **Urgence est coché** : pour indiquer plus d'information sur l'urgence. Le commentaire apparaîtra lors de l'ajout de la référence sur une réception, et au survol de la ligne de réception en urgence

{% embed url="https://www.screencast.com/t/x9iDgQb1ItQ" %}

**Zone Fournisseurs**

Vous devez ajouter au moins un fournisseur de la référence. Il est possible de mettre plusieurs fournisseurs pour une même référence. Pour cela, cliquez sur <mark style="background-color:blue;">**Ajouter un article fournisseur**</mark>

Pour ajouter un fournisseur, il faut remplir :&#x20;

* **Nom fournisseur\*** : va chercher dans la liste des fournisseurs. A la sélection du nom, le code se remplit automatiquement
* **Code fournisseur\*** : va chercher dans la liste des codes fournisseurs. A la sélection du code, le nom se remplit automatiquement
* **Ref article fournisseur\*** : code de la référence article chez le fournisseur
* **Libellé**\* : libellé de la référence article chez le fournisseur&#x20;

**Zone Inventaires**&#x20;

* **Catégorie d'inventaire** : ce champ va chercher dans la liste des catégories d'inventaire paramétrées ([Paramétrage > Stock > Inventaires](broken-reference)). Attribuer une catégorie d'inventaire à une référence permet de générer automatiquement des missions d'inventaire en fonction de la fréquence associée à la catégorie. Exemple : si la fréquence est de 2 mois et que la date de dernier inventaire de la référence est supérieure à 2 mois, la référence sera placée sur la prochaine mission d'inventaire générée. Les missions sont générées chaque dimanche soir. Dans le cas d'une référence en gestion quantité article, on vient regarder la date de dernier inventaire de chaque article, et si cette dernière est supérieure à la fréquence, l'article est placé dans la prochaine mission d'inventaire

**Zone Champs libres**

Les champs libres apparaissent en fonction du type de la référence sélectionné. Complétez les au besoin

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider la création de la référence

{% hint style="info" %}
Si vous avez créé la référence en statut _Brouillon_, un mail sera envoyé aux personnes ayant un rôle qui a le droit _Valideur de références_ coché pour l'informer qu'une référence est à valider.&#x20;
{% endhint %}

### Visualiser une référence

Vous pouvez visualiser une référence en cliquant sur la ligne de la référence souhaitée.&#x20;

Le détail de la référence s'ouvrira alors.&#x20;

{% embed url="https://www.screencast.com/t/UAfYPrsYT5F" %}
Visualistion d'une référence
{% endembed %}

Les champs sont les mêmes qu'à la création. Certains champs apparaissent en plus :&#x20;

**Zone Référence**

* **Quantité disponible** : quantité en stock de la référence qui n'est pas bloquée dans une demande de livraison ou de transfert

**Zone Informations**

* **Créée par** : utilisateur ayant créé la référence et horodatage de création (si vous n'avez pas d'utilisateur et/ou d'horodate de création, cela signifie que votre référence a été créée avant la mise en place de cette fonctionnalité)
* **Dernière modification par** : dernier utilisateur ayant modifié la référence et horodatage de la modification&#x20;
* **Dernier entrée le** : date et heure du dernier mouvement d'entrée en stock. Cela peut correspondre à une réception ou une collecte&#x20;
* **Dernière sortie le** : date et heure du dernier mouvement de sortie de stock. Cela correspond à une livraison

**Zone Gestion quantité**

* **Quantité en stock** : quantité totale en stock de la référence

**Zone Prévision de stock**

Cet encart vous permet de connaître à un instant T votre quantité en stock (quantité disponible) et son évolution dans le futur à 1 mois, 3 mois ou 6 mois. La courbe évolue en fonction des demandes de livraison ou des réception que vous effectuez sur cette référence.

<figure><img src="../../.gitbook/assets/Capture d’écran 2022-09-20 à 17.19.48.png" alt=""><figcaption><p>Prévision de stock</p></figcaption></figure>

**Zone Inventaires**

* **Date de dernier inventaire** : dernière date d'inventaire de la référence. Pour les références en gestion quantité article, cette date ne sera jamais remplie car la date de dernier inventaire est portée par les articles de la référence
* **Catégorie d'inventaire :** Indique la catégorie d'inventaire de cette référence [(paramètrage > stock > inventaire)](broken-reference)
*   **Inventaire à jour** : Dans le cas d'une référence en Gestion quantité par article, remplacer le champ "Date de dernier inventaire" est remplacé pour le champ "Inventaire à jour"

    Inventaire à jour :

    * si date d'aujourd'hui - date de dernière inventaire la plus ancienne parmi les articles de la référence < fréquence, alors OUI
    * si date d'aujourd'hui - date de dernière inventaire la plus ancienne parmi les articles de la référence > fréquence, alors NON

### Modifier une référence

Pour modifier une référence, 2 chemins :&#x20;

* Dans la liste des références, cliquez sur les ![](<../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>) d'une ligne de référence et cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> pour être redirigé vers la page de modification de référence
* Sur la visualisation d'une référence, cliquez sur <mark style="background-color:blue;">**Modifier**</mark> pour que la page passe en mode modification

L'utilisateur doit avoir le droit de modification pour voir apparaître les boutons <mark style="background-color:blue;">**Modifier**</mark>.&#x20;

Vous pouvez modifier :

* La **photo**
* La **référence**&#x20;
* Le **libellé**
* Le **statut**. Si une référence n'est plus en statut Brouillon, il n'est plus possible de la repasser sur ce statut
* La **synchronisation nomade**&#x20;
* Le **groupe de visibilité**
* Les **pièces jointes**
* La **nomenclature**
* Les **gestionnaires**
* L'**acheteur**
* La **gestion de stock**, pour les _**références en gestion quantité à l'article**_
* Le **prix unitaire (€)**, pour les _**références en gestion quantité à la référence**_
* Le **seuil d'alerte**
* Le **seuil de sécurité**
* L'**urgence**, et son **commentaire** s'il est coché, pour les _**références en gestion quantité à l'article**_
* **Ajouter un article fournisseur**
* La **catégorie d'inventaire**
* Les **champs libres**

Cliquez sur <mark style="background-color:blue;">**Annuler**</mark> pour revenir en mode visualisation sans prendre en compte ce que vous avez pu modifier. Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour enregistrer vos modifications

Si vous modifiez une référence en changeant son statut de _Brouillon_ à _Actif_, un mail sera envoyé à l'enregistrement au créateur de la référence pour lui indiquer que sa référence a été validée.

#### Modifier partiellement une référence

Certains utilisateurs peuvent avoir un rôle leur autorisant partiellement de modifier une référence. Dans ce cas, ils pourront modifier les champs :&#x20;

* **Image**
* **Libellé**
* **Pièces jointes**
* **Nomenclature**
* **Prix unitaire (€)**, pour les _**références en gestion quantité à la référence**_
* **Seuil d'alerte**
* **Seuil de sécurité**
* **Urgence** et **commentaire de l'urgence**, pour les _**références en gestion quantité à l'article**_
* **Fournisseurs**
* **Champs libres**

### Supprimer une référence

Pour supprimer une référence, cliquez sur les ![](<../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>) de la ligne de référence et cliquez sur <mark style="background-color:blue;">**Supprimer**</mark>.

Une modale de confirmation de suppression apparaîtra alors.&#x20;

Il n'est pas possible de supprimer une référence dans le cas où elle est liée à n'importe quel élément de l'application (colis, mouvements, livraison, collecte, transfert, réception, ou article fournisseur). Dans ce cas, il est conseillé de passer la référence en _Inactif_ si vous n'en avez plus l'utilité.

### Voir les mouvements

Pour voir les mouvements de stock concernant seulement la référence que vous souhaitez, en plus de filtrer sur la référence dans la page Stock > Mouvements de stock, vous pouvez cliquez sur les ![](<../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>) de la ligne de la référence et cliquez sur <mark style="background-color:blue;">**Voir les mouvements**</mark>.&#x20;

Une modale s'ouvrira alors avec la liste de tous les mouvements de stock de la référence.&#x20;

Elle est constituée de :

* Une zone de **recherche rapide**
* Un **tableau**
* Une **pagination**&#x20;

Contenu du tableau :

| Colonne          | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Date**         | Date et heure du mouvement de stock                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Issu de**      | <p>Origine du mouvement. Il est possible d'avoir en origine : <br>- une réception (mouvement d'entrée)<br>- une préparation (mouvement de transfert)<br>- une livraison (mouvement de sortie)<br>- une collecte (mouvement d'entrée)<br>- un transfert (mouvement de transfert)<br>- un inventaire (mouvement d'entée ou de sortie inventaire)<br>Si la donnée contient une flèche, il est possible de cliquer dessus pour être redirigé vers la demande ou l'ordre en question</p> |
| **Code article** | Code de l'article mouvementé. S'il s'agit d'une référence en gestion quantité référence, cela sera le code barre de la référence                                                                                                                                                                                                                                                                                                                                                    |
| **Quantité**     | Quantité mouvementée                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Origine**      | Emplacement d'origine du mouvement. L'origine n'est pas tout le temps remplie en fonction du type de mouvement et de la sa provenance                                                                                                                                                                                                                                                                                                                                               |
| **Destination**  | Emplacement de destination du mouvement. La destination n'est pas tout le temps remplie en fonction du type de mouvement et de la sa provenance                                                                                                                                                                                                                                                                                                                                     |
| **Type**         | Type du mouvement entrée transfert sortie entrée d'inventaire sortie d'inventaire                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Opérateur**    | Utilisateur ayant réalisé le mouvement                                                                                                                                                                                                                                                                                                                                                                                                                                              |

### Recalculer les quantités

Pour accéder au recalcul des quantités, clique sur les ![](<../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16.png>) de la référence souhaitée puis cliquez sur <mark style="background-color:blue;">**Recalculer les quantités**</mark>. Les quantités en stock et disponibles seront alors mises à jour. Ce bouton sert notamment si vous avez effectué une opération qui touche à la quantité de la référence et qu'elle n'a pas encore été mise à jour sur la page.&#x20;

### Ajouter au panier

C'est à partir de la page des références qu'il est possible d'ajouter une référence au panier, afin de la demander en livraison, en collecte, ou en achat.

Cliquez sur le panier sur la ligne de la référence que vous souhaitez ajouter au panier pour qu'elle soit ajoutée au panier. Pour voir le fonctionnement du panier, voir [Panier](panier.md).

Si une référence n'a pas de panier sur sa ligne, c'est qu'elle est inactive.
