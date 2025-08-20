---
description: >-
  La demande d'expédition sert à demander d'expédier une ou plusieurs références
  vers un emplacement nécessitant le transport de celle(s)-ci. Cela implique une
  décrémentation du stock.
---

# Expéditions

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Demande**</mark>, puis <mark style="background-color:blue;">**Expédition.**</mark> Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau

| Filtre                 | Description                                                                                                                                                                                                                                                                                               |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création de la demande d'expédition                                                                                                                                                                                                                              |
| **Au**                 | La tranche haute filtrant sur la date de création de la demande d'expédition                                                                                                                                                                                                                              |
| **Statuts**            | Le(s) statut(s) des demandes d'expéditions à filtrer                                                                                                                                                                                                                                                      |
| **Demandeurs**         | Pour filtrer sur la personne ayant créée la demande d'expédition. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignés dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **N° commande client** | Pour filtrer sur les numéros de commande client des demandes d'expédition                                                                                                                                                                                                                                 |
| **Transporteurs**      | Pour filtrer sur les transporteurs renseignés dans la demande d'expédition                                                                                                                                                                                                                                |

* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes d'expédition créées
* Une **gestion des colonnes** du tableau

<figure><img src="../../../.gitbook/assets/Capture d’écran 2025-08-19 à 15.17.27.png" alt=""><figcaption></figcaption></figure>

## Créer une demande d'expédition

### Via le bouton "+"

Dans le bouton d'action rapide, sélectionnez **Expédition** pour créer une demande d'expédition.

<figure><img src="../../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

Une modale s'ouvrira alors pour remplir les informations d'entête de la demande :&#x20;

* **Demandeur(s)\*** : personne créant la demande. Il est possible de changer ce champ ou d'ajouter plusieurs demandeurs. Par défaut, ce champ se remplit avec la personne connectée.
* **Téléphone\***: le numéro de téléphone du demandeur renseigné sur sa fiche utilisateur. Par défaut, ce champ se rempli avec le Demandeur.
* **N° commande client\*** : Le numéro de commande client que l'on associe à la demande d'expédition. Champ texte libre.
* **Livraison à titre gracieux** : Champ à cocher si cette demande d'expédition est à titre gratuit et sans frais.
* **Article(s) conforme(s)** : Champ à cocher si vous estimez que ce sont des articles conformes à expédier
* **Destinataire** :&#x20;
  * **Client\*** : Le client destinataire de la demande d'expédition. Ce champ fait appel aux clients enregistrés dans le **Référentiel | Client**, mais il est possible d'ajouter un nouveau client directement sur la modale de création de demande d'expédition.
  * **Téléphone\*** : Le numéro de téléphone du client destinataire renseigné sur la fiche client dans le **Référentiel | Client**. Par défaut, ce champ se rempli avec le Client.
* **A l'attention de :** Nom du destinataire final. Champ texte libre.
* **Adresse de livraison\* :** Adresse de livraison du client destinataire renseigné sur la fiche client dans le **Référentiel | Client**. Par défaut, ce champ se rempli avec le Client.
* **Expédition** :&#x20;
* **Date de prise en charge souhaitée**\* : Sélection de la date de prise en charge souhaitée de la demande d'expédition.
* **Transporteur** : Sélection du transporteur de la demande d'expédition. Les transporteurs sont enregistrés dans le **Référentiel | Transporteur.**
* **Envoi** National / International : Type d'envoi de la demande d'expédition. Par défaut, c'est Envoi National sélectionné.
* **Port** Dû / Payé :  Port Dû indique que le coût de transport est payé à l'arrivée, et Port Payé signifie que vendeur paie le fret pour le transport de la marchandise jusqu'à la destination convenue. Par défaut, c'est Port Dû sélectionné.
* **Autre** :&#x20;
* **Commentaire** : Possibilité d'ajouter un commentaire, une information supplémentaire sur la demande d'expédition.

<figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

En cliquant sur <mark style="background-color:blue;">**Enregistrer**</mark>, la demande d'expédition est créée au statut brouillon et vous êtes redirigé vers le **détail de la demande**.

Le **détail** est constitué de :&#x20;

* une **entête gauche**. Elle contient la timeline des statuts de la demande d'expédition de la création, au traitement, à la planification et à l'expédition. Puis les différents champs renseignés précédemment liés aux informations de la demande d'expédition.
* une **entête centrale.** Elle contient les informations du **Transport**, avec d'une part les **Caractéristiques** suivantes :&#x20;

**Nombre de colis** : Nombre d'unité logistique à expédier

**Valeur totale** : Somme total en euros, des références à expédier en fonction de leur prix unitaire des quantités.

**Poids brut(kg)** : Total du poids brut en kg après colisage.

**Poids net (kg)**: Total du poids net de toutes les références à expédier.

> Ces informations seront remplies automatiquement à l'ajout des références à expédier et de leur colisage. D'autre part, ce sont des informations complémentaires sur le **Transporteur** renseignées précédemment lors de la création et le Numéro de Tracking qui sera rempli à l'étape du colisage.

* Le **tableau** des **Produits à expédier**, qui a les colonnes suivantes :&#x20;

<table><thead><tr><th width="358">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Référence</strong></td><td>Référence à expédier.</td></tr><tr><td><img src="../../../.gitbook/assets/image (85).png" alt=""></td><td>Logo avertissant que la référence est renseignée sur sa fiche Article de référence comme étant une Matière Dangereuse. Affichage sous condition lors de la saisie d'une référence tagguée comme tel, si elle ne l'est pas le logo n'apparaît pas.</td></tr><tr><td><img src="../../../.gitbook/assets/image (24).png" alt=""></td><td>Lien qui dirige sur la fiche de l'article de Référence afin d'informer si une Fiche de données de sécurité a été ajoutée. Une référence tagguée comme matière dangereuse doit renseigner 3 champs obligatoires : Code ONU, Classe Produit et mettre en pièce jointe une Fiche de données de sécurité.</td></tr><tr><td><strong>Libellé</strong></td><td>Libellé de la référence à expédier. Champ pré rempli lors de la saisie de la référence.</td></tr><tr><td><strong>Quantité*</strong></td><td>Quantité de la référence à expédier.</td></tr><tr><td><strong>Prix unitaire (€)*</strong></td><td>Prix unitaire en euros de la référence à expédier.</td></tr><tr><td><strong>Poids net (kg)*</strong></td><td>Poids net en kg de la référence à expédier.</td></tr><tr><td><strong>Montant total</strong></td><td>Calcul du montant total du prix de la référence selon la quantité et le prix unitaire renseigné.</td></tr></tbody></table>

### Ajouter une référence

Pour ajouter une référence, cliquez sur <mark style="background-color:blue;">**+**</mark>**.**

Vous avez la possibilité de sélectionner une référence existante du Stock ou d'en créer une nouvelle. En cliquant sur <mark style="background-color:blue;">**+ Nouvelle référence**</mark>, vous serez dirigez sur la page de création **Stock | Article de référence**. Afin de pouvoir créer rapidement une références, vous pouvez appliquer un paramétrage des valeurs par défaut pour les champs obligatoires dans **Paramétrage | Stock | Demandes | Expédition**.&#x20;

Voici les informations que vous pouvez en préalable pré remplir pour la création d'une nouvelle référence dans une demande d'expédition :&#x20;

* Type de la référence
* Nom fournisseur
* Code fournisseur
* Référence article fournisseur
* Libellé article fournisseur

Tapez le code de la référence en premier, si elle est tagguée comme étant une Matière dangereuse, le logo Matière dangereuse apparaîtra ainsi que le logo permettant d'aller sur la fiche de l'article de référence pour voir ou ajouter sa fiche de données de sécurité. Puis saisir une quantité, le prix unitaire et le poids net. Le montant total de prix se remplira automatique à la fin de la saisie de la ligne.&#x20;

Vous pouvez supprimer une ligne de référence, et en ajouter autant que vous souhaitez en expédier.&#x20;

Une fois que vous avez fini d'ajouter vos références à expédier, cliquez sur le bouton <mark style="background-color:blue;">**Valider l'expédition**</mark> pour que votre demande d'expédition soit prise en compte et passe au statut à traiter.&#x20;

Au statut à traiter vous pouvez toujours rajouter des références en plus en fonction du paramétrage de vos droits, puis vous pouvez passer à l'étape de **Planification.** Il vous faut cliquez sur <mark style="background-color:blue;">**Planifier.**</mark>

<mark style="background-color:blue;">**Attention**</mark> : Le passage à l'étape de Planification nécessite une **vérification de la conformité des références à expédier**. Si vous souhaitez ajouter une référence tagguée comme Matière Dangereuse en n'ayant pas complété les informations obligatoires telles que la Fiche de données de sécurité, le Code ONU et la Classe produit, vous ne pourrez passer à l'étape Planification de votre demande d'expédition.  Dans ce cas un message pop-up vous avertira des champs manquants, il vous suffira de compléter les champs manquants et vous pourrez poursuivre votre process.&#x20;

Dans **Paramétrage | Stock | Demandes | Expédier**, vous avez la possibilité de définir par défaut un **Emplacement d'expédition** et un emplacement de **Quai d'expédition**. Ainsi vos références à expédier seront indiquées à ces lieux.&#x20;

### Planification

En cliquant sur Planifier, une modale s'ouvrira alors pour remplir les informations de <mark style="background-color:blue;">**Planification du transport**</mark> :&#x20;

* **Caractéristiques** :
* **Nombre d'UL\***: Indiquer le nombre d'unité logistique à expédier.
* **Poids brut (Kg)** : Poids brut total en kg des unités logistiques de la demande d'expédition.
* **Transporteur** :&#x20;
* **Nom transporteur** : Sélection du transporteur enregistré dans le **Référentiel | Transporteu**r. Il peut être pré rempli s'il a été renseigné au préalable lors de la création de la demande d'expédition.&#x20;
* **Numéro de tracking** : Numéro de tracking du transporteur. Champ textuel libre.
* **Date d'enlèvement** : Sélection de la date d'enlèvement de l'expédition par le transporteur.

<figure><img src="../../../.gitbook/assets/image (16) (1).png" alt=""><figcaption></figcaption></figure>

Une fois la modale remplis, cliquez sur le bouton <mark style="background-color:blue;">**Valider le transport.**</mark>

### Colisage

Vous serez dirigé dans la modale de Colisage UL permettant d'indiquer quelle références sont dans quels colis. Parmi la liste des références à expédier, le principe est de cocher celles que vous souhaitez mettre dans tel ou tel colis. Cette modale sert également à indiquer les dimensions du colis (Longueur x Largeur x Hauteur cm). De plus, pour se faire, il vous faut renseigner une nature de colis par défaut en allant dans le **Référentiel | Nature.**&#x20;

<figure><img src="../../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

Après avoir ranger vos références dans le nombre d'unité logistique que vous avez indiqué, cliquez sur <mark style="background-color:blue;">**Valider le colisage.**</mark> Votre demande d'expédition passe du statut A Traiter à Planifiée. Par conséquent elle est prête à être expédiée, pour passer à ce statut, il vous faudra cliquer sur le bouton <mark style="background-color:blue;">**Expédier.**</mark>&#x20;

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

### Envoi d'email

Par la suite, en fonction de votre paramétrage dans **Paramétrage | Stock  | Demandes | Expéditions**, vous pouvez déterminer à quel statut et les personnes qui réceptionneront un email de suivi de traitement de votre demande d'expédition.

### Bordereau de livraison

Enfin pour finir, vous avez possibilité de **Générer une bordereau de livraison** pour votre demande d'expédition en cliquant sur les trois petits de l'entête gauche.&#x20;

C'est un format PDF issu d'un modèle Word personnalisable en fonction des variables que vous souhaitez faire apparaître.&#x20;

Vous pouvez retrouvez notre modèle par défaut ainsi que les variables disponibles dans **Paramétrage | Modèle de document | Expéditions | Bordereau de livraison.**
