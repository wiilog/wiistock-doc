---
description: Mise en production du 21/02/2024
---

# Mise à jour - Suivi d'OF, Préparation nomade, gestionnaire d'emplacement et évolution dashboard

### Suivi des ordres de fabrication - demande de production

 _Ce projet est utilisé pour le suivi des ordres de fabrication sur une vue planning. Vous pourrez paramétrer un workflow de vie d'un OF mais aussi le gérer en tant réel sur une tablette ou un écran tactile via du drag and drop._&#x20;

* WEB - Paramétrage | Rôle | Production&#x20;
  * Nouveaux droits de création / modification / suppressions de demande de production.&#x20;
  * Nouveau droit de visualisation de la vue planning des ordres de fabrication.
  * Nouveau droit de changement de la date attendue des ordres de fabrication.
* WEB - Paramétrage | Rôle | Paramétrage - production&#x20;
  * Nouveau droit d'accès au paramétrage des demandes de production
* WEB - Paramétrage | Production | Paramétrage complet :&#x20;
  * Configuration : Ajout de réceptions de mails si urgence d'une demande.&#x20;
  * Statuts : Nouvelle page d'ajout de statuts visibles sur vue planning ou pas.
  * Champs fixes : Nouvelle page de champs fixes.
  * Types et champs libres : Nouvelle page de type et champs libres.&#x20;
* WEB - Production | Liste des OF :&#x20;
  * Nouvelle page de liste des demandes de production exportable et filtrable.
* WEB - Production | Planning :
  * Nouvelle page planning des demandes de production avec drag and drop si droit activé, modification du statut et ouverture de la carte pour visualisation des autres champs.
* WEB | Production | Détails :&#x20;
  * Nouvelle page de détail des demandes de production avec historisation de l'ensemble des modifications faites sur la demande.&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-02-21 104515.png" alt=""><figcaption><p>Page Production | Planning</p></figcaption></figure>

### &#x20;Gestionnaire d'emplacement

      _Ce projet est utilisé pour notifier via mail un utilisateur étant identifié comme responsable d'emplacement à chaque dépose d'une unité logistique sur son emplacement._&#x20;

* WEB - Référentiel | Emplacement :&#x20;
  * Ajout d'un champ sélection d'utilisateur pour responsable d'emplacement et case à cocher pour activation de l'envoi d'email pour chaque dépose.&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-02-21 104740.png" alt=""><figcaption></figcaption></figure>

### &#x20;Nomade : Emplacement sur préparation d'article

      _Ce projet est utilisé pour identifier un emplacement potentiel d'article sur un ordre de préparation en fonction de la gestion de stock de la référence associé (FIFO ou FEFO)._

* NOMADE - Stock | Préparation&#x20;
  * Ajout d'un champs emplacement rempli par l'emplacement de l'article FIFO ou FEFO lié à la référence. L'opérateur ne sera pas obligé de scanner cet article, l'emplacement permet uniquement de le diriger dans l'entrepôt.&#x20;

### Evolution du composant "Demandes à traiter"

      _Ce projet permet de filtrer avec plus de détails des demandes d'acheminements sur le composant dashboard "Demandes à traiter". Vous pouvez donc filtrer les demandes par urgence mais aussi par emplacement de prise et emplacement de dépose de vos acheminements. Au clic sur le composant, si vous avez activer le paramétrage, vous serez redirigé vers la liste des demandes d'acheminements filtrée._&#x20;

* WEB - Paramétrage | Dashboard
