---
description: Ensemble des paramétrages pour les demandes de livraison
---

# Livraisons

Cette partie sert à paramétrer le comportement de création d'une livraison

### **Création livraison**

* **Gérer le champ "Destination" en liste déroulante** : cochez ce paramétrage pour ne pas à avoir à taper une première lettre pour voir la liste des emplacements dans le champ Destination lors d'une création de demande de livraison (que ça soit via le +, le panier, ou une réception)
* **La livraison est directement préparée à sa validation** : L'ordre de livraison est directement mis en préparé et l'ordre de livraison est généré à la validation de la demande de livraison, sauf si les références / articles sur la demande sont sur des emplacements différents au moment de la validation de la demande livraison.
* **Ne pas gérer les quantités en stock** : Aucun contrôle de quantité ne sera effectué sur aucune des étapes de la livraison. Des articles seront générés automatiquement à la validation de la demande de livraison.
* **Faire le contrôle de la quantité au lancement de préparation :** Lorsque ce paramétrage est activé, les préparations créées seront visibles\
  uniquement sur la page **Ordre | Préparation - Planning**.<br>

### **Création livraison après réception**

* **"Demande de livraison" coché par défaut sur réception :** Lors d'une réception, la création d'une demande de livraison sera sélectionnée par défaut.
* **Comportement de la demande de livraison** : lors d'une réception, vous pouvez choisir un des 3 comportements suivants concernant la demande de livraison
  * **Création seulement de la demande de livraison en "A traiter"** : La demande de livraison sera créée sans préparation.
  * **Création de la demande de livraison avec sa préparation** : la demande sera automatiquement créée au statut A traiter avec l'ordre de préparation associé aussi au statut À traiter.
  * **Livraison directe : passage direct à l'ordre de livraison** : la demande de livraison se crée, l'ordre de préparation généré soit directement au statut Préparé et ainsi qu'un ordre de livraison soit automatiquement généré au statut A traiter. Cela permet ainsi d'éviter l'étape de préparation
  *
* **Le demandeur est l'utilisateur de la session en cours** : activez ce paramétrage pour que, lors d'une demande de livraison créée via l'étape de conditionnement d'une réception, le demandeur soit automatiquement rempli avec l'utilisateur de la session en cours

### Ajout référence <a href="#ajout-reference" id="ajout-reference"></a>

* **Faire apparaître l'emplacement cible de picking à l'ajout d'une référence et dans son traitement** : si vous activez ce paramétrage, lorsque vous ajoutez une référence gérée par article dans une demande de livraison, vous pourrez renseigner sur quel emplacement venir prélever la quantité demandée. Il sera présenté en priorité à l'opérateur qui effectue la préparation les articles présents sur l'emplacement de picking noté
* **Ajout d'unité logistique** : Deux possibilité de contenant dans les demandes de livraisons. Si ce paramétrage n'est pas coché, ce seront des références à ajouter, dans le cas contraire des unités logistiques.
* **Préremplir le champ commentaire de la ligne si le code projet de la référence est défini avec :** Possibilité d'intégrer les variable @Projet et @Destinataire.
* **Préremplir le champ commentaire de la ligne si le code projet de la référence n'est pas défini avec** : Possibilité d'intégrer la variable @Destinataire.
