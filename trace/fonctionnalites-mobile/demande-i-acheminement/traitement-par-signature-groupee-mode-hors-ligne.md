---
description: >-
  Le traitement des demandes d'acheminement par signature groupée sur
  l'application mobile possède un mode hors ligne.
---

# Traitement par signature groupée - Mode hors ligne

Le mode hors ligne du traitement des acheminements uniquement par signature groupée s'active par le **Paramétrage | Utilisateurs | Rôle | Nomade | Demandes** - <mark style="background-color:blue;">**Mode hors ligne pour les demandes d'acheminements et la signature groupée.**</mark>&#x20;

Le fonctionnel mode hors ligne **s'applique différemment de celui du mode en ligne**. En effet, en mode en ligne la création de demande d'acheminement et le traitement se fait sur deux menus différents. En **mode hors ligne ça s'applique dans un unique menu Demande | Acheminement.**&#x20;

En premier lieu, pour utiliser le mode hors ligne il est important sur votre nomade de **vous mettre  en mode avion** afin d'éviter toutes possibilités pour l'application de détecter du réseau, car cela pourrait causer des pertes de données.&#x20;

## Menu Demande | Acheminement | Mode hors ligne

Tout le fonctionnel du mode hors ligne va s'appliquer dans le menu **Demande | Acheminement** contenant la liste des demandes d'acheminements.&#x20;

### Liste des demandes d'acheminement

A la différence du mode en ligne, vous retrouverez **uniquement les demandes d'acheminements créées par l'utilisateur connecté**.&#x20;

Le classement des demandes d'acheminements est établi selon un ordre :&#x20;

* En premier, les demandes d'acheminements ayant la mention d'Urgence, une icône d'urgence est visible sur les vignettes.
* En second, par l'ordre des statuts défini dans le paramétrage des statuts.&#x20;

### Visualisation des demandes d'acheminements

Plusieurs informations pour chaque demande d'acheminement sont visibles sur la liste :&#x20;

* **Entête colorée** : Associée au statut de la demande, paramétrée dans **Paramétrage | Trace | Acheminements | Types et champs libres.**
* **Numéro de la demande d'acheminement** : Numéro d'acheminement généré par l'application lorsque la demande a été synchronisée, si elle ne l'a pas encore été, le champ Numéro n'est pas visible.&#x20;
* **Dernière synchronisation** : Date et heure de la dernière synchronisation, si elle ne l'a pas encore été, le champ sera complété par "Non synchronisé".&#x20;
* **Type** : Type de la demande d'acheminement.&#x20;
* **Enlèvement** : Emplacement d'enlèvement.&#x20;
* **Livraison** : Emplacement de livraison.&#x20;
* **Urgence** : Urgence de la demande d'acheminement.&#x20;
* **Référence (quantité)** : Référence(s) présente(s) dans la demande d'acheminement et leurs quantités.&#x20;

### Les statuts de demandes d'acheminement en mode hors ligne

Voici les conditions d'affichage et de modification pour chaque état des demandes d'acheminement en mode hors ligne :

#### Etat brouillon&#x20;

* Voir le détail de la demande d'acheminement
* Possibilité de **supprimer la demande** via l'icône poubelle **si la demande d'acheminement n'a pas encore était synchronisée.**
* Ajouter de nouvelles unités logistiques et références.
* Modifier des unités logistiques et références.
* Supprimer des unités logistiques et références.

**Etat A traiter, Partiel et Traité**

* Voir le détail de l'acheminement
* Pour supprimer une demande d'acheminement en état A traiter, il vous faudra aller sur le web dans le détail de la demande d'acheminement, **la passer en état Brouillon** via les trois petits points afin de pouvoir la supprimer.&#x20;

<figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

### Menu

<figure><img src="../../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

Dans l'écran de la liste des demandes d'acheminement, pour le mode hors ligne le bouton ![](<../../../.gitbook/assets/image (55).png>) donne accès à un menu pour avoir accès à trois actions :&#x20;

* ![](<../../../.gitbook/assets/image (62).png>) **Création d'une demande** d'acheminement en mode hors ligne. Vous serez donc dirigé vers le formulaire de création de demande d'acheminement.
* ![](<../../../.gitbook/assets/image (41).png>) **Traitement des demandes d'acheminement par signature groupé**e en mode hors ligne. Vous serez dirigé vers l'écran de filtrage et de sélection des demandes d'acheminement pour la signature groupée.&#x20;
* ![](<../../../.gitbook/assets/image (77).png>) **Synchronisation** des demandes d'acheminement. Mise à jour de la liste des demandes d'acheminement.&#x20;

## La synchronisation

La synchronisation des données a pour objectif de **faire correspondre les données stockées en local sur un serveur.** Grâce à cette action les données sont mises à jour. Dans le cas de notre application, la synchronisation peut se faire soit :&#x20;

* Via l'appuie du bouton ![](<../../../.gitbook/assets/image (43).png>) Synchroniser
* Automatiquement via la désactivation du mode avion si vous êtes dans un lieu avec du réseau.
* Automatiquement via la désactivation du mode avion et activation du wifi s'il est présent.&#x20;
* Automatiquement en désactivant le mode avion et via la connexion éthernet au branchement d'un câble.

**Attention** : Lorsque vous utilisez le mode hors ligne pour le fonctionnel des acheminements par signature groupée, il est possible de faire tout le flux sans avoir synchronisé une fois, c'est à dire de la création jusqu'au traitement. Toutefois, si vous en avez la possibilité, il est important de synchroniser ces données à chaque fois que vous le pouvez. Auquel cas, penser à **rester sur le menu Demande | Acheminement** et à **ne pas en sortir si vous avez effectué des actions** (création d'acheminement, traitement) qui n'ont pas été synchronisées au moins une fois. Vous pouvez verrouillez votre nomade sur l'écran Demande | Acheminement sans perdre de la donnée, mais **si vous sortez de ce menu vos données seront effacées.** &#x20;

### Alerte

**A la connexion et déconnexion de l'utilisateur** sur l'application mobile, si vous utilisez le mode hors ligne en ayant activé le mode avion, un **message de rappel apparaîtra** " Veuillez vous connecter à internet afin de synchroniser vos données."

### Synchroniser

L'action de synchroniser s'affiche via un loading de synchronisation qui peut durer plusieurs secondes en fonction du nombre de demande d'acheminement à mettre à jour.&#x20;

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

**La synchronisation met à jour la liste des demandes d'acheminement** :&#x20;

_Synchronisation sur le nomade_ :&#x20;

* Les demandes d'acheminement en état Brouillon qui n'avaient pas été synchronisées ont un Numéro d'acheminement. Le champ "Dernière synchronisation : Non synchronisé" est remplacé par l'horodatage de la dernière synchronisation.&#x20;
* Les demandes d'acheminement en état A traiter et Partiel sont mises à jour avec leur date de dernière synchronisation.&#x20;
* Les demandes d'acheminement en état Traité disparaissent.

_Synchronisation sur le web_ :&#x20;

* Création des demandes d'acheminement dans **Demande | Acheminement**.
* **Mise à jour du statut, de la timeline et du champs "Dernière mise à jour"** dans le détail des demande d'acheminement.&#x20;
* **Mise à jour des modifications des références** lors de la création d'une demande d'acheminement.&#x20;
* **Création des nouvelles références** dans **Stock | Référence** lors de la création d'une demande d'acheminement.
* **Envoie des comptes rendu PDF et mail**.
* **Pièce jointe de la lettre de voiture dans le détai**l des demandes d'acheminements.&#x20;
* **Création et mise à jour des mouvements de traçabilité.** Un mouvement de prise et un mouvement de dépose.
* **Préservation des dates en temps réel**.&#x20;

## Création d'une demande d'acheminement en mode hors ligne

Dans le menu **Demande | Acheminement** appuyer sur le bouton ![](<../../../.gitbook/assets/image (35).png>) et vous serez dirigé vers l'écran **Demande | Acheminement | Création | Mode hors ligne**. **Même fonctionnel que le mode en ligne,** il vous faudra remplir le formulaire de création de demande d'acheminement. **Les paramétrages qui s'appliquent sur le mode en ligne, s'applique également sur le mode hors ligne.**&#x20;

* **Type\*** : Type d'acheminement paramétré dans **Paramétrage | Trace | Acheminements | Types et champs libres.**&#x20;
* **Enlèvement\*** : Emplacement de prise. Vous avez la possibilité lors de l'ajout d'un nouveau Type de saisir un emplacement de prise par défaut ou encore définir un ou plusieurs emplacements de prise suggérés. Ce paramétrage permettra de bloquer la saisie d'autres emplacements qui ne sont pas associés au type.&#x20;
* **Livraison\*** : Emplacement de dépose. Vous avez la possibilité lors de l'ajout d'un nouveau Type de saisir un emplacement de dépose par défaut ou encore définir un ou plusieurs emplacements de dépose suggérés. Ce paramétrage permettra de bloquer la saisie d'autres emplacements qui ne sont pas associés au type.
* **Commentaire** : Commentaire d'une demande d'acheminement.
* **Urgence** : Degré d'urgence de la demande d'acheminement paramétrable dans **Paramétrage | Trace | Acheminements | Champs fixe | Urgence.**&#x20;
* **Destinataire** : Destinataire optionnel du mail de réception des comptes rendus en PDF. Champ lié au référentiel Utilisateurs.&#x20;

Cliquer sur <mark style="background-color:blue;">**Valider**</mark>, vous serez dirigé vers l'écran d'ajout d'unité logistique.

### Ajouter des unités logistiques en mode hors ligne

**Même fonctionnel que le mode en ligne**, vous pouvez ajouter des unités logistiques via scan du code barre/ QR Code ou par entrée manuelle.&#x20;

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

Par scan, flasher le code barre / QR code de votre UL et vous serez automatiquement dirigé vers le formulaire d'ajout de référence.

Par entrée manuelle, saisissez votre UL puis appuyer sur <mark style="background-color:blue;">**+**</mark> et vous serez dirigé vers le formulaire d'ajout de référence.

<figure><img src="../../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

Dans ce formulaire, vous pouvez renseignez des informations sur votre unité logistique : &#x20;

* **Nature\*** : Nature de l'unité logistique. Possibilité d'en paramétrer une par défaut dans **Référentiel | Nature | Ajouter une nature** ou **à la modification** de sa fiche, en cochant <mark style="background-color:blue;">**Nature par défaut.**</mark>
* **Poids (kg)** : Poids (kg) de l'unité logistique. Champ textuel libre.
* **Volume (m3)** : Volume (m3) de l'unité logistique. Champ textuel libre.&#x20;
* **Commentaire** : Commentaire de l'unité logistique.
* **Référence\*** : Référence à ajouter. Fait appel au **Stock | Référence**, il vous faut saisir le code référence **en entier** puis appuyer sur le bouton <mark style="background-color:blue;">**Rechercher.**</mark>

**Attention** : Le fonctionnel du traitement des demandes d'acheminements par signature groupée s'applique avec des **demandes d'acheminement contenant une unique référence par unité logistique**. Mais vous pouvez mettre autant d'unités logistiques dans votre demande d'acheminement.

### Ajouter une référence en mode hors ligne

Pour ajouter une référence dans une unité logistique deux cas de figures : &#x20;

#### Ajouter une référence existante

Dans le fonctionnel du mode hors ligne, pour ajouter une référence déjà existante et récupérer ses informations, celle-ci doit être cochée en <mark style="background-color:blue;">**Synchronisation nomade.**</mark> **Attention, on ne peut synchroniser sur le nomade que 4 000 références.**

**A la saisie du code de référence** dans le champ <mark style="background-color:blue;">**Référence**</mark>, appuyer sur le bouton <mark style="background-color:blue;">**Rechercher**</mark> pour ouvrir le formulaire. Même fonctionnel que celui du mode en ligne, certains champs seront pré remplis s'ils sont renseignés sur la fiche de l'article de référence, et d'autres devront être saisis car c'est des informations propre à une demande d'acheminement.

Champs propres à une demande d'acheminement à saisir : &#x20;

* **Quantité\*** : Quantité de la référence présente dans l'unité logistique.&#x20;
* **Numéro de série** : Numéro de série de la référence. Champ textuel libre.
* **Numéro de lot\*** : Numéro de lot de la référence. Champ textuel libre.
* **Numéro de plombage/scellé** : Numéro de plombage/scellé de la référence. Champ textuel libre.&#x20;
* **ADR** : Accord européen relatif au transport international des marchandises Dangereuses par Route. Champ de type Switch, sélectionné en Off par défaut.&#x20;
* **Commentaire** : Commentaire sur la référence. Propre à une demande d'acheminement et n'est donc associé au champ Commentaire dans **Stock | Références | Article de référence**.
* **Photo(s)** : Pièce(s) jointe(s) à joindre à propos de la référence dans la demande d'acheminement. Propre à une demande d'acheminement et n'est donc associé au champ Pièce jointe dans **Stock | Références | Article de référenc**e.

Les autres champs sont pré remplis s'ils sont renseignés dans la fiche de référence. Ils sont **modifiables via le formulaire d'ajout de référence**. Vous pourrez voir leurs modifications dans **Stock | Références | Article de référence | Description après avoir synchronisé votre demande d'acheminement.**

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

* **Matériel hors format** : Champ de type Switch, sélectionné Off par défaut.&#x20;
* **Code fabricant\*** : Code fabriquant de la référence. Champ textuel libre.
* **Longueur (cm)** : Longueur en cm de la référence.&#x20;
* **Largeur (cm)** : Largeur en cm de la référence.
* **Hauteur (cm)** : Hauteur en cm de la référence.&#x20;
* **Volume (m3)\*** : Volume en m3 de la référence. Le calcul de celui-ci se fait grâce à la saisie des champs Longueur, Largeur et Hauteur. Il est en valeur décimal 6 chiffres après la virgule.&#x20;
* **Poids (kg)\*** : Poids en kg de la référence.
* **Types de documents associés\*** : Sélection d'un ou plusieurs types de documents associés. Paramétrable dans Paramétrage | Stock | Configurations, via le champ <mark style="background-color:blue;">**Valeurs du champ "Types de documents associés d'une référence article."**</mark>

Après les avoir saisis, appuyer sur <mark style="background-color:blue;">**Valider.**</mark>

#### Ajouter une nouvelle référence

Pour ajouter et créer une référence dans l'unité logistique de votre demande d'acheminement. Il suffit de saisir le code référence et d'appuyer sur le bouton <mark style="background-color:blue;">**Rechercher.**</mark> Sur le même principe que d'ajouter une référence déjà existante, le formulaire s'affichera mais en ayant aucuns champs de rempli. **Celle ci sera enregistrée dans la base de données lorsque la demande sera synchronisée.**

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

&#x20;Une fois le formulaire saisi, appuyer sur <mark style="background-color:blue;">**Valider.**</mark>

#### Visualisation d'une demande d'acheminement en état brouillon non synchronisée

Vous pouvez donc ajouter autant d'UL contenant une référence pour chaque dans votre demande. A chaque UL ajoutée, vous avez un **visuel globa**l de votre demande d'acheminent avec les informations générales de celle-ci : Enlèvement, Livraison, Commentaire, Urgence et Type.&#x20;

<figure><img src="../../../.gitbook/assets/image (13) (1).png" alt=""><figcaption></figcaption></figure>

Ainsi que le contenant de celle-ci avec vos UL, leurs numéros, la nature, la référence contenant et la quantité de celle-ci. En appuyant sur la vignette d'une UL, vous pouvez rentrer dans le détail de celle-ci, modifier ses informations et celles de la références.  Il est possible également de supprimer via l'icône poubelle.&#x20;

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

#### Générer une lettre de voiture en mode hors ligne

La génération de la lettre de voiture en mode hors ligne s'effectue lors de la création d'une demande d'acheminement. **Si la demande d'acheminement est au statut Brouillon et n'a toujours pas été synchronisée, vous pouvez générer autant de fois la lettre de voiture** dans la cas où vous modifiez à plusieurs reprises votre demande. En revanche, si votre demande d'acheminement a été synchronisée au moins une fois et même si elle est en état Brouillon, vous ne pourrez plus générer de lettre de voiture. Le switch ne sera plus accessible.&#x20;

**Le fonctionnel reste le même que celui du mode en ligne**, le switch est sélectionné en Off par défaut, si vous le passez en On, vous serez dirigé vers le formulaire de lettre de voiture.&#x20;

L'application des champs par défaut dans Paramétrag**e | Modèles de document | Acheminements | Lettre de voiture | Champs par défaut** s'applique aussi pour le mode hors ligne. Liste des champs paramétrables :&#x20;

* **Adresse de l'expéditeur\***
* **Nom de l'expéditeur\***
* **Téléphone / Email\***
* **Adresse du destinataire par défaut\***
* **Lieu de chargement\***
* **Lieu de déchargement\***
* **Transporteur par défaut\***

**Attention :** Les saisies de l'utilisateur pour le formulaire de la lettre de voiture sont enregistrées malgré le paramétrage des champs par défaut. Dans le cas où vous saisissez un **Lieu de chargement** et un **Lieu de déchargement** différents à chaque demande d'acheminement, vous devez cocher le paramétrage <mark style="background-color:blue;">**Ne pas sauvegarder les saisies de l'utilisateur pour la lettre de voiture.**</mark> Ce paramétrage s'applique uniquement pour ces deux champs.

Sur le formulaire de lettre de voiture sur le nomade, il vous faudra renseigner trois champs obligatoires en plus :&#x20;

* **Destinataire - Nom\***
* **Destinataire - Téléphone - Email\***
* **Notes de bas de page\***

Appuyer ensuite sur <mark style="background-color:blue;">**Valider.**</mark>&#x20;

A contrario du mode en ligne, **votre lettre de voiture sera accessible uniquement sur le web dans le détail de votre demande d'acheminement après synchronisation** de votre demande.&#x20;

_Si vous souhaitez l'avoir dans vos fichiers nomade, en présence de réseau, vous pouvez vous connecter sur le web en passant par le moteur de recherche de votre nomade et la télécharger par ce canal._

Lorsque vous estimez que la création de votre demande d'acheminement est complète et prête, appuyer sur <mark style="background-color:blue;">**Valider.**</mark> Ainsi votre demande d'acheminement passe du **statut Brouillon en A traiter, données enregistrées en local.**&#x20;

## Traitement par signature groupée

Après avoir créer un ou plusieurs demandes d'acheminements prête à être enlevées sur leur emplacement de prise, il vous faut les traiter dans le même menu **Demande | Acheminement** en appuyant sur le bouton ![](<../../../.gitbook/assets/image (61).png>)Signature groupée.

**Le traitement par signature groupée en mode hors ligne s'applique uniquement sur les demandes d'acheminement créées par l'utilisateur connecté**. Il a été pensé dans le cas du traitement de plusieurs demandes dans le même temps. Mais il est tout à fait possible d'utiliser la signature pour une seule demande d'acheminement.&#x20;

Après avoir appuyé sur le bouton ![](<../../../.gitbook/assets/image (61).png>)Signature groupée, vous serez directement dirigé sur l'écran de sélection et filtrage des demandes d'acheminement de l'utilisateur.&#x20;

Les paramétrages utilisés pour le mode en ligne ; **Paramétrage | Utilisateurs | Rôles | Demande | Acheminements** "<mark style="background-color:blue;">**Signature groupée"**</mark> et "<mark style="background-color:blue;">**Obliger la signature groupée pour traiter les acheminements"**</mark> dans **Paramétrage | Trace | Acheminements | Configuration s'appliquent également en mode hors ligne.**&#x20;

### Filtrer les demandes d'acheminements&#x20;

Pour rappel, pour faire la signature groupée les demandes doivent **avoir les mêmes caractéristiques**, **le même statut, le même type d'acheminement et le même emplacement de prise OU de dépose.** Sans ces conditions réunies, la signature groupée ne peut être utilisée.&#x20;

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

Après avoir sélectionné vos demandes d'acheminement, appuyer sur <mark style="background-color:blue;">**Valider.**</mark>

### Sélectionné un statut

Comme expliqué précédemment, dans mon exemple toutes mes demandes d'acheminement sont au statut A signer (en état A traiter), donc dans ma sélection de statut sera affiché uniquement le ou les statuts postérieurs selon l'ordre défini dans le paramétrage des statuts. Ici, mon seul choix possible c'est le statut Validé que j'ai paramétré en état partiel.

<figure><img src="../../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>



### Signature groupée mode hors ligne

Suite à ma sélection du statut, j'appuie sur <mark style="background-color:blue;">**Valider.**</mark> Vient donc l'étape de la signature groupée.

**Les associations utilisateurs et codes signataires sont enregistrées en local** et par conséquent le fonctionnel de signature groupée est le même que celui du mode en ligne.

Pour valider la signature et le changement de statut de mes demandes d'acheminements, plusieurs conditions :&#x20;

* Le trigramme signataire (utilisateur) et code signataire doivent correspondre auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>
* Les champs Trigramme signataire, Code signataire et Commentaire (s'il a été paramétré comme tel) sont obligatoires, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>&#x20;
* Uniquement le ou les signataire attribués à l'emplacement de prise (en situation d'enlèvement) ou à l'emplacement de dépose (en situation de livraison) qui peuvent valider cet étape, auquel cas, un message d'erreur apparaîtra après avoir cliqué sur <mark style="background-color:blue;">**Valider.**</mark>

<figure><img src="../../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Appuyer sur <mark style="background-color:blue;">**Valider**</mark>, et vos demandes d'acheminements passeront au statut A signer (état A traiter) au statut Validé (étant Partiel), le modification du statut est enregistrée en local. Pour communiquer les mises à jours de la demande au serveur il faudra synchroniser, et de ce fait les comptes rendus et mails seront envoyés aux destinataires paramétrés, le détail de vos demandes d'acheminement sur le web sera mis à jour et les mouvements de traçabilité seront créés.
