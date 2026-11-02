---
description: Workflow des demandes d'achat.
---

# Statuts

**Chemin :** Paramétrage › Stock › Demandes › Achats - Statuts

Une demande d'achat passe par une succession de statuts. Cliquez sur **Ajouter** (ou sur une ligne pour la modifier) et remplissez :

| Colonne                                                              | Description                                                                                                                                                                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Libellé\***                                                        | Nom du statut.                                                                                                                                                                                                |
| **État\***                                                           | **Brouillon** (on peut encore ajouter des références), **À traiter** (demande validée, date de validation), **En cours** (prise en compte par l'acheteur), **Traité** (demande terminée, date de traitement). |
| **Statut par défaut**                                                | Statut appliqué à la création.                                                                                                                                                                                |
| **Envoi d'emails à l'acheteur**                                      | Email aux acheteurs des références au passage à ce statut.                                                                                                                                                    |
| **Envoi d'emails au demandeur**                                      | Email au demandeur au passage à ce statut.                                                                                                                                                                    |
| **Blocage du changement de statut si frais de livraison non rempli** | Impossible de passer à ce statut tant que les frais de livraison ne sont pas renseignés.                                                                                                                      |
| **Passage au statut à la génération du bon de commande**             | La demande passe automatiquement à ce statut quand le bon de commande est généré.                                                                                                                             |
| **Création automatique d'une réception**                             | (État Traité) Une réception est créée avec les informations de la demande.                                                                                                                                    |
| **Ordre\***                                                          | Position du statut dans la liste.                                                                                                                                                                             |

{% hint style="info" %}
Pour un workflow cohérent, prévoyez au moins un statut par état : Brouillon, À traiter, En cours et Traité.
{% endhint %}

Un statut utilisé sur une demande d'achat ne peut pas être supprimé. Cliquez sur **Enregistrer** pour valider.
