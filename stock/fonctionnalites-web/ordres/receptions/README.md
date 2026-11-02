---
description: >-
  Enregistrer les attendus de réception, puis faire entrer en stock les
  références et articles reçus.
---

# Réceptions

**Chemin :** Ordre › Réception · Web uniquement

Une réception fait entrer des références et des articles en stock. Vous pouvez la créer à l'avance (attendu de réception), l'importer via [Imports & mises à jour](../../../../parametrages/donnees/imports-and-mises-a-jour.md), ou la créer depuis un [arrivage UL](../../../../trace/fonctionnalites-web/arrivages-unites-logistiques/) (action **Réceptionner**) ou une [demande d'achat](../../demandes/achats.md) terminée.

Le traitement d'une réception (ajout des références, réception des quantités) est décrit dans [Détail réception](detail-reception.md).

## Créer une réception

1. Cliquez sur **Nouvelle réception**.
2. Renseignez l'**Emplacement** de réception (obligatoire) : les références y seront déposées par défaut.
3. Complétez si besoin (selon les [champs fixes](../../../parametrage/receptions.md#champs-fixes) paramétrés) :
   * **Date commande**, **Date attendue**, **Numéro(s) de commande** ;
   * **Fournisseur**, **Transporteur** : s'ils n'existent pas, cliquez sur **Créer** et renseignez le **Nom** et le **Code** ;
   * **Emplacement de stockage** : destination des demandes de transfert créées depuis la réception ;
   * **Anomalie** : la réception passe au statut _Anomalie_ ;
   * **Urgence ?** : la réception est signalée comme urgente (ligne rouge dans la liste) ;
   * **Commentaire**, **Pièces jointes** (bon de livraison, par exemple) et champs libres.
4. Cliquez sur **Enregistrer**.

## Les statuts d'une réception

| Statut                      | Signification                                                          |
| --------------------------- | ---------------------------------------------------------------------- |
| **En attente de réception** | Créée, en attente des marchandises.                                    |
| **Anomalie**                | Un problème a été signalé sur la réception.                            |
| **Réception totale**        | Terminée avec **Finir la réception**.                                  |
| **Réception partielle**     | Annulée après avoir été terminée : elle peut être complétée à nouveau. |

## Retrouver une réception

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Fournisseurs**, **Date attendue**, **N° de commande**, **Créé par**. Les filtres proposés dépendent des champs fixes paramétrés.
* La flèche à côté de **Nouvelle réception** donne accès à **Exporter au format CSV** et à **Gestion des colonnes**.

<details>

<summary>Colonnes disponibles</summary>

| Colonne                                            | Description                                                         |
| -------------------------------------------------- | ------------------------------------------------------------------- |
| **Date création**, **Date attendue**, **Date fin** | Dates clés. La date de fin est remplie avec **Finir la réception**. |
| **N° de réception**                                | **R** + date + compteur.                                            |
| **Numéro(s) commande**, **Fournisseur**            | Informations de la commande.                                        |
| **Statut**                                         | Voir ci-dessus.                                                     |
| **Emplacement de stockage**                        | Destination des transferts créés depuis la réception.               |
| **Commentaire**                                    | Commentaire de la réception.                                        |
| **Type(s) de demande de livraison liée(s)**        | Types des livraisons créées depuis la réception.                    |
| **Frais de livraison**                             | Frais renseignés.                                                   |
| **Créé par**                                       | Auteur de la réception.                                             |
| **Destinataire(s)**                                | Demandeurs des livraisons créées depuis la réception.               |

</details>
