---
hidden: true
---

# WiiSpool V2

#### Introduction

**Objectif**

L'objectif principal du système Wiispool est de fournir une solution efficace et conviviale pour la gestion des documents à imprimer. Conçu pour optimiser le traitement des travaux d'impression, Wiispool offre une automatisation accrue, réduisant ainsi le besoin d'interventions manuelles et augmentant la productivité globale. Grâce à sa configuration aisée et son interface intuitive, Wiispool vise à simplifier les tâches quotidiennes et à garantir une expérience utilisateur sans tracas. Wiispool se révèle particulièrement utile après la génération de divers documents PDF par Wiistock, notamment des étiquettes avec des dimensions personnalisées adaptées à vos besoins logistiques, ou des lettres de voiture destinées à être imprimées sur des feuilles de format A4, par exemple. Il est essentiel de souligner que ces documents peuvent nécessiter l'utilisation d'imprimantes distinctes pour une impression optimale. Wiispool facilite le processus d'impression en dirigeant automatiquement le document téléchargé vers l'imprimante appropriée, évitant ainsi toute confusion et optimisant l'efficacité de l'impression.

**Configuration**

* **téléchargement**

***

Pour commencer à utiliser Wiispool et améliorer la gestion de vos impressions, vous pouvez facilement télécharger le logiciel. Cliquez simplement sur le lien suivant pour accéder au fichier de téléchargement : [Télécharger Wiispool](https://github.com/wiilog/wiispool/releases/download/ScaleAndOrientationOK/wiispool.zip), ou rendez-vous à l'adresse suivante : [https://github.com/wiilog/wiispool/releases/download/ScaleAndOrientationOK](https://github.com/wiilog/wiispool/releases/download/ScaleAndOrientationOK/wiispool.zip) et téléchargez le fichier wiispool.zip

* **Installation**

Après avoir téléchargé le fichier `wiispool.zip`, suivez les étapes suivantes pour l'installation et la configuration de votre système :

* Décompresser le fichier téléchargé.
* Exécuter le programme d'installation pour installer Wiispool sur votre ordinateur, en exécutant le fichier ![](<../.gitbook/assets/image (101).png>)
* Lors de l'installation la fenêtre suivante peut apparaitre :&#x20;



<figure><img src="../.gitbook/assets/image (110).png" alt="" width="266"><figcaption></figcaption></figure>

_Le message que vous voyez est généré par Microsoft Defender SmartScreen, un composant de sécurité intégré à Windows. Il a pour objectif de protéger votre ordinateur en empêchant l'exécution d'applications non reconnues ou potentiellement dangereuses. Ce message apparaît car Wiispool est récemment développé et n'est pas largement utilisé, et peut ne pas être reconnue par SmartScreen. Pour contourner cette alerte vous pouvez cliquer sur "Informations complémentaires" puis sélectionner "Exécuter quand même"._

* Vous pouvez ajouter un lien vers Wiispool directement sur votre bureau en créant un raccourci vers le fichier ![](<../.gitbook/assets/image (102).png>)
* Création d'un raccourci sur le bureau Windows
  * Clic droit sur un endroit vide sur votre bureau => Nouveau => Raccourci => Entrer l'emplacement vers le fichier ![](<../.gitbook/assets/image (104).png>)que vous avez précédemment décompressé.
* **Configuration Initiale**\
  &#x20;

Lors du premier lancement de Wiispool l'interface est la suivante : ![](<../.gitbook/assets/image (105).png>)\
&#x20; Vous devez sélectionner le dossier que Wiispool va écouter pour effectuer l'envoie des fichiers à imprimer vers la bonne imprimante. Cliquer sur "Parcourir" et renseigner le chemin vers le dossier ou vos téléchargements sont stocker par votre navigateur sur votre poste de travail.\


**Trouver où le navigateur enregistre les fichiers téléchargés**

_(Dans cet exemple je montre la procédure en utilisant Chrome la procédure est très ressemblante sur les autres navigateurs)._\


* Cliquer sur les 3 points ![](<../.gitbook/assets/image (106).png>) en haut a droite de la fenêtres de votre navigateur. Puis cliquer sur paramètres.\
  ![](<../.gitbook/assets/image (107).png>)
* Aller dans le menu Téléchargements
* Ensuite recopier le chemin de l'emplacement où sont stockés vos téléchargements.

![captured screen](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2Fhojp6sKJ2FhUBigg2hta%2Fimage.png?alt=media\&token=089c11c2-4cc5-471b-a618-2752416f992f)\


**Création d'association préfixe/imprimante**

* Cliquer sur "Ajouter un préfixe"

<figure><img src="../.gitbook/assets/image (111).png" alt="" width="263"><figcaption></figcaption></figure>

* Dans la modale suivante&#x20;

<figure><img src="../.gitbook/assets/image (113).png" alt="" width="238"><figcaption></figcaption></figure>

* &#x20;Dans le champ "Ajouter un préfixe" renseignez le préfixe que vous voulez associer. _("ETQ" dans mon exemple)_
* Dans le champ _"Sélectionner un e imprimante", &#x73;_&#xE9;lectionnez l'imprimante que vous voulez associée au préfixe renseigné dans le champ du dessus._(L'imprimante doit déjà être accessible sur votre poste de travail)_
* Enregistrer cette nouvelle association en cliquant sur "_Ajouter un préfixe_".

**Modification d'une association préfixe/imprimante**

* Cliquez sur Liste attributs.

<figure><img src="../.gitbook/assets/image (114).png" alt="" width="240"><figcaption></figcaption></figure>

* Dans la fenêtre suivante, vous pouvez cliquer sur l'icone d'édition _(Crayon)._

<figure><img src="../.gitbook/assets/image (115).png" alt="" width="243"><figcaption></figcaption></figure>

* Vous êtes redirigé vers la fenêtre de modification d'une association préfixe/imprimante.

<figure><img src="../.gitbook/assets/image (116).png" alt="" width="243"><figcaption></figcaption></figure>

* Vous pouvez modifier le préfixe, l'imprimante vers la quelle vos documents .PDF préfixés par la valeur du champ "Modifier le préfixe" seront envoyés ou les deux.\
  Validez votre modification en cliquant sur "Modifier préfixe". votre modification est enregistrée vous pouvez modifier d'autres associations si vous avez besoin.
* En cliquant sur "Accueil" vous retournerez à la fenêtre principale de Wiispool.

**Lancer l'impression automatique**

* Une fois le paramétrage terminé, pour lancer l'exécution de Wiispool, il vous suffit de cliquer sur Activer l'impression.
* A partir de la dés que vous téléchargerez un document .PDF préfixé avec  un des préfixes paramétré, ce document sera automatiquement envoyé vers l'imprimante qui est associée avec ce préfixe et le document sera automatiquement supprimé de votre dossier de téléchargement.

