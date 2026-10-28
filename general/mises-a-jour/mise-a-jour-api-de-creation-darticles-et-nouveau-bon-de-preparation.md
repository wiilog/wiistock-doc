---
description: Mise en production du 28/10/2026
---

# Mise à jour - API de création d'articles et nouveau bon de préparation

## API - Création d'articles

**Problématique** : _La création d'articles sur Follow se fait souvent en doublon d'une réception de l'ERP client. Pour limiter la double saisie des opérateurs, une API a été mise à disposition pour permettre à l'ERP client de générer les articles dans Follow depuis la réception client._

**Fonctionnement** : Il est possible de générer une clé API valable 1 an qui autorise la génération d'un token valable 1 jour pour créer des articles. Les articles dépendant des référentiels, il est également possible de créer les référentiels manquants (projet, emplacement, référence, fournisseur) tant que l'ensemble des champs obligatoires à la création de ses informations sont remplis.&#x20;

Si vous souhaitez utiliser cette API, contactez Wiilog pour organiser une réunion de lancement avec l'équipe qui gère votre ERP : le bon fonctionnement dépend des données que votre ERP envoie à l'API.



## Stock - Bon de préparation

**Problématique** : _Face à un volume important de demandes de livraison, de nombreuses préparations pouvent être entreposées dans un même espace, avec parfois des références produits identiques. Cette organisation augmente le risque d’erreurs lors de la livraison, notamment lorsque la préparation des commandes et leur expédition sont réalisées par des personnes différentes._

_**Réponse au besoin** :_ Un bon de préparation qui rappeplle le contenu de la préparation, les articles, et la livraison associée.&#x20;

**Fonctionnement** **pour répondre au besoin** : Il est possible de générer un bon de préparation à partir d’un ordre de préparation. Ce document permet de disposer d’un support facilitant l’identification des produits à préparer et le contrôle des commandes avant leur livraison.

Le bon de préparation est entièrement paramétrable selon le type de demande de livraison, depuis le menu Paramétrage | Modèles de documents | Livraison | Bon de préparation. Il est possible d’y intégrer des champs fixes ainsi que des champs libres afin d’adapter le contenu du document aux besoins opérationnels et de faciliter la transmission des informations entre les équipes chargées de la préparation et de la livraison.

<figure><img src="../../.gitbook/assets/image (200).png" alt=""><figcaption></figcaption></figure>
