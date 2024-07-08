---
description: >-
  La page des emplacements contient tous les emplacements de l'application,
  ainsi que les groupes d'emplacement.
---

# Emplacements

Pour accéder à la page, vous devez aller dans le menu **Référentiel**, puis choisir **Emplacements**.

La page des colis contient plusieurs éléments :&#x20;

* Une **recherche rapide**, permettant de filtrer les données affichées dans les tableaux
* 2 **onglets** Emplacements et Groupes
* Un bouton <mark style="background-color:blue;">**Nouvel emplacement**</mark> pour l'**onglet Emplacements** pour ajouter un emplacement, contenant dessous 2 boutons
  * Bouton <mark style="background-color:blue;">**Imprimer les étiquettes**</mark> : faites d'abord une recherche rapide pour avoir une liste d'emplacements dont vous souhaitez avoir les étiquettes et cliquez sur le bouton pour sortir les étiquettes des emplacements. Vous pouvez aussi imprimer individuellement les étiquettes emplacement en cliquant sur<img src="../.gitbook/assets/3points" alt="" data-size="line">d'une ligne emplacement et en cliquant sur <mark style="background-color:blue;">**Imprimer**</mark>
  * Bouton <mark style="background-color:blue;">**Statut emplacement actif**</mark> : cliquez sur le bouton pour avoir seulement dans la liste les emplacements actifs
* Un bouton <mark style="background-color:blue;">**Nouveau groupe**</mark> pour l'**onglet Groupes** pour ajouter un groupe d'emplacements
* Un **tableau** dans chaque onglet, l'un avec la liste des emplacements, l'un avec la liste des groupes d'emplacements

{% embed url="https://www.screencast.com/t/w0JA2TNbKA3e" %}
Page référentiel emplacements
{% endembed %}

## Contenu du tableau - Onglet Emplacements

| Colonne                         | Description                                                                                                                                      |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Nom**                         | Nom de l'emplacement                                                                                                                             |
| **Description**                 | Description de l'emplacement                                                                                                                     |
| **Point de livraison**          | <p>Si l'emplacement est un point de livraison<br>Oui/Non</p>                                                                                     |
| **Encours visible**             | <p>Affichage de l'encours à la prise sur cet emplacement sur le terminal mobile<br>Oui/Non</p>                                                   |
| **Délai maximum**               | Délai maximum autorisé pour un colis sur cet emplacement                                                                                         |
| **Actif/Inactif**               | Statut de l'emplacement                                                                                                                          |
| **Natures de colis autorisées** | Natures des colis pouvant être déposées sur cet emplacement                                                                                      |
| **Températures autorisées**     | Ne pourront être accepté sur cet emplacement que des colis avec une plage de température correspondante (utilisé pour les demandes de transport) |

### Ajouter un emplacement

Pour ajouter un emplacement, cliquez le bouton <mark style="background-color:blue;">**Nouvel emplacement**</mark> et renseignez les champs suivants :&#x20;

* **Nom\*** : nom/code de l'emplacement. Ce nom peut contenir des lettres minuscules et/ou majuscules, des nombres de 0 à 9, les caractères \_, /, - et espace. Tous les autres caractères ne sont pas autorisés ainsi que les accents. Le nom doit avoir maximum 24 caractères et être unique.
* **Description\*** : description de l'emplacement. Cette description est utile notamment si votre nom est un code pour expliciter le code
* **Délais traça HH:MM** : temps maximum durant lequel un colis doit rester sur cet emplacement. Ce temps permet de mettre des indications visuelles dans l'application si un colis dépasse ce temps
* **Natures de colis autorisées** : ne mettez rien si toutes les natures de colis sont autorisées. Si vous mettez des natures de colis autorisées sur cet emplacement, il sera seulement possible de déposer des colis ayant ces natures sur cet emplacement
* **Températures autorisées** :  ne mettez rien si toutes les températures sont autorisées. Si vous mettez des températures autorisées sur cet emplacement, il sera seulement possible de déposer des colis ayant la même température sur cet emplacement
* **Types de livraisons autorisés** : lors de la création d'une demande de livraison, cet emplacement sera proposé dans les emplacements de destination pour les types autorisés sur cet emplacement
* **Types de collectes autorisés** : lors de la création d'une demande de collecte, cet emplacement sera proposé dans les points de collecte pour les types autorisés sur cet emplacement
* **Point de livraison ?** : activez ce paramétrage pour que, suite à un arrivage avec un destinataire, un mail soit envoyé au destinataire de cet arrivage quand les colis de cet arrivage sont déposés sur un emplacement identifié comme point de livraison
* **Encours visible nomade ?** : activez ce paramétrage pour que lors d'une prise sur le nomade sur cet emplacement, l'encours de cet emplacement, c'est-à-dire tous les colis présents sur cet emplacement, apparaisse. Attention, si cet emplacement a un encours important, il n'est pas conseillé d'activer ce paramétrage car cela risque de causer des ralentissements

<figure><img src="../.gitbook/assets/Photo sélectionnée (1).jpg" alt=""><figcaption><p>Vision de l'encours via activation du paramétrage "Encours visible nomade" depuis mouvement de prise</p></figcaption></figure>

Cliquez sur le bouton <mark style="background-color:blue;">**Enregistrer**</mark> pour valider la création de l'emplacement.

{% embed url="https://www.screencast.com/t/b2pci9ub2" %}

### Modifier un emplacement

Pour modifier un emplacement, cliquez sur la ligne de l'emplacement que vous souhaitez modifier pour ouvrir la modale de modification d'emplacement.&#x20;

La modale est la même que la modale de création ainsi que le remplissage de champs, excepté un champ supplémentaire qui est présent sur la modale de modification : le champ **Actif ?**. Ce champ est activé par défaut à la création d'un emplacement. Venez le désactiver si l'emplacement en cours de modification est un emplacement qui n'est plus utilisé mais que vous ne pouvez pas supprimer car utilisé dans l'application.&#x20;

N'oubliez pas d'<mark style="background-color:blue;">**enregistrer**</mark> pour valider vos modifications.&#x20;

### Supprimer un emplacement

Vous pouvez supprimer un emplacement en cliquant sur les<img src="../.gitbook/assets/3points" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression de l'emplacement. Si l'emplacement est déjà utilisé dans l'application, vous ne pourrez pas le supprimer et une modale d'erreur apparaîtra, vous proposant de passer en inactif l'emplacement.&#x20;

## Contenu du tableau - Onglet Groupes

Les groupes d'emplacements sont utilisés pour le moment dans l'application Wiilog dans la brique IoT pour associer un capteur à un groupe d'emplacement.&#x20;

Ils sont aussi utilisés sur les dropzone des utilisateurs pour l'envoi de mail de relance si un colis est présent sur un emplacement point de livraison faisant parti du groupe mis en dropzone sur l'utilisateur. &#x20;

| Colonne                   | Description                                  |
| ------------------------- | -------------------------------------------- |
| **Nom**                   | Nom du groupe                                |
| **Description**           | Description du groupe                        |
| **Actif/Inactif**         | Statut du groupe                             |
| **Nombre d'emplacements** | Nombre d'emplacements contenu dans un groupe |

Sur chaque ligne de groupe peut aussi apparaître un logo wifi si le groupe d'emplacement est lié à un objet connecté.&#x20;

<div align="center">

<img src="../.gitbook/assets/image (75).png" alt="">

</div>

Si la ligne a un logo wifi, un bouton <mark style="background-color:blue;">**Historique des données**</mark> est présent en plus sous les <img src="../.gitbook/assets/3points" alt="" data-size="line">

Il ouvre une page permettant de suivre toutes les données remontées par les capteurs qui ont été associés à ce groupe d'emplacements (Voir la partie [IoT](broken-reference) de la documentation).

### Ajouter un groupe d'emplacements

Pour ajouter un groupe d'emplacements, cliquez le bouton <mark style="background-color:blue;">**Nouveau groupe**</mark> et renseignez les champs suivants :

* **Nom du groupe\*** : nom du groupe d'emplacements. Ce nom doit être unique et ne doit pas être le même qu'un emplacement
* **Description\*** : description du groupe d'emplacements
* **Statut\*** : Actif/Inactif. Même chose que pour un emplacement : si vous n'utilisez plus un groupe d'emplacement qui ne peut pas être supprimé, passez le groupe en inactif
* **Emplacements\*** : emplacements faisant partis du groupe

### Modifier un groupe

Pour modifier un groupe d'emplacements, cliquez sur la ligne du groupe d'emplacements que vous souhaitez modifier pour ouvrir la modale de modification de groupe d'emplacements.&#x20;

La modale est la même que la modale de création ainsi que le remplissage de champs.

N'oubliez pas d'<mark style="background-color:blue;">**enregistrer**</mark> pour valider vos modifications.&#x20;

### Supprimer un groupe

Vous pouvez supprimer un groupe d'emplacements en cliquant sur les<img src="../.gitbook/assets/3points" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression du groupe d'emplacements. Si le groupe est déjà utilisé dans l'application, vous ne pourrez pas le supprimer et une modale d'erreur apparaîtra.
