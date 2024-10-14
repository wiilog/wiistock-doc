# Utilisateurs

Pour donner accès aux managers ou opérateurs sur l'application, vous devez leur créer des comptes utilisateurs. Vous pouvez soit créer tous les comptes utilisateurs 1 à 1, soit les importer en masse via les import, soit demander aux utilisateurs de valider le formulaire de création de compte disponible depuis l'écran d'authentification de l'application.

Le compte utilisateur est ensuite rattaché à un rôle lui permettant d'accéder à certaines fonctionnalités de l'application. ([Voir Utilisateurs | Roles](roles/))

### Créer un nouvelle utilisateur

#### Depuis l'interface de paramétrage

Allez dans utilisateur (sous-menu d'utilisateur) et cliquez sur le bouton "nouvel utilisateur". Le formulaire de création s'ouvre et vous propose de saisir les informations suivantes :

* **Statut :** Vous avez la possibilité de rendre l'utilisateur inactif, cela peut être utile si vous ne pouvez pas le supprimer
* **Rôle** : Permet d'affecter un rôle à l'utilisateur pour lui donner accès à certaines fonctionnalités de l'application
* **Nom d'utilisateur** : nom affiché dans la barre de menu de l'application, sert de login sur l'application nomade et doit donc être unique
* **Email** : Il doit correspondre à votre email pour recevoir les emails de notification sur les différentes actions de l'application, sert de login sur l'application web et doit donc être unique. Vous avez la possibilité d'en ajouter 2 en plus en cliquant sur "ajouter un mail".
* **Mot de passe** : la saisie de mot de passe doit respecter les contraintes suivantes
  * minimum 8 caractères
  * 1 caractère spécial
  * 1 chiffre
  * 1 majuscule
* **Confirmer mot de passe** : Permet de ressaisir le mot de passe pour valider qu'il n'y a pas eu d'erreur de saisie
* **Clé de connexion nomade** : mot de passe utilisé pour le nomade&#x20;
  * La longueur doit être comprise entre 14 et 24 caractères.
* **Numéro de téléphone** : renseignez le numéro de téléphone de l'utilisateur
* **Adresse** : Renseignez l'adresse de l'utilisateur
* **Langue** : sélectionner la langue de l'application, par défaut vous avez le choix entre français et anglais.
* **Format de date** : le sens dans lequel vont s'afficher les dates dans l'application. Vous avez le choix entre 3 formats : jj/mm/aaaa, mm/dd/yyyy et yyyy/mm/dd.
* **Type livraison, acheminement, service** : Permet de préciser les Type de demandes visibles par l'utilisateur. Ainsi l'opérateur pourra traiter tous les types renseignés (Cela permet de cacher les autres types de demandes de livraison sur l'application mobile)
* **Groupe de visibilité** : Permet de donner accès aux utilisateurs seulement à certaines références du stock en fonction du groupe de visibilité attribué.

{% hint style="info" %}
Si un utilisateur n'a aucun groupe de visibilité, il peut voir toutes les références peu importe leur groupe de visibilité.
{% endhint %}

* **Dropzone** : Permet d'affecter un emplacement à un utilisateur. Cette fonctionnalité est utilisée sur les arrivages de traçabilité. Si l'utilisateur est positionné en acheteur, alors l'emplacement dropzone sera affiché sur l'étiquette d'unité de tracking

Une fois enregistré, le rôle est modifiable depuis la liste des utilisateurs.

{% embed url="https://www.screencast.com/t/IJVEnrwaIQq" %}

#### Depuis l'interface de connexion

Depuis l'écran d'authentification de l'application, un bouton <mark style="background-color:blue;">**Créer un compte**</mark> redirige vers un formulaire de création de compte.

Ce formulaire est limité et permet seulement une saisie des champs suivants :

* Nom d'utilisateur
* Adresse email
* Mot de passe
* Confirmer mot de passe
* Langue
* Format de date

Une fois créé, l'utilisateur pourra s'authentifier pour entrer dans l'application et sera rattaché au rôle automatique **Aucun accès**. Les administrateurs pourront ensuite affecter le bon rôle et compléter le paramétrage de l'utilisateur.

#### Depuis l'import des utilisateurs

Dans le paramétrage aller dans Imports & mises à jour (sous-menu de données), cliquez sur le bouton "<mark style="background-color:blue;">**Ajouter un import**</mark>", dans le formualire vous allez choisir dans **type de données à importer** : utilisateurs. Vous pouvez télécharger un fichier de modèle d'import pour les utilisateurs vide, le compléter et l'uploader dans pièces jointes.

{% hint style="info" %}
Les nouveaux utilisateurs seront créés avec un mot de passe aléatoire. Ils devront configurer ce dernier via la fonctionnalité "**Mot de passe oublié**".
{% endhint %}

### Modifier un utilisateur

Pour modifier un utilisateur cliquer simplement sur sa ligne, le formulaire apparaitra.

Il n'est pas recommandé de modifier l'email d'un utilisateur. Tous les autres champs peuvent être modifiés. La réinitialisation de mot de passe est possible depuis la modification de l'utilisateur.

### Supprimer ou désactiver un utilisateur <a href="#supprimer-ou-desactiver-un-utilisateur" id="supprimer-ou-desactiver-un-utilisateur"></a>

Pour supprimer un utilisateur cliquer sur la corbeille à droite dans la liste des utilisateurs.

Un utilisateur peut être supprimé s'il n'a jamais créé d'informations liées à son profil (ex : arrivage / demandes / mouvements / autres )

**Si l'utilisateur est lié à des données, il n'est plus possible de le supprimer.** Dans ce cas, il est possible de le désactiver en passant son statut d'actif à inactif.

La désactivation d'un utilisateur restreint :

* La possibilité de se connecter sur l'application
* Sa sélection dans les champs destinataires / acheteurs

### Mot de passe oublié

Une fonction de mot de passe oublié permet à l'utilisateur de réinitialiser son mot de passe.

1. Depuis l'écran d'authentification, vous devez valider le formulaire de mot de passe oublié. L'application envoie ensuite un lien temporaire chiffré sur votre boite email comportant un lien redirigeant vers un formulaire de réinitialisation de mot de passe.
2. Vous cliquez sur le lien se trouvant dans le mail puis validez le formulaire en saisissant un nouveau mot de passe.
3. le mot de passe est maintenant réinitialisé et vous pouvez à nouveau vous connecter sur l'application.
