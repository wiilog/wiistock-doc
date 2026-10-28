---
description: Créer des articles dans Follow GT directement depuis votre ERP.
---

# API de création d'articles

Disponible depuis la mise en production du 28/10/2026.

Lorsque les réceptions sont saisies dans votre ERP, les opérateurs créent souvent les mêmes articles une seconde fois dans Follow GT. L'API de création d'articles permet à votre ERP de créer les articles automatiquement et supprime cette double saisie.

### Fonctionnement

1. Une **clé API**, valable **1 an**, est générée pour votre instance.
2. Avec cette clé, votre ERP obtient un **jeton**, valable **1 jour**.
3. Avec ce jeton, votre ERP crée les articles dans Follow GT.

Les articles dépendent des référentiels. Si un **projet**, un **emplacement**, une **référence** ou un **fournisseur** n'existe pas encore, l'API peut le créer, à condition que tous les champs obligatoires à sa création soient renseignés.

### Mise en place

La mise en place nécessite la participation de l'équipe qui gère votre ERP, car le bon fonctionnement dépend des données qu'il envoie. Contactez Wiilog pour organiser une réunion de lancement.
