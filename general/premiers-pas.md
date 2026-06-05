# Premiers pas

## Création de vos instances

Vos instances (page web qui vous donne accès à l'application et ses fonctionnalités) sont créées par Wiilog. Vous aurez une instance de production et une instance de recette. La page de connexion se présente ainsi :

{% embed url="https://www.screencast.com/t/qqKcGidIT" %}

Créez votre premier compte utilisateur en cliquant sur <mark style="background-color:blue;">**Créer un compte**</mark> et demandez à Wiilog de vous accorder un rôle. Les rôles peuvent ensuite être paramétrés avec l'aide de Wiilog et selon les fonctionnalités que vous souhaitez utiliser.

## Création d'utilisateurs

### Via la page de connexion:&#x20;

Tout comme vous, un utilisateur a la possibilité d'utiliser l'option "Créer un compte" disponible sur la page de connexion de votre instance. Ensuite, il sera nécessaire de lui assigner un rôle approprié en fonction de son utilisation de l'application. Pour finaliser le processus, il conviendra de valider son compte en utilisant un compte déjà approuvé et ayant les droits requis pour réaliser ces démarches.&#x20;

### Via Paramétrage | Données | Imports & mises à jour :&#x20;

Si votre rôle le permet, vous avez la possibilité de créer des utilisateurs en masse en utilisant le module "Paramétrage | Données | Imports & mises à jour". Après avoir cliqué sur le bouton "<mark style="background-color:blue;">+ Nouvel import</mark>", sélectionnez "Utilisateur" comme valeur pour le champ "Type de données à importer". Votre fichier à importer doit être au format CSV encodé en UTF-8 et doit être conforme au modèle de document vierge que vous pouvez télécharger en cliquant sur le bouton "<mark style="background-color:blue;">Télécharger</mark>" disponible.&#x20;

### Via Paramétrage | Utilisateurs :&#x20;

Si votre rôle vous le permet, vous avez la possibilité de créer un nouvel utilisateur en accédant au module "Paramétrage | Utilisateurs" et en cliquant sur le bouton "<mark style="background-color:blue;">Nouvel utilisateur</mark>". Le formulaire de création s'affichera, vous permettant de saisir les informations nécessaires. Assurez-vous de cocher la case "<mark style="background-color:blue;">Statut actif</mark>" et d'attribuer le rôle approprié en fonction de l'utilisation prévue de l'application. <br>

## Mise à jour de l’application nomade sur un terminal Android Zebra

Certaines mises à jour de l'application exigent également une mise à jour de l'application nomade. À cet effet, je vous présente ci-dessous les méthodes disponibles pour réaliser ces mises à jour.&#x20;

### Mise à jour via l'interface nomade de Follow

Lorsqu'une mise à jour est nécessaire sur les appareils nomades, la page suivante apparaît lors de la connexion de l'utilisateur : &#x20;

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2023-08-23 113102.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Dans le cas où ce n'est pas la première fois qu'une mise à jour est effectuée sur cet appareil Android, si vous souhaitez réinstaller le fichier, il vous suffira de cliquer sur le bouton "Retélécharger". Une fois le téléchargement terminé, la fenêtre suivante apparaîtra. Pour ouvrir le fichier téléchargé, il vous suffira simplement de cliquer sur le bouton "<mark style="background-color:blue;">Ouvrir</mark>".
{% endhint %}

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2023-08-23 113332.png" alt=""><figcaption></figcaption></figure>

Si vous ne disposez pas du temps nécessaire pour cliquer immédiatement et que la fenêtre précédente ne reste plus à l'écran, ne vous inquiétez pas. Vous pouvez facilement retrouver le fichier à ouvrir

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2023-08-23 113422.png" alt=""><figcaption></figcaption></figure>

En cliquant sur les trois points situés en haut à gauche de votre écran, puis en sélectionnant l'option "Téléchargements".

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2023-08-23 113459.png" alt=""><figcaption></figcaption></figure>

Puis cliquer sur "<mark style="background-color:blue;">Installer</mark>" puis "<mark style="background-color:blue;">Ouvrir</mark>".&#x20;

L’application est mise à jour vous pouvez vous connecter. 👌

### **Téléchargement manuel**&#x20;

Pour télécharger manuellement le fichier APK de l'application Follow GT/Wiilog, suivez les étapes suivantes :

1. Ouvrez un navigateur internet sur votre terminal mobile Android.
2. Rendez-vous à l'adresse suivante : `https://{instance internet que vous souhaitez utiliser}/telecharger/nomade.apk`. Par exemple, si vous souhaitez effectuer les tests sur votre instance de recette, utilisez l'adresse `https://abc1-rec.follow-gt.fr/telecharger/nomade.apk`.
3. Le téléchargement du fichier APK s'effectue automatiquement.

Une fois les tests sur l'instance de recette terminés et que vous souhaitez réinstaller l'application de production sur votre terminal, procédez comme suit :

1. Désinstallez manuellement l'application de recette de votre terminal.
2. Ouvrez un navigateur internet sur votre terminal mobile Android.
3. Rendez-vous à l'adresse suivante : `https://abc1-prod.follow-gt.fr/telecharger/nomade.apk`.
4. Le téléchargement du fichier APK s'effectue automatiquement.
5. Une fois le fichier APK téléchargé, vous pouvez [l'installer sur votre terminal](premiers-pas.md#mise-a-jour-manuelle-procedure-de-mise-a-jour-de-lenvironnement-de-recette).

### Désinstaller Follow GT/Wiilog

Pour désinstaller l'application Follow GT/Wiilog de votre terminal Android, suivez les étapes suivantes :

1. Ouvrez le menu des applications de votre terminal.
2. Appuyez de manière prolongée sur l'icône de l'application Follow GT/Wiilog.
3. Appuyez sur "Désinstaller" pour confirmer la désinstallation de l'application.<br>

