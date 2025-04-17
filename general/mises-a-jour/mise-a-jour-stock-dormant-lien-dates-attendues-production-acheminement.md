---
description: Mise en production du 26/03/2025
---

# Mise à jour - Stock dormant, lien dates attendues production - acheminement

## Surveillance stock dormant

Le projet à pour but de surveiller des références du stock qui ne seraient pas utilisées pendant un certain temps. Un email sera envoyé aux gestionnaires donc les références sont considérées comme dormante pour qu'ils récupèrent leur référence ou qu'ils demandent une prolongation en stock.&#x20;

### Règle d'envoi d'email&#x20;

L'administrateur devra renseigner les informations suivante sur chaque type de référence :&#x20;

* Durée de stockage maximal (j) : nombre de jours de stockage autorisé d'une référence (nombre de jours sans mouvement d'entrée ou sortie de stock)&#x20;
* Temps d'immobilisation (j) : nombre de jours de stockage d'une référence (nombre de jours sans mouvement d'entrée ou sortie de stock)&#x20;
* Fréquence d'interrogation : fréquence ou l'email doit se déclencher si le nombre de jours sans bougé de la référence est supérieur au temps d'immobilisation et/ou à la durée de stockage maximale.&#x20;

### Paramétrage

* Paramétrage | Stock | Demandes | Livraisons - Modèle de demande : Nouveau modèle de type "stock dormant" pour créer des demandes de livraisons sans références précise avec une icone.&#x20;

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

* Paramétrage | Stock | Articles | Alerte stock dormant :&#x20;
  * Possibilité dans ce paramétrage d'ajouter des boutons d'actions depuis la liste de modèles créés à l'étape d'avant.&#x20;
  * Possibilité de choisir par type de référence, une fréquence d'interrogation des gestionnaires.

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2025-04-17 134424.png" alt=""><figcaption></figcaption></figure>

### Email et page de gestion des références dormantes

En tant que gestionnaire de référence, si je reçois un email me demandant de gérer mon stock, je dois cliquer sur le bouton "Cliquez ici pour faire vos choix" et je serais rediriger sans connexion vers la page de gestion des références.&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2025-04-17 135439.png" alt=""><figcaption><p>Style de l'email envoyé aux gestionnaires</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2025-04-17 135519.png" alt=""><figcaption><p>Page de gestion des articles</p></figcaption></figure>

## Evolution lien date attendue production - acheminement

L'évolution à pour objectif de faciliter le remplissage d'une demande d'acheminement depuis une demande de production en préremplissant les dates d'échéances de la demande d'acheminement avec la date attendue de la demande de production.



## Evolution de l'ordre des paramétrages pour mise en cohérence - Projet interne

Objectif : Rationnaliser le fonctionnement des paramétrages dans l'ordre des pages à paramétré pour une installation d'instance.&#x20;

1. Types et champs libres
2. Statuts
3. Champs fixes
4. Configuration&#x20;
