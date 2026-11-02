---
description: >-
  Enregistrer les colis, palettes et autres unités logistiques (UL) reçus sur
  votre site, puis imprimer leurs étiquettes.
---

# Arrivages Unités Logistiques

**Chemin :** Traçabilité › Arrivages UL · Web uniquement

Un arrivage UL enregistre une livraison reçue sur votre site : qui l'a apportée (fournisseur, transporteur), à qui elle est destinée et combien d'unités logistiques (UL) elle contient. À l'enregistrement, Follow GT crée les UL, les dépose sur l'emplacement de dépose et génère leurs étiquettes.

<figure><img src="../../../.gitbook/assets/Capture d’écran 2025-08-14 à 10.26.04.png" alt="Liste des arrivages UL"><figcaption></figcaption></figure>

## Créer un arrivage UL

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur **Nouvel arrivage UL**.
{% endstep %}

{% step %}
### Renseigner l'arrivage

Remplissez au minimum les champs obligatoires, marqués d'un astérisque : **Type**, **Statut** et **Emplacement de dépose** (ainsi que le **Transporteur** s'il est obligatoire sur votre instance).

Le fournisseur, le transporteur ou le chauffeur n'existe pas encore ? Cliquez sur **Créer** à côté du champ pour l'ajouter au référentiel.
{% endstep %}

{% step %}
### Indiquer le nombre d'UL

Dans **Nombre d'unités logistiques à ajouter**, saisissez une quantité pour chaque nature reçue (Colis, Palettes…).
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**. Si la case **Impression UL** est cochée, les étiquettes des UL sont générées automatiquement. Avec [WiiSpool](../../../services-externes/wiispool-v3.md) installé sur votre poste, elles partent directement à l'impression.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Un message peut s'afficher avant l'impression :**

* **Fournisseur possible douane** : cliquez sur **Oui** pour revenir au formulaire et cocher **Douane**, ou sur **Non** pour continuer.
* **Fournisseur urgent** ou **N° de commande urgent** : cliquez sur **Continuer**. L'arrivage est enregistré et passe en urgence.

Ces règles se définissent dans [Référentiel › Fournisseurs](../../../referentiel/fournisseurs.md) et dans [Urgences](../urgences.md). Si les deux contrôles s'appliquent, le message douane s'affiche en premier.
{% endhint %}

<details>

<summary>Détail des champs du formulaire</summary>

Les champs affichés et obligatoires se règlent dans [Paramétrage › Trace › Arrivages UL › Champs fixes](../../parametrage/arrivages-ul/champs-fixes.md).

| Champ                                     | À quoi il sert                                                                                                                                                                                     |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Fournisseur**                           | Fournisseur de la marchandise, issu du [référentiel Fournisseurs](../../../referentiel/fournisseurs.md).                                                                                           |
| **Transporteur**                          | Transporteur qui a livré, issu du [référentiel Transporteurs](../../../referentiel/transporteurs.md).                                                                                              |
| **Chauffeur**                             | Chauffeur qui a livré, issu du [référentiel Chauffeurs](../../../referentiel/chauffeurs.md).                                                                                                       |
| **N° tracking transporteur**              | Numéro de suivi du transporteur.                                                                                                                                                                   |
| **N° arrivage camion**                    | Rattache l'arrivage UL à un [arrivage camion](../../parametrage/arrivages-camion/) existant.                                                                                                       |
| **N° commande / BL**                      | Un ou plusieurs numéros de commande ou de bon de livraison. Validez chaque numéro avec **Entrée**.                                                                                                 |
| **Type** \*                               | Type d'arrivage. Il est prérempli s'il n'en existe qu'un. Voir [Types et champs libres](../../parametrage/arrivages-ul/types-et-champs-libres.md).                                                 |
| **Statut** \*                             | Statut de l'arrivage, qui dépend du type. Voir [Statuts](../../parametrage/arrivages-ul/statuts.md).                                                                                               |
| **Emplacement de dépose** \*              | Emplacement où les UL sont déposées automatiquement. Par défaut, c'est celui défini dans [Configurations](../../parametrage/arrivages-ul/configurations.md).                                       |
| **Destinataire(s)**                       | Personnes à qui les UL sont destinées. Elles peuvent recevoir un mail à la création de l'arrivage, puis à la dépose sur un point de livraison.                                                     |
| **Acheteur(s)**                           | Acheteurs concernés, notamment utiles en cas de litige.                                                                                                                                            |
| **Numéro de projet**                      | Texte libre.                                                                                                                                                                                       |
| **Business unit**                         | Liste de valeurs définie dans les champs fixes.                                                                                                                                                    |
| **Douane**                                | Signale des colis à dédouaner. Selon votre paramétrage, les UL vont sur un emplacement dédié et leurs étiquettes portent une mention spéciale.                                                     |
| **Congelé**                               | Signale des colis congelés.                                                                                                                                                                        |
| **Impression UL**                         | Imprime les étiquettes des UL dès l'enregistrement. Pour la cocher par défaut : option **Impressions cochées par défaut** dans [Configurations](../../parametrage/arrivages-ul/configurations.md). |
| **Nombre d'unités logistiques à ajouter** | Une quantité par nature d'UL. Voir [Natures](../../../referentiel/natures.md).                                                                                                                     |
| **Projet**                                | Projet issu du [référentiel Projets](../../../referentiel/projets.md).                                                                                                                             |
| **Champs libres**                         | Champs propres à votre activité, définis par type d'arrivage.                                                                                                                                      |
| **Commentaire**, **Pièces jointes**       | Informations complémentaires et documents. Une photo peut être prise directement.                                                                                                                  |

</details>

## Retrouver un arrivage

* Utilisez la **barre de filtres**, puis cliquez sur **Filtrer**. Vos filtres sont conservés d'une session à l'autre ; **Effacer** les réinitialise.
* Pour une recherche rapide dans le tableau, utilisez le champ **Rechercher**.
* Pour choisir les colonnes affichées, ouvrez la flèche à côté de **Nouvel arrivage UL**, puis **Gestion des colonnes**.

<details>

<summary>Filtres disponibles</summary>

Dates de création (**Du** / **Au**), **Type**, **Statuts**, **N° d'arrivage UL**, **N° d'arrivage camion**, **Douane ?**, **Congelé ?**, **Urgence ?**, **Fournisseurs**, **Transporteur**, **Destinataires**, **Emplacement de dépose**, **Business unit**, **Numéro de projet**, **Numéro de tracking**, **N° commande / BL**.

Les filtres proposés dépendent des champs affichés dans [Champs fixes](../../parametrage/arrivages-ul/champs-fixes.md).

</details>

## Agir sur un arrivage

| Action                     | Où la trouver                           | Résultat                                                                                                                          |
| -------------------------- | --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Voir**                   | Clic sur la ligne                       | Ouvre le [détail de l'arrivage](details-arrivage.md).                                                                             |
| **Impression**             | Menu **⋮** de la ligne                  | Réimprime les étiquettes des UL.                                                                                                  |
| **Réceptionner**           | Menu **⋮** de la ligne                  | Crée une [réception](../../../stock/fonctionnalites-web/ordres/receptions/) Stock préremplie avec les informations de l'arrivage. |
| **Exporter au format CSV** | Flèche à côté de **Nouvel arrivage UL** | Exporte les arrivages filtrés.                                                                                                    |

## Acheminer un ou plusieurs arrivages

Pour envoyer les UL d'un ou plusieurs arrivages vers un autre lieu, créez une [demande d'acheminement](../demandes/acheminements/).

{% stepper %}
{% step %}
### Passer en mode acheminement

Filtrez d'abord si besoin : les filtres disparaissent dans ce mode. Ouvrez ensuite la flèche à côté de **Nouvel arrivage UL** et cliquez sur **Acheminer**.
{% endstep %}

{% step %}
### Sélectionner les arrivages

Cochez les arrivages concernés. L'icône ⇄ signale un arrivage déjà acheminé. Cliquez ensuite sur **Valider arrivages à acheminer**.

<figure><img src="../../../.gitbook/assets/Capture d’écran 2025-08-14 à 10.48.48.png" alt="Sélection des arrivages à acheminer"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Créer ou compléter la demande

Choisissez de créer une demande ou d'ajouter les UL à une demande existante (elle doit être au statut brouillon et créée par vous). Vous pouvez ajuster la liste des UL : quantité, commentaire, suppression. Cliquez sur **Enregistrer**.
{% endstep %}

{% step %}
### Valider la demande

Vous arrivez sur la demande, au statut brouillon. Cliquez sur **Valider la demande** pour qu'elle soit traitée par vos opérateurs.
{% endstep %}
{% endstepper %}

Pour quitter le mode acheminement sans rien créer, cliquez sur **Annuler acheminer**.

## Envoyer la liste des UL par mail

Le destinataire peut recevoir par mail la liste des UL de l'arrivage, chacune avec son QR code. Les opérateurs le scannent avec le menu **Lecture** du nomade pour afficher les informations de l'UL.

Activez l'option **Envoyer email après nouvel arrivage** dans [Paramétrage › Trace › Arrivages UL › Configurations](../../parametrage/arrivages-ul/configurations.md).

<figure><img src="../../../.gitbook/assets/image (14) (2).png" alt="Mail avec la liste des UL"><figcaption></figcaption></figure>

{% hint style="warning" %}
Au-delà de 15 UL, les QR codes ne sont plus affichés dans le mail.
{% endhint %}
