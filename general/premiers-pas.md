# Premiers pas

## Premiers pas

### 1. Accéder à vos instances

Wiilog crée deux instances pour vous :

| Instance   | Adresse (exemple)                | Usage                        |
| ---------- | -------------------------------- | ---------------------------- |
| Production | `https://abc1-prod.follow-gt.fr` | Utilisation quotidienne      |
| Recette    | `https://abc1-rec.follow-gt.fr`  | Tests des nouvelles versions |

Pour créer votre premier compte, cliquez sur **Créer un compte** sur la page de connexion, puis demandez à Wiilog de vous attribuer un rôle. Les rôles se paramètrent ensuite avec Wiilog, selon les fonctionnalités que vous utilisez.

{% embed url="https://www.screencast.com/t/qqKcGidIT" %}

### 2. Créer des utilisateurs

Choisissez la méthode qui vous convient :

| Méthode                                            | Quand l'utiliser                       | Procédure                                                                                                                                                                                    |
| -------------------------------------------------- | -------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Page de connexion**                              | L'utilisateur crée lui-même son compte | 1. L'utilisateur clique sur **Créer un compte**. 2. Un administrateur lui attribue un rôle et valide son compte.                                                                             |
| **Paramétrage › Utilisateurs**                     | Création d'un seul utilisateur         | 1. Cliquez sur **Nouvel utilisateur**. 2. Remplissez le formulaire. 3. Cochez **Statut actif** et attribuez un rôle.                                                                         |
| **Paramétrage › Données › Imports & mises à jour** | Création en masse                      | 1. Cliquez sur **+ Nouvel import**. 2. Choisissez le type de données **Utilisateur**. 3. Téléchargez le modèle avec **Télécharger**, remplissez-le, puis importez-le en CSV encodé en UTF-8. |

{% hint style="info" %}
Les méthodes 2 et 3, ainsi que la validation des comptes, nécessitent un rôle disposant des droits correspondants.
{% endhint %}

### 3. Installer et mettre à jour l'application nomade (Android Zebra)

#### Mise à jour automatique

Quand une mise à jour est nécessaire, un écran dédié s'affiche à la connexion.

1. Lancez le téléchargement. Si l'application a déjà été mise à jour sur ce terminal, cliquez sur **Retélécharger**.
2. À la fin du téléchargement, cliquez sur **Ouvrir**, puis **Installer** et **Ouvrir**.

\[capture : écran de mise à jour]

{% hint style="info" %}
La fenêtre de téléchargement a disparu ? Ouvrez le menu **⋮** en haut à gauche, puis **Téléchargements**, et ouvrez le fichier.
{% endhint %}

#### Installation manuelle

1. Sur le terminal, ouvrez un navigateur internet.
2. Allez à l'adresse `https://{votre-instance}/telecharger/nomade.apk`, par exemple `https://abc1-rec.follow-gt.fr/telecharger/nomade.apk`.
3. Le fichier APK se télécharge automatiquement. Ouvrez-le, puis cliquez sur **Installer**.

#### Passer de la recette à la production

1. Désinstallez l'application de recette.
2. Installez l'application de production en suivant l'installation manuelle avec l'adresse `https://abc1-prod.follow-gt.fr/telecharger/nomade.apk`.

#### Désinstaller l'application

1. Ouvrez le menu des applications du terminal.
2. Faites un appui long sur l'icône Follow GT / Wiilog.
3. Appuyez sur **Désinstaller**.

