---
description: >-
  Description du cas d'utilisation des fonctionnalités Follow dédiées au client
  A.
---

# Cas d'usage "Surveillance des délais de livraison"

## Contexte client&#x20;

L'équipe du site client à remonter le besoin de suivre précisément sur Follow les temps des colis de leur arrivée au quai jusqu'à leur livraison finale. Le projet portait les contraintes suivantes :&#x20;

* plusieurs flux aux fonctionnements variés pour un même colis.
* pas de continuité dans les identifiants scannés pour un même objet (parfois des UL, parfois des OT).

## 1. Paramétrages & fonctionnement référentiels

Pour faire fonctionner le projet de délai de traitement sur les unités logistiques, les référentiels à paramétrés sont : les Natures et les Emplacements.&#x20;

### Référentiel Emplacement

De nouveaux paramétrages sur le référentiel emplacement ont étés ajoutés : l'encart "Typologie d'emplacement".&#x20;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Emplacement de prise initiale : Permettra d'afficher un délai de traitement sur l'UL prise à cet emplacement à la condition que celui-ci ait une nature avec un délai de traitement renseigné. Le délai prendra en compte le temps passé de l'UL sur cet emplacement, sauf si l'emplacement est également un emplacement de pause.&#x20;

Emplacement de pause : Permettra de mettre en pause le délai de traitement sur l'UL déposée à cet emplacement. Le délai reprendra à la prise sur cet emplacement. Une unité logistique en pause n'affichera pas la donnée "Date max de traitement".&#x20;

Emplacement de dépose finale : Permettra de faire disparaitre le délai de traitement et la date max de traitement de l'UL lors de la dépose de celle-ci sur l'emplacement.&#x20;

Activer le changement de nature à la prise : Ce paramétrage changera la nature de toute unité logistique prise sur cet emplacement avec la nature renseignée en dessous. Attention, si vous laissez l'encart "Nouvelle nature à la prise sur emplacement" alors l'unité logistique perdra sa nature.&#x20;

Activer le changement de nature à la dépose : Ce paramétrage changera la nature de toute unité logistique déposé sur cet emplacement avec la nature renseignée en dessous. Attention, si vous laissez l'encart "Nouvelle nature à la dépose sur emplacement" alors l'unité logistique perdra sa nature.&#x20;
{% endhint %}

### Référentiel Nature

De nouveaux paramétrages sur le référentiel nature ont étés ajoutés : l'encart "Délai de traitement" et "Segments horaires".&#x20;

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Délai de traitement de la nature : Ce champs doit être rempli en heures et minutes "00h00" et permet de positionner un temps de traitement théorique en fonction de la nature de l'unité logistique.&#x20;

Délai de traitement de la nature dépassé : Ce paramétrage permet de sélectionné une couleur qui sera positionné sur le délai de traitement lorsque celui-ci aura dépassé le délai de traitement.&#x20;

Les segments horaires : Via le bouton +, vous pouvez paramétrer les couleurs que prendront les délais de traitement en fonction du segment horaire dans lequel ils se trouveront.&#x20;
{% endhint %}

### Paramétrage des mouvements de traçabilité

Nous avons ajouté des cases à cocher dans le paramétrage des mouvements afin de permettre aux anciens clients de ne pas être impactés par les nouvelles fonctionnalités développées.&#x20;

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Afficher le champ "Début de délai manuel" : Une fois coché, ce paramétrage permet de positionner un T0 sur une unité logistique (T0 = date et heure de début du flux) sur les mouvements de traçabilité web et nomade. Un opérateur peut donc cliquer sur une unité logistique en prise et lui associer une date et heure de début de délai.&#x20;

Dépose des groupes automatiquement sur l'emplacement ... : Ce paramétrage permet, lorsqu'une UL avec délai de traitement est mise dans un nouveau groupe, de déposer le groupe sur l'emplacement de cette unité logistique et de lui associé sa nature.&#x20;

Exemple :&#x20;

J'ai une unité logistique avec délai de traitement. Je créer un nouveau groupe "Groupe A", a la validation, mon groupe aura la nature de l'unité logistique et sera déposé sur l'emplacement de l'unité logistique.&#x20;

Remontée des délais de traitement des unités logistiques sur leur groupe : Ce paramétrage permet, lorsqu'une UL avec délai de traitement est mise dans un groupe, de positionner la nature et le délai de l'unité logistique dont le délai est le plus court sur le groupe.&#x20;

Exemple :&#x20;

J'ai 2 unités logistiques avec deux délais de traitement différents. Je les groupes dans un groupe A, alors mon groupe aura la nature et le délai de l'unité logistique avec le délai restant le plus court.&#x20;
{% endhint %}

## 2. Flux entrant via l'arrivage camion

Pour obtenir le T0 du flux entrant depuis des arrivées de camions, nous avons modifié les paramétrages de la fonctionnalité **Arrivage camion** afin de rendre le numéro de tracking non obligatoire au scan puis ajouter des liens entre la création d'arrivage camion et d'arrivage UL pour améliorer l'expérience utilisateur.&#x20;

Il est donc possible d'ajouter des arrivages camions sans numéro de tracking : ces arrivages camions peuvent être suivi par le composant "Suivi des transporteur" qui, si paramétré, permet de compter les arrivages camions non associés à des arrivages UL en fonction du nombre de numéro de tracking ou d'un arrivage camion sans numéro de tracking (compte pour 1 tant que non associé).&#x20;

<div data-full-width="true"><figure><img src="../.gitbook/assets/Capture d’écran 2024-09-13 100358.png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Capture d’écran 2024-09-13 100505.png" alt=""><figcaption></figcaption></figure></div>

La date et heure de l'arrivage camion correspond au T0 des flux entrants.&#x20;

L'opérateur va ensuite créer des arrivages UL depuis sont arrivage camion et déterminer le nombre d'unités logistiques en fonction des flux.&#x20;

* Ce sont les natures qui vont jouer le rôle de flux et qui porteront le délai de traitement qui sera suivi par les opérateurs. Ce délai se déclenche automatiquement à l'arrivage UL lorsque les unités logistiques générées sont avec des natures qui ont des délais de traitement et que l'arrivage ul est lié à un arrivage camion.&#x20;

Exemple :&#x20;

{% hint style="info" %}
Je créer un arrivage camion le 25/07/2025 à 9h00, puis un opérateur créé un arrivage UL depuis cet arrivage camion à 10h00 le même jour. Il créé 3 UL, 2 avec la nature Urgent 2h et 1 avec la nature Standard 7h. Alors à 10h30 le même jour :&#x20;

* Les 2 UL urgentes auront un délai restant de : 30 minutes avec une date maximale de traitement au 25/07/2025 11h.&#x20;
* L'UL standard 24h aura un délai restant de 22h30 avec une date maximale de traitement au 28/07/2025 9h00.&#x20;
{% endhint %}

Attention, les dates maximales de traitement et les délais restant prennent en compte les jours ouvrés et heures de travaille renseignés dans les paramétrages généraux Follow.&#x20;



Les opérateurs pourront ensuite faire des prises et déposes jusqu'à des emplacements de "Début", "Fin" ou de "Mise en pause" des flux.&#x20;

## 2. Flux entrant via mouvement de traçabilité & T0 fixé

## Le suivi des mouvements de traçabilité et groupage

Pour assurer la traçabilité des unités logistique de A à Z, nous avons utilisé la fonctionnalité Groupage. Les unités logistiques peuvent donc être associées depuis un TC ou un PC à d'autres numéros de suivi. Les groupages vont permettre de regrouper les prises et déposes d'unités logistiques et donc de faciliter la traçabilité. Une unité logistique portant un délai de traitement (chrono)&#x20;

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
