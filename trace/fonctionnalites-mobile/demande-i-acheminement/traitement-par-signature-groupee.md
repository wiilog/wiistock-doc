---
description: >-
  Le traitement des demandes d'acheminement par signature groupée sur
  l'application mobile implique un contrôle de validation des prises et déposes
  d'unités logistiques sur les emplacements.
---

# Traitement par signature groupée

## Création d'une demande d'acheminement

Dans le menu **Demande | Acheminement** appuyer sur <mark style="background-color:blue;">**+**</mark> et vous serez dirigé vers l'écran **Demande | Acheminement | Création**. Il vous faudra remplir le formulaire de création de demande d'acheminement avec les champs suivants :&#x20;

<figure><img src="../../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

* **Type\*** : Type d'acheminement paramétré dans **Paramétrage | Trace | Acheminements | Types et champs libres.**&#x20;
* **Enlèvement\*** : Emplacement d'enlèvement. Vous avez la possibilité lors de l'ajout d'un nouveau Type de saisir un emplacement de prise par défaut ou encore définir un ou plusieurs emplacements de prise suggérés. Ce paramétrage permettra de bloquer la saisie d'autres emplacements qui ne sont pas associés au type.&#x20;
* **Livraison\*** : Emplacement de dépose. Vous avez la possibilité lors de l'ajout d'un nouveau Type de saisir un emplacement de dépose par défaut ou encore définir un ou plusieurs emplacements de dépose suggérés. Ce paramétrage permettra de bloquer la saisie d'autres emplacements qui ne sont pas associés au type.&#x20;
* **Commentaire** : Commentaire d'une demande d'acheminement.
* **Urgence** : Degré d'urgence de la demande d'acheminement paramétrable dans **Paramétrage | Trace | Acheminements | Champs fixe | Urgence**.&#x20;
* **Destinataire** : Destinataire optionnel du mail de réception des comptes rendus en PDF. Champ lié au référentiel Utilisateurs.&#x20;

Cliquer sur <mark style="background-color:blue;">**Valider**</mark>, vous serez dirigé vers l'écran d'ajout d'unité logistique.

### Ajouter des unités logistiques

Vous pouvez ajouter des unités logistiques via scan du code barre ou par entrée manuelle.&#x20;

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

Par scan, flasher le code barre / QR code de votre UL et vous serez automatiquement dirigé vers le formulaire d'ajout de référence.

Par entrée manuelle, saisissez votre UL puis appuyer sur <mark style="background-color:blue;">**+**</mark> et vous serez dirigé vers le formulaire d'ajout de référence.

<figure><img src="../../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

Dans ce formulaire, vous pouvez renseigner des informations sur votre unité logistique : &#x20;

* **Nature\*** : Nature de l'unité logistique. Possibilité d'en paramétrer une par défaut dans **Référentiel | Nature | Ajouter une nature** ou **à la modification** de sa fiche, en cochant <mark style="background-color:blue;">**Nature par défaut.**</mark>
* **Poids (kg)** : Poids (kg) de l'unité logistique. Champ textuel libre.
* **Volume (m3)** : Volume (m3) de l'unité logistique. Champ textuel libre.&#x20;
* **Commentaire** : Commentaire de l'unité logistique.
* **Référence\*** : Référence à ajouter. Fait appel au **Stock | Référence**, il vous faut saisir le code référence **en entier** puis appuyer sur le bouton <mark style="background-color:blue;">**Rechercher.**</mark>

**Attention** : Le fonctionnel du traitement des demandes d'acheminements par signature groupée s'applique avec des **demandes d'acheminement contenant une unique référence par unité logistique**. Mais vous pouvez mettre autant d'unités logistiques dans votre demande d'acheminement.

### Ajouter une référence

Pour ajouter une référence dans une unité logistique deux cas de figures : &#x20;

#### Ajouter une référence existante

Si je souhaite ajouter une référence déjà existante dans mon stock, je dois **saisir le code de référence entièrement** dans le champ <mark style="background-color:blue;">**Référence**</mark>, puis appuyer sur le bouton <mark style="background-color:blue;">**Rechercher.**</mark> Par la suite, un formulaire va s'afficher avec plusieurs champs d'informations à propos de la référence. Certains seront pré remplis s'ils sont renseignés sur la fiche de l'article de référence, et d'autres devront être saisis car c'est des informations propres à une demande d'acheminement.

Champs propres à une demande d'acheminement à saisir : &#x20;

* **Quantité\*** : Quantité de la référence présente dans l'unité logistique.&#x20;
* **Numéro de série** : Numéro de série de la référence. Champ textuel libre.
* **Numéro de lot\*** : Numéro de lot de la référence. Champ textuel libre.
* **Numéro de plombage/scellé** : Numéro de plombage/scellé de la référence. Champ textuel libre.&#x20;
* **ADR** : Accord européen relatif au transport international des marchandises Dangereuses par Route. Champ de type Switch, sélectionné en Off par défaut.&#x20;
* **Commentaire** : Commentaire sur la référence. Propre à une demande d'acheminement et n'est donc associé au champ Commentaire dans **Stock | Références | Article de référence.**
* **Photo(s)** : Pièce(s) jointe(s) à joindre à propos de la référence dans la demande d'acheminement. Propre à une demande d'acheminement et n'est donc pas associé au champ Commentaire dans **Stock | Références | Article de référence.**

Les autre champs seront pré remplis s'ils sont renseignés dans la fiche de référence. Ils sont **modifiables via le formulaire d'ajout de référence**. Vous pourrez voir leurs modifications dans **Stock | Références | Article de référence | Description.**&#x20;

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

* **Matériel hors format** : Champ de type Switch, sélectionné Off par défaut.&#x20;
* **Code fabricant\*** : Code fabricant de la référence. Champ textuel libre.
* **Longueur (cm)** : Longueur en cm de la référence.&#x20;
* **Largeur (cm)** : Largeur en cm de la référence.
* **Hauteur (cm)** : Hauteur en cm de la référence.&#x20;
* **Volume (m3)\*** : Volume en m3 de la référence. Le calcul de celui-ci se fait grâce à la saisie des champs Longueur, Largeur et Hauteur. Il est en valeur décimal 6 chiffres après la virgule.&#x20;
* **Poids (kg)\*** : Poids en kg de la référence.
* **Types de documents associés\*** : Sélection d'un ou plusieurs types de documents associés. Paramétrables dans Paramétrage | Stock | Configurations, via le champ <mark style="background-color:blue;">**Valeurs du champ "Types de documents associés d'une référence article."**</mark>

Après les avoir saisis, appuyer sur <mark style="background-color:blue;">**Valider.**</mark>

#### Ajouter une nouvelle référence

Pour ajouter et créer une référence dans l'unité logistique de votre demande d'acheminement, il suffit de saisir le code référence et d'appuyer sur le bouton <mark style="background-color:blue;">**Rechercher.**</mark> Sur le même principe que d'ajouter une référence déjà existante, le formulaire s'affichera mais en ayant aucuns champs de rempli.&#x20;

Il y a des champs obligatoires à saisir pour créer une référence :&#x20;

* **Quantité\***
* **Numéro de lot**
* **Code fabricant**
* **Longueur (cm)**
* **Largeur (cm)**&#x20;
* **Hauteur (cm)**&#x20;
* **Volume (m3)**
* **Poids (kg)**
* **Types de documents associés**

&#x20;Une fois le formulaire complété, appuyer sur <mark style="background-color:blue;">**Valider**</mark> ; votre référence sera bien créée et enregistrée dans votre stock.&#x20;

#### Visualisation d'une demande d'acheminement en état brouillon

Vous pouvez donc ajouter autant d'UL contenant une référence pour chaque dans votre demande. A chaque UL ajoutée, vous avez un **visuel global** de votre demande d'acheminent avec les informations générales de celle-ci : Numéro de demande d'acheminement, Enlèvement, Livraison, Commentaire, Urgence et Type.&#x20;

<figure><img src="../../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

Ainsi que le contenant de celle-ci avec vos UL, leurs numéros, la nature de l'UL, la référence contenant et la quantité de celle-ci. En appuyant sur la vignette d'une UL, vous pouvez rentrer dans le détail de celle-ci, modifier ses informations et celles de la référence.  Il est possible également de la supprimer via l'icône poubelle.&#x20;

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

#### Générer une lettre de voiture

Avant de valider votre demande d'acheminement pour la passer au statut A traiter, vous pouvez générer une lettre de voiture via le switch. Sélectionné en Off par défaut, si vous le passez en On, vous serez dirigé vers le formulaire de lettre de voiture.&#x20;

Vous pouvez paramétrer les champs par défaut dans **Paramétrage | Modèles de document | Acheminements | Lettre de voiture | Champs par défaut**. Liste des champs paramétrables :&#x20;

* **Adresse de l'expéditeur\***
* **Nom de l'expéditeur\***
* **Téléphone / Email\***
* **Adresse du destinataire par défaut\***
* **Lieu de chargement\***
* **Lieu de déchargement\***
* **Transporteur par défaut\***

**Attention :** Les saisies de l'utilisateur pour le formulaire de la lettre de voiture sont enregistrées malgré le paramétrage des champs par défaut. Dans le cas où vous saisissez un **Lieu de chargement** et un **Lieu de déchargement** différents à chaque demande d'acheminement, vous devez cocher le paramétrage <mark style="background-color:blue;">**Ne pas sauvegarder les saisies de l'utilisateur pour la lettre de voiture.**</mark> Ce paramétrage s'applique uniquement pour ces deux champs.

Sur le formulaire de la lettre de voiture sur le nomade, il vous faudra renseigner trois champs obligatoires en plus :&#x20;

* **Destinataire - Nom\***
* **Destinataire - Téléphone - Email\***
* **Notes de bas de page\***

Appuyer ensuite sur <mark style="background-color:blue;">**Valider.**</mark> Votre lettre voiture sera générée et **téléchargée automatiquement en format PDF dans vos fichiers.** Vous pourrez également la retrouver en pièce jointe sur le web dans le détail de votre demande d'acheminement.&#x20;

Lorsque vous estimez que la création de votre demande d'acheminement est complète et prête, appuyer sur <mark style="background-color:blue;">**Valider.**</mark> Ainsi votre demande d'acheminement passe du **statut Brouillon en A traiter.**&#x20;

## Traitement par signature groupée

Après avoir créer une ou plusieurs demandes d'acheminements prêtes à être enlevées sur leur emplacement de prise, il vous faut les traiter dans le menu **Traçabilité | Acheminement.**&#x20;

Le fonctionnel du traitement par signature groupée a été pensé dans le cas du traitement de plusieurs demandes en même temps. Mais il est tout à fait possible d'utiliser la signature pour une seule demande d'acheminement.&#x20;

Dans l'écran **Traçabilité | Acheminement**, il vous sera affiché toutes les demandes d'acheminement de tous les utilisateurs de votre instance. Après avoir coché dans **Paramétrage | Utilisateurs | Rôles | Demande | Acheminements**, le paramétrage <mark style="background-color:blue;">**Signature groupée**</mark> et <mark style="background-color:blue;">**Obliger la signature groupée pour traiter les acheminements**</mark> dans **Paramétrage | Trace | Acheminements | Configuration,** sera visible sur votre liste le bouton <mark style="background-color:blue;">**Signature groupée**</mark> permettant d'utiliser le fonctionnel du traitement par signature groupée.&#x20;

### Filtrer les demandes d'acheminements

Après avoir appuyé sur <mark style="background-color:blue;">**Signature groupée,**</mark> vous êtes dirigé vers l'écran **Traçabilité | Acheminements | Signature groupée** permettant de **filtrer et sélectionner** les demandes d'acheminements.&#x20;

Pou rappel, pour faire la signature groupée les demandes doivent **avoir les mêmes caractéristiques**, **le même statut, le même type d'acheminement et le même emplacement de prise OU de dépose.** Sans ces conditions réunies, la signature groupée ne peut être appliquée.&#x20;

Vous pouvez donc sélectionner par le scan d'une unité logistique dans une demande d'acheminement ou manuellement par la flèche de transfert.&#x20;

C'est **au scan d'une troisième UL** donc de trois demandes d'acheminements que les filtres se définissent et s'appliquent : Enlèvement ou Livraison, Statut et Type.&#x20;

Cet enregistrement des filtres permet de :&#x20;

* Scanner ou transférer uniquement des demandes d'acheminements ayant les mêmes caractéristiques.&#x20;
* Définir si la signature groupée est en situation d'enlèvement ou de livraison. Cela implique à l'étape suivante, la sélection des statuts postérieurs selon l'ordre défini dans le paramétrage des statuts.&#x20;

<figure><img src="../../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

Dans cet exemple sur la capture ci-dessus, les filtres appliqués après avoir scanné 3 UL, sont :&#x20;

* Enlèvement : LBH- Gare A. Après avoir **scanné trois UL de trois demandes d'acheminement ayant le même emplacement de l'enlèvement et un emplacement de livraison différent, l'application a détecté que nous sommes en situation d'enlèvement**. Dans le cas d'une situation de livraison c'est à dire au moins trois demandes ayant le même emplacement de livraison, on aurait affiché à la place du champ Enlèvement, le champ Livraison.
* Statut :  A signer. Les 7 demandes d'acheminement sélectionnées ont toutes le même statut.&#x20;
* Type : INTRASITE. Les 7 demandes d'acheminement sélectionnées ont toutes le même type.&#x20;

Après avoir sélectionné vos demandes d'acheminements, appuyer sur <mark style="background-color:blue;">**Valider.**</mark>

### Sélectionné un statut

Comme expliqué précédemment, dans mon exemple toutes mes demandes d'acheminement sont au statut A signer (en état A traiter), donc dans ma sélection de statut sera affichée uniquement le ou les statuts postérieurs selon l'ordre défini dans le paramétrage des statuts. Ici, mon seul choix possible c'est le statut Validé que j'ai paramétré en état partiel.

<figure><img src="../../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>



### Signature groupée

Suite à ma sélection du statut, j'appuie sur <mark style="background-color:blue;">**Valider.**</mark> Vient donc l'étape de la signature groupée.

Pour valider la signature et le changement de statut de mes demandes d'acheminements, plusieurs conditions :&#x20;

* Le trigramme signataire (utilisateur) et code signataire doivent correspondre auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>
* Les champs Trigramme signataire, Code signataire et Commentaire (s'il a été paramétré comme tel) sont obligatoires, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>&#x20;
* Uniquement le ou les signataire attribués à l'emplacement de prise (en situation d'enlèvement) ou à l'emplacement de dépose (en situation de livraison) qui peuvent valider cet étape, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>

<figure><img src="../../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Appuyer sur <mark style="background-color:blue;">**Valider**</mark>, et vos demandes d'acheminements passeront au statut A signer (état A traiter) au statut Validé (étant Partiel). Les comptes rendus et mails seront envoyés aux destinataires paramétrés, et le détail de de vos demandes d'acheminements sur le web sera mis à jour.&#x20;
