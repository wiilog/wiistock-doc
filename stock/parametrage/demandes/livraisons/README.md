---
description: Comportement des demandes de livraison à la création.
---

# Livraisons

**Chemin :** Paramétrage › Stock › Demandes › Livraisons

### Création livraison

| Paramètre                                                        | Effet                                                                                                                                                                           |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Gérer le champ "Destination" en liste déroulante**             | La liste des emplacements s'affiche sans avoir à taper une première lettre (création via +, panier ou réception).                                                               |
| **La livraison est directement préparée à sa validation**        | L'ordre de préparation passe directement en _Préparé_ et l'ordre de livraison est généré à la validation, sauf si les références/articles sont sur des emplacements différents. |
| **Faire le contrôle de la quantité au lancement de préparation** | Les préparations créées ne sont visibles que dans **Ordre › Préparation - Planning**.                                                                                           |
| **Ne pas gérer les quantités en stock**                          | Aucun contrôle de quantité à aucune étape. Des articles sont générés automatiquement à la validation (fonctionne aussi pour les références gérées à la référence).              |

### Création livraison après réception

* **"Demande de livraison" coché par défaut sur réception** : la création d'une demande de livraison est pré-cochée lors d'une réception.
* **Comportement de la demande de livraison** :

| Option                                                           | Résultat                                                                                                    |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Création seulement de la demande de livraison en "A traiter"** | Pas d'ordre de préparation créé.                                                                            |
| **Création de la demande de livraison avec sa préparation**      | Demande et ordre de préparation en _À traiter_.                                                             |
| **Livraison directe : passage direct à l'ordre de livraison**    | Demande et préparation en _Préparé_, ordre de livraison en _À traiter_ : l'étape de préparation est sautée. |

### Ajout référence

* **Faire apparaître l'emplacement cible de picking à l'ajout d'une référence et dans son traitement** : pour une référence gérée par article, on indique l'emplacement où prélever. Les articles de cet emplacement sont proposés en priorité au préparateur.
* **Ajout d'unité logistique** : la demande contient des unités logistiques au lieu de références.
* **Préremplir le champ commentaire de la ligne si le code projet de la référence est défini avec** : texte qui peut contenir **@Projet** et **@Destinataire**.
* **Préremplir le champ commentaire de la ligne si le code projet de la référence n'est pas défini avec** : texte qui peut contenir **@Destinataire**.

Cliquez sur **Enregistrer** pour valider.
