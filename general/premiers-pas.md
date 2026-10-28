# Premiers pas

### 1. Accéder à vos instances

Wiilog crée deux instances pour vous :

| Instance   | Adresse (exemple)                | Usage                        |
| ---------- | -------------------------------- | ---------------------------- |
| Production | `https://abc1-prod.follow-gt.fr` | Utilisation quotidienne      |
| Recette    | `https://abc1-rec.follow-gt.fr`  | Tests des nouvelles versions |

Sur le web, l'identifiant est votre **adresse email**. Sur l'application nomade, c'est votre **clé de connexion nomade**.

{% hint style="info" %}
**Connexion SSO** : si votre entreprise utilise un fournisseur d'identité et que la connexion SSO est paramétrée sur votre instance, saisissez votre adresse email : vous êtes redirigé vers sa page de connexion. La création de compte et le « mot de passe oublié » sont alors gérés par votre fournisseur d'identité. Voir [Connexion SSO](../parametrages/utilisateurs/connexion-sso.md).
{% endhint %}

Pour votre premier compte (hors SSO), cliquez sur **"Demandez-en un maintenant"** sur la page de connexion. Votre administrateur recevra votre demande, vous attribue un rôle et vous informe de l'activation de votre compte utilisateur.

<figure><img src="../.gitbook/assets/image (204).png" alt=""><figcaption></figcaption></figure>

### 2. Créer des utilisateurs

| Méthode                                                    | Quand l'utiliser                                                                               |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Demander un compte** sur la page de connexion (hors SSO) | L'utilisateur demande lui-même son compte. L'administrateur l'active et lui attribue un rôle.  |
| **Paramétrage › Utilisateurs › Nouvel utilisateur**        | Création d'un seul utilisateur                                                                 |
| **Paramétrage › Données › Imports & mises à jour**         | Création en masse (fichier CSV encodé en UTF-8)                                                |

Le détail des champs et des procédures se trouve dans [Utilisateurs](../parametrages/utilisateurs/utilisateurs.md).

### 3. Installer et mettre à jour l'application nomade (Android Zebra)

#### Mise à jour automatique

Quand une mise à jour est nécessaire, un écran dédié s'affiche à la connexion.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FzXyLTrXiXClbtMv7l0Kv%2FCapture%20d&#x27;%C3%A9cran%202023-08-23%20113102.png?alt=media&#x26;token=0ebb04b7-a96e-4623-9d97-3a1baf70dd75" alt="Écran de mise à jour"><figcaption></figcaption></figure>

1. Lancez le téléchargement. Si l'application a déjà été mise à jour sur ce terminal, cliquez sur **Retélécharger**.
2. À la fin du téléchargement, cliquez sur **Ouvrir**, puis **Installer** et **Ouvrir**.

{% hint style="info" %}
La fenêtre de téléchargement a disparu ? Ouvrez le menu **⋮** en haut à gauche, puis **Téléchargements**, et ouvrez le fichier.
{% endhint %}

#### Installation manuelle

1. Sur le terminal, ouvrez un navigateur internet.
2. Allez à l'adresse `https://{votre-instance}/telecharger/nomade.apk`, par exemple `https://abc1-rec.follow-gt.fr/telecharger/nomade.apk`.
3. Le fichier APK se télécharge automatiquement. Ouvrez-le, puis cliquez sur **Installer**.

#### Passer de la recette à la production

1. [Désinstallez](premiers-pas.md#desinstaller-lapplication) l'application de recette.
2. Suivez l'[installation manuelle](premiers-pas.md#installation-manuelle) avec l'adresse `https://abc1-prod.follow-gt.fr/telecharger/nomade.apk`.

#### Désinstaller l'application

1. Ouvrez le menu des applications du terminal.
2. Faites un appui long sur l'icône Follow GT / Wiilog.
3. Appuyez sur **Désinstaller**.
