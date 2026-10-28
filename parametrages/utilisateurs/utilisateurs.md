# Utilisateurs

Chaque personne qui utilise Follow GT a besoin d'un compte utilisateur rattaché à un [rôle](roles/). Le rôle détermine les fonctionnalités accessibles.

Pour une personne qui doit seulement recevoir des emails ou des colis, sans se connecter, créez plutôt un [contact](../../referentiel/contacts.md).

{% hint style="info" %}
Si votre entreprise utilise la [connexion SSO](connexion-sso.md), la création de compte depuis la page de connexion et le « mot de passe oublié » sont gérés par votre fournisseur d'identité.
{% endhint %}

### Créer un utilisateur

#### Depuis le paramétrage

Allez dans **Paramétrage | Utilisateurs | Utilisateurs** et cliquez sur **Nouvel utilisateur**.

| Champ                                | Description                                                                                                                                                        |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Statut**                           | Actif ou inactif. Un utilisateur inactif ne peut plus se connecter.                                                                                                |
| **Rôle**                             | Donne accès aux fonctionnalités.                                                                                                                                   |
| **Nom d'utilisateur**                | Nom affiché dans l'application et identifiant sur le **nomade**. Doit être unique.                                                                                 |
| **Email**                            | Identifiant sur le **web** et adresse de réception des notifications. Doit être unique. Le bouton « ajouter un mail » permet d'ajouter 2 adresses supplémentaires. |
| **Mot de passe** / **Confirmer**     | 8 caractères minimum, dont 1 caractère spécial, 1 chiffre et 1 majuscule.                                                                                          |
| **Clé de connexion nomade**          | Mot de passe de l'application nomade, entre 14 et 24 caractères.                                                                                                   |
| **Numéro de téléphone**, **Adresse** | Coordonnées de l'utilisateur.                                                                                                                                      |
| **Langue**                           | Langue de l'application (français ou anglais par défaut).                                                                                                          |
| **Format de date**                   | jj/mm/aaaa, mm/dd/yyyy ou yyyy/mm/dd.                                                                                                                              |
| **Types de demandes visibles**       | Types de livraison, d'acheminement, de service, de **production** et de **tournée** visibles par l'utilisateur. Voir ci-dessous.                                   |
| **Groupe de visibilité**             | Limite les références du stock visibles. Sans groupe, l'utilisateur voit toutes les références.                                                                    |
| **Dropzone**                         | Emplacement affecté à l'utilisateur pour les arrivages de traçabilité. Si l'utilisateur est acheteur, la dropzone figure sur l'étiquette d'unité de tracking.      |
| **Code signataire**                  | Code PIN à 4 caractères pour signer les acheminements groupés.                                                                                                     |
| **Livreur**                          | Indique un chauffeur-livreur du module Track.                                                                                                                      |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FSsXo4sEAGNoC5Hmat3Rr%2Fimage.png?alt=media&#x26;token=d450edc5-abc8-4a93-b26e-17756fddbe43" alt=""><figcaption></figcaption></figure>

**Filtrer les types de demandes visibles**

Ces champs limitent les types de demandes que l'utilisateur voit. Quand un champ est vide :

| Champ                            | Web                     | Nomade             |
| -------------------------------- | ----------------------- | ------------------ |
| Livraison, acheminement, service | Tous les types visibles | Aucun type visible |
| Production                       | Tous les types visibles | Sans objet         |
| Tournée                          | Tous les types visibles | Aucun type visible |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FQkJaD4zCNSmyJq3kXqmN%2Fimage.png?alt=media&#x26;token=f6ff6a61-8249-44ef-9725-6b192fe61cbb" alt=""><figcaption></figcaption></figure>

#### Depuis la page de connexion (hors SSO)

Le bouton **Créer un compte** ouvre un formulaire limité : nom d'utilisateur, adresse email, mot de passe, langue et format de date.

Le compte créé reçoit le rôle **Aucun accès**. L'administrateur reçoit un email de demande de compte : le lien de cet email ouvre la fiche de l'utilisateur pour lui attribuer un rôle et compléter son paramétrage.

#### Par import

1. Allez dans **Paramétrage | Données | Imports & mises à jour** et cliquez sur **Ajouter un import**.
2. Choisissez le type de données **Utilisateurs**.
3. Téléchargez le modèle vide, complétez-le, puis ajoutez-le en pièce jointe (CSV encodé en UTF-8).

{% hint style="info" %}
Les utilisateurs importés reçoivent un mot de passe aléatoire. Ils le définissent avec **Mot de passe oublié** (hors SSO).
{% endhint %}

### Modifier un utilisateur

Cliquez sur la ligne de l'utilisateur. Tous les champs sont modifiables, mais il est déconseillé de modifier l'email. La réinitialisation du mot de passe se fait aussi depuis ce formulaire.

### Supprimer ou désactiver un utilisateur

Cliquez sur la corbeille à droite de la ligne. La suppression n'est possible que si l'utilisateur ne s'est jamais connecté et n'a créé aucune donnée (arrivage, demande, mouvement…).

Sinon, passez son statut à **inactif**. Il ne peut alors plus se connecter ni être sélectionné comme destinataire ou acheteur.

### Mot de passe oublié (hors SSO)

1. Sur la page de connexion, remplissez le formulaire **Mot de passe oublié**.
2. Cliquez sur le lien temporaire reçu par email.
3. Saisissez votre nouveau mot de passe.
