---
description: >-
  Description du cas d'utilisation des fonctionnalités Follow dédiées au client
  A.
---

# Cas d'usage "Surveillance des délais de livraison"

## 0. Contexte client&#x20;

L'équipe du site client à remonter le besoin de suivre précisément sur Follow les temps des colis de leur arrivée au quai jusqu'à leur livraison finale. Le projet portait les contraintes suivantes :&#x20;

* plusieurs flux aux fonctionnements variés.
* pas de continuité dans les identifiants scannés pour un même objet (parfois des UL, parfois des OT).

## 1. L'arrivage camion - arrivage UL

Pour obtenir le T0 du flux entrant depuis des arrivées de camions, nous avons modifié les paramétrages de la fonctionnalité **Arrivage camion** afin de rendre le numéro de tracking non obligatoire au scan puis ajouter des liens entre la création d'arrivage camion et d'arrivage UL pour améliorer l'expérience utilisateur.&#x20;



<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2024-09-18 151915.png" alt=""><figcaption></figcaption></figure>

<div data-full-width="true"><figure><img src="../.gitbook/assets/Capture d’écran 2024-09-13 100358.png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Capture d’écran 2024-09-13 100505.png" alt=""><figcaption></figcaption></figure></div>



## 2. Le suivi des mouvements de traçabilité et groupage

Pour assurer la traçabilité des unités logistique de A à Z, nous avons utilisé la fonctionnalité Groupage. Les unités logistiques peuvent donc être associées depuis un TC ou un PC à d'autres numéros de suivi comme les OT. Les groupages vont permettre de regrouper les prises et déposes d'unités logistiques et donc de faciliter la traçabilité.

{% hint style="info" %}
La différence entre groupage et association : Une association permet d'identifier une ou plusieurs unités logistiques sous un autre identifiant si l'étiquette d'UL n'est plus la donnée à suivre. L'association n'a pas de fin, l'unité logistique pourra toujours être déplacée avec son association. Le groupage, peut être dégroupé, et est donc supposé temporaire.&#x20;
{% endhint %}

L'identifiant utilisé lors du groupage peut être recherché depuis la barre des filtres des unités logistiques.&#x20;

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2025-01-17 122341.png" alt=""><figcaption></figcaption></figure>

Enfin, pour faciliter le management visuel et la recherche dans la vie d'une unité logistique, nous avons ajouter un historique de traçabilité sur chaque UL. Vous pouvez donc voir l'ensemble des mouvements de l'unité logistique de son arrivée du camion jusqu'à sa livraison finale.&#x20;

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2024-09-13 105055.png" alt=""><figcaption></figcaption></figure>

## 3. Les divisions d'UL par groupage

Une UL peut être divisée en deux UL : une UL parente et une UL enfant (.1).&#x20;

Pour diviser deux UL, il faut :&#x20;

* Qu'une ULA soit inclue dans un groupe A
* Que l'ULA soit scannée dans un groupe B, et valider la division.&#x20;

Ainsi, deux UL seront obtenues : Une ULA dans le groupe A et une ULA.1 dans le groupe B.&#x20;

L'ULA.1 portera l'historique de traçabilité de l'UL parent.

## 4. Les délais de livraison&#x20;

Des règles ont étés mises en place pour suivre les délais de livraison des unités logistiques en fonction des paramètres suivants :&#x20;

* Les heures et jours travaillés
* Les jours fériés
* Les délais de livraison sur le référentiel Nature
* Les start, stop et pause de mesure des temps sur le référentiel Emplacement.&#x20;

En fonction du point d'entrée de l'unité logistique, le T0 variera :&#x20;

* Si l'UL est dans son premier décompte et proviens d'un arrivage camion, alors son T0 sera la date et heure de création de l'arrivage camion auquel elle est reliée.&#x20;
* Si l'UL est dans son premier décompte et n'est pas reliée à un arrivage camion, alors son T0 sera la date de son dernier mouvement.&#x20;

### Les délais de livraison depuis un arrivage camion

Prenons le cas des paramétrages suivants :&#x20;

* Liste des emplacements et paramétrages :&#x20;
  * "Arrivage" : Emplacement sans paramétrage spécifique.
  * "Gare A": Emplacement de dépose "pause".
  * "Gare B": Emplacement de "dépose finale" et de "prise initiale".
  * "Gare C" : Emplacement de "prise initiale" et "dépose pause".&#x20;
  * "Gare D" : Emplacement de "dépose finale".&#x20;
  * "Gare E" : Emplacement de changement de nature à la dépose "Flux 4h"
  * "Gare F" : Emplacement de changement de nature à la prise "Urgent 0h30".&#x20;
  * "Gare G" : Emplacement de changement de nature à la dépose : "Flux 3h"&#x20;

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2024-09-18 141144.png" alt=""><figcaption></figcaption></figure>



### Les délais de livraison sans arrivage camion

Une UL peut être inconnue du système, sa création se fera alors via un mouvement de prise sur un emplacement.&#x20;

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2024-09-18 141256.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Capture d&#x27;écran 2024-09-18 151120.png" alt=""><figcaption></figcaption></figure>
