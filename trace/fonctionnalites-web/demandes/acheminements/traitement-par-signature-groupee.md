---
description: >-
  Le traitement des demandes d'acheminement par signature groupée implique un
  contrôle de validation des prises et déposes d'unités logistiques sur les
  emplacements.
---

# Traitement par signature groupée

Le principe de traitement des demandes d'acheminement par signature groupée nécessite un paramétrage spécifique pour appliquer ce fonctionnel. A la différence du traitement standard des demandes d'acheminement, le passage d'un statut à un autre nécessite une validation supplémentaire. Cette validation s'applique via un code signataire personnel à chaque utilisation de l'application que vous pouvez saisir sur la fiche utilisateur ou par un import des utilisateurs. De cette manière, vous pouvez également sélectionner plusieurs demandes d'acheminement ayant les mêmes caractéristiques, et les passer au statut suivant dans le même temps avec une signature groupée.&#x20;

Pour utiliser ce fonctionnel, dans **Paramétrage | Utilisateurs | Rôles | Demande | Acheminement**s, il suffira de cocher le paramétrage <mark style="background-color:blue;">**Signature groupée.**</mark> Il peut s'appliquer à la fois sur le nomade et la supervision.

Il vous faudra également dans **Paramétrage | Trace | Acheminements | Configuration**, cocher le paramétrage <mark style="background-color:blue;">**Obliger la signature groupée pour traiter les acheminements.**</mark>

## Code signataire



<figure><img src="../../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Ce code signataire doit comporter au minimum 4 caractères, il est confidentiel et propre à chaque utilisateur donc associé à son nom.&#x20;

Il est donc **saisi lors du changement de statut d'une demande d'acheminement.** Son utilisation est semblable à l'application d'un identifiant et mot de passe, si le code signataire n'est pas associé à l'utilisateur vous ne pourrez valider le changement de statut.&#x20;

## Paramétrage des statuts

Comme énoncé précédemment, la signature groupée s'applique sur le changement de statut, il faut donc les paramétrer dans **Paramétrage | Trace | Acheminements | Statuts.**&#x20;

Le tableau du paramétrage des statuts  se présente en plusieurs colonnes :&#x20;

<table><thead><tr><th width="358">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Libellé*</strong></td><td>Libellé du statut.</td></tr><tr><td><strong>Etat*</strong></td><td>Etat du statut. Quatre états possibles : Brouillon ; A traiter ; Partiel et Traité.</td></tr><tr><td><strong>Type*</strong></td><td>Type d'acheminement sur lequel s'applique le paramétrage du statut. </td></tr><tr><td><strong>Envoi d'emails au demandeur</strong></td><td>Oui ou non. Le demandeur se réfère à celui qui créé la demande d'acheminement.</td></tr><tr><td><strong>Envoi d'emails au destinataire</strong></td><td>Oui ou non. Le destinataire se réfère à celui qui a été désigné comme tel lors de la création de la demande d'acheminement. </td></tr><tr><td><strong>Envoi compte rendu</strong></td><td>Oui ou non. Le compte rendu est un document PDF visible dans le détail de la demande d'acheminement une fois généré et peut être inclus en pièce jointe dans le mail standard du suivi du traitement de la demande d'acheminement. C'est une synthèse de l'état de la demande, avec les UL et références qu'elle contient.</td></tr><tr><td><strong>Signature groupée</strong></td><td>Enlèvement ou livraison. Définir si la signature groupée est pour une situation d'enlèvement  à ce statut ou une situation de livraison. Ce paramétrage s'applique lors du traitement sur nomade, lors de la sélection du statut d'une demande d'acheminement. Il permet de proposer uniquement les statuts à venir selon l'ordre défini.</td></tr><tr><td><strong>Couleur signature groupée</strong></td><td>Entête colorée. Lors de l'application de la signature groupée sur le nomade, vous retrouverez la liste des demandes d'acheminement à sélectionner, ils seront  différencier de leur statut grâce aux entêtes colorées définies.</td></tr><tr><td><strong>Synchronisation nomade</strong></td><td>Oui ou non. Synchronisation du statut qui sera visible sur le nomade.</td></tr><tr><td><strong>Commentaire obligatoire signature groupée</strong></td><td>Oui ou non. Champ libre textuel, à rajouter lors de la saisie du code signataire pour signer une demande d'acheminement.</td></tr><tr><td><strong>Ordre*</strong></td><td>Ordre des statuts.</td></tr></tbody></table>

Le paramétrage des statuts est important pour la définition de votre workflow avec l'application de la signature groupée.

## Worflow du traitement par signature groupée

Pour rappel, lors de la création d'une demande d'acheminement il est obligatoire de saisir un emplacement de prise et un emplacement de dépose. Dans le flux standard classique, à la création de votre demande, celle-ci est en état Brouillon, puis après avoir ajouté vos UL et références, à la validation le demande passe en état A traiter. Une fois déposée sur l'emplacement de dépose indiqué, votre demande termine son workflow en état Traité.&#x20;

Dans le fonctionnel de signature groupée, on ajoute au workflow un état <mark style="background-color:blue;">**Partiel**</mark> qui intervient après l'état A traiter. Pour donner un exemple, cet état Partiel on lui a attribué comme libellé de statut "Validé". En appliquant le paramétrage de la Signature groupée sur ce statut, cette action traduit une validation de l'enlèvement des unités logistiques sur l'emplacement de prise.&#x20;

On peut le voir également comme une vérification, ou un contrôle d'autrui**\*** attestant que cette demande d'acheminement est A traiter et prête à transiter vers son emplacement de dépose.

Pour poursuivre notre exemple, vous pouvez également appliquer cette signature lors du passage de votre demande en état Traité, confirmant la dépose des unités logistiques sur l'emplacement de dépose. Cela renforce la confirmation du traitement, qui dans le standard nécessite uniquement la sélection du statut.&#x20;

Autres options, dans une optique de renforcer le contrôle de la traçabilité de vos unités logistiques, vous pouvez ajouter des statuts partiels qui précèdent l'état Traité, dans le cas où pour X raisons vos unités logistiques n'ont pas put être déposé à l'emplacement de dépose prévu. Exemple de statut en état partiel : Litige, Entrepôt fermé, Signataire absent.&#x20;

Voici un exemple de paramétrage de statut possible pour un contrôle total de chaque étape de traitement de vos demandes d'acheminement :&#x20;

<figure><img src="../../../../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

**\***Autrui, car le signataire de cette vérification peut être différent de l'utilisateur qui a créé la demande d'expédition.&#x20;

Après avoir paramétré vos statuts en fonction du type de vos acheminement. Il vous faut **définir des signataires sur emplacement.**

## Référentiel | Emplacements

Pour l'application de la signature groupée il vous faut en premier des **signataires ayant un code signataire** et qu'ils soient **attribués à des emplacements** en droit de signer.&#x20;

Pour signer une demande d'acheminement en situation d'enlèvement, c'est à dire de passer en état A traiter à Partiel (Validé), le signataire doit être attribué à l'emplacement de prise.&#x20;

Pour signer une demande d'acheminement en situation de livraison, c'est à dire de passer en état A traiter à Traité (Livré), ou encore Partiel à Traité (Livré), le signataire doit être attribué à l'emplacement de dépose.&#x20;

L'attribution des signataires sur les emplacements est saisie dans Référentiel | Emplacement en cliquant sur <mark style="background-color:blue;">**+ Nouvel emplacement,**</mark> à la modification d'emplacement ou encore via l'import des emplacements.&#x20;

Dans la modale, vous pourrez renseignez le champ <mark style="background-color:blue;">**Signataires**</mark> en sélectionnant un ou plusieurs utilisateurs enregistrés dans l'application. En effet, il peut y avoir plusieurs signataires possible sur un emplacement.

Vous retrouverez également le champ <mark style="background-color:blue;">**Email,**</mark> en l'usage ça peut être l'adresse mail de l'emplacement concerné. Cette adresse mail réceptionnera les mails du suivi de traitement des demandes d'acheminements qui transitent sur cet emplacement et qui ont fait l'objet d'une signature.&#x20;

<figure><img src="../../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

## Traitement des demandes d'acheminements&#x20;

L'application de signature groupée nécessite le traitement de plusieurs demandes d'acheminements. Il est toutefois possible de signer une seule demande.&#x20;

### Filtrer les demandes d'acheminements

Dans **Demande | Acheminement**, pour faire la signature groupée les demandes doivent **avoir les mêmes caractéristiques:** **le même statut, le même type d'acheminement et le même emplacement de prise et de dépose.** Sans ces conditions, la signature groupée ne peut être utilisée. Après avoir appliqué les filtres, cliquez sur ![](<../../../../.gitbook/assets/image (54).png>) à côté du bouton Exporter au format CSV, et cliquez sur <mark style="background-color:blue;">**Signature groupée.**</mark> La page Demande | Acheminement va s'actualiser dans le fonctionnel de signature groupée, il suffira de sélectionner le demandes d'acheminements à signer et par conséquent à changer de statut. Dans la capture ci-dessous, c'est une signature groupée en situation d'enlèvement de trois acheminements en état A traiter (A signer), de type INTRASITE avec le même emplacement de prise "LBH-Gare A".

<figure><img src="../../../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

### La signature groupée

Après avoir coché les demandes, cliquez sur <mark style="background-color:blue;">**Signature groupée**</mark> et une modale s'ouvrira. Vient l'étape de la sélection du <mark style="background-color:blue;">**statut**</mark>, la saisie du <mark style="background-color:blue;">**Trigramme signataire\***</mark> qui est le nom d'utilisateur, le <mark style="background-color:blue;">**Code signataire\***</mark> associé à l'utilisateur et <mark style="background-color:blue;">**Commentaire**</mark> qui en fonction du paramétrage des statuts peut être obligatoire ou non.&#x20;

Le Code signataire est confidentiel, vous ne verrez apparaître que des étoiles et non les caractères visibles.&#x20;

Pour valider la signature et le changement de statut, plusieurs conditions :&#x20;

* Le trigramme signataire et code signataire doivent correspondre auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>
* Les champs Statut, Trigramme signataire, Code signataire et Commentaire (s'il a été paramétré comme tel) sont obligatoires, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>&#x20;
* Uniquement le ou les signataire attribués à l'emplacement de prise (en situation d'enlèvement) ou à l'emplacement de dépose (en situation de livraison) qui peuvent valider cet étape, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>

<figure><img src="../../../../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

### Le compte rendu

Après avoir cliqué sur <mark style="background-color:blue;">**Valider,**</mark> les demandes d'acheminements sont mises à jour avec le statut sélectionné, et en fonction de votre paramétrage des statuts, un mail du suivi de traitement de la demande est envoyé avec en pièce jointe un compte rendu PDF, également présent dans le détail de votre demande d'acheminement.&#x20;

Dans le workflow du traitement d'une demande d'acheminement par signature groupée,  on y génère **deux comptes rendu** au format PDF :

* Le premier est généré lors de la signature en situation d'enlèvement attestant que les unités logistiques sont prêtes à être traitées et enlevées. Le titre du PDF est composé du numéro d'acheminement généré par l'application, du préfixe ENL (pour compte rendu de l'enlèvement), de l'emplacement de prise, puis emplacement de dépose et l'horodatage.&#x20;
* Le second est généré lors de lors de la signature en situation de livraison attestant que les unités logistiques ont bien été traitées et livrées. Le titre du PDF est composé du numéro d'acheminement généré par l'application, du préfixe LIV (pour compte rendu de livraison), de l'emplacement de prise, puis emplacement de dépose et l'horodatage.&#x20;

<figure><img src="../../../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

Ce format PDF est issu d'un modèle Word personnalisable en fonction des variables que vous souhaitez faire apparaître. L'objectif de ce document était de reprendre les informations générales de la demande d'acheminement, un tableau des unités logistiques et les références avec leurs informations.

Vous pouvez retrouvez notre modèle par défaut ainsi que les variables disponibles dans **Paramétrage | Modèle de document | Acheminements | Compte rendu.**
