---
description: Utiliser vos propres modèles Word pour les documents générés par FollowGT.
---

# Modèles de document

**Chemin :** Paramétrage › Modèles de document

Pour chaque document, FollowGT propose un **modèle par défaut** (fichier .dotx, téléchargeable). Vous pouvez le remplacer par un **modèle personnalisé** : un fichier Word contenant des **variables** `${...}`, remplacées par les données au moment de la génération. La liste des variables disponibles est affichée sur chaque page.

| Rubrique          | Document                                                                                                                                                   | Variables                                                                                                                                                                 |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Acheminements** | Lettre de voiture : **modèle standard** et **modèle avec rupture à l'arrivage**.                                                                           | Champs de l'acheminement (`${numach}`, `${typeach}`, `${transporteurach}`…), liste des UL (`${UL}`, `${nature}`, `${poids}`…), champs du formulaire de lettre de voiture. |
| **Livraisons**    | Bon de préparation (appelé « lettre de voiture » à l'écran), généré depuis un [ordre de préparation](../stock/fonctionnalites-web/ordres/preparations.md). | Champs de la livraison (`${numordreliv}`, `${typeliv}`, `${demandeurliv}`…) et liste des UL.                                                                              |
| **Achats**        | Bon de commande, généré depuis une [demande d'achat](../stock/fonctionnalites-web/demandes/achats.md).                                                     | Fournisseur, frais de livraison, prix total, et liste des références (`${reference}`, `${prixunitaire}`, `${quantitecommandee}`…).                                        |

{% hint style="info" %}
Sans modèle personnalisé, le modèle par défaut est utilisé.
{% endhint %}

**Bon de commande :** la génération peut faire passer la demande d'achat au statut suivant (option **Passage au statut à la génération du bon de commande** dans les [statuts d'achat](../stock/parametrage/demandes/achats/statuts.md)). Le rôle doit avoir le droit **Afficher achats**.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FUZVCgLS7FVWhrtn8BLmZ%2Fimage.png?alt=media&#x26;token=d34bed0a-cb9e-4280-91f3-479a976f86b4" alt="Bon de préparation"><figcaption><p>Bon de préparation</p></figcaption></figure>
