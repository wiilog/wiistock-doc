# Préparation - Planning

Les préparations via le planning changent légèrement de flux comparé aux Préparations "classique". Vos demandes de livraison pourront donc arriver sur le planning avec différentes dates attendues et sans vérification du stock disponible pour ensuite permettre de faire des lancements de commande en masse.

## **Paramétrage pour accéder et utiliser le planning**

Pour afficher la page planning, allez dans le paramétrage de votre [rôle](../../../parametrages/utilisateurs/roles/), onglet **Ordre** puis **Préparations** et activer **Afficher préparations - planning**, vous pouvez aussi activer **Modifier la date de préparation** pour afficher le bouton <mark style="background-color:blue;">**Modifier**</mark> dans le détail d'une préparation et ainsi modifier la date de préparation de votre livraison, par défaut la date de préparation sera le même jour que la date attendue.

Deux autres paramétrages sont à activer sur la demande de livraison, dans [Stock > Demande > Livraisons](../../parametrage/demandes/livraisons/) activer **Réaliser une demande de livraison sans quantité en stock (lancement de préparation)** et dans Livraisons - Champs fixes afficher **Date attendue** à la création.

## Page Préparation - Planning

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Ordres**</mark>, puis <mark style="background-color:blue;">**Planning**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* un **planning**, permettant d'afficher l'ensemble des préparations aux différents statuts

{% embed url="https://www.screencast.com/t/EQ6gzltZ" %}
Page Préparation - Planning
{% endembed %}

### Contenu des filtres

|                       |                                                                                                                                                                                                                                                        |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Numéro de demande** | Pour filtrer sur les numéros de demande de livraison ayant générés les ordres                                                                                                                                                                          |
| **Opérateurs**        | Pour filtrer sur la personne ayant traitée l'ordre de préparation. Vous pouvez renseigner plusieurs utilisateurs. opérateur ayant traité l'ordre de préparation. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application.  |
| **Type**              | Type de la demande de livraison ayant créée l'ordre de préparation                                                                                                                                                                                     |
| **Statuts**           | Statut de l'ordre de préparation. Par défaut, tous les statuts sont sélectionnés.                                                                                                                                                                      |

Liste des statuts :&#x20;

* **Validé** : Demande de livraison validée, 1er statut d'une préparation
* **Lancé** : Préparation lancée, les quantités en stock sont disponibles
* **En cours de préparation** : L'opérateur a commencé à préparer la préparation
* **Partiellement préparé** : Seulement une quantité a été préparée et envoyée en livraison. Un reliquat de préparation a été généré avec les quantités restantes. La demande de livraison est au statut partiellement préparé
* **Traité** : Toutes les quantités demandées ont été pickées. La demande de livraison est au statut préparé

### Contenu planning

* Un filtre sur **Aujourd'hui** pour revenir à la date du jour et 2 flèches pour naviguer dans les semaines
* Un bouton <mark style="background-color:blue;">**Lancer les préparations**</mark> pour passer les préparations Validé au statut Lancé
* Le planning avec 5 jours afficher contenant les **étiquettes de préparation :**
  * Le numéro de la préparation
  * Le statut
  * Le type de la livraison&#x20;
  * La date de création de la livraison
  * La date attendue de la livraison

{% hint style="info" %}
Au clique sur l'étiquette renvois vers le détail de la préparation. Il est possible de faire un glisser-déposer entre les jours pour modifier les dates de préparations, seulement pour les ordres en statut Validé.
{% endhint %}

{% embed url="https://www.screencast.com/t/QcvnFtjnfFxv" %}
Glisser-déposer d'une préparation
{% endembed %}

## Lancer les préparations

Pour lancer les préparations cliquer sur <mark style="background-color:blue;">**Lancer les préparations**</mark> une modale Lancement des préparations s'ouvrira avec les préparations qui ont leur date de préparation entre les bornes choisie et au statut Validé. Par défaut la prériode de lancement est celle afficher sur le planning soit 5 jours.

{% embed url="https://www.screencast.com/t/y8MvzEbi9" %}
Modale lancement des préparations
{% endembed %}

Dans la partie de gauche **Préparation(s) disponible(s) au lancement** vous retrouvez les préparations à lancer, à noté que la date attendue a été remplacé par la date de préparation.

Vous pouvez passer par glissé-déposé les préparations que vous voulez lancer dans **Préparation(s) à lancer** ou via le bouton <mark style="background-color:blue;">**Lancer tous**</mark> pour tout passer. vous pouvez aussi faire le mouvement inverse en cliqant sur <mark style="background-color:blue;">**Remettre tout**</mark>.

{% embed url="https://www.screencast.com/t/PMXfaGdCMa" %}

Une fois que des préparations sont dans **Préparation(s) à lancer** le bouton <mark style="background-color:blue;">**Vérifier le stock**</mark> s'active.

Lors de la vérification du stock, on interroge le stock disponible pour chaque référence. Si la quantité disponible est supérieure ou égale à la quantité demandée, vous pourrez valider le lancement. Si la quantité disponible est inférieure à la quantité demandée, vous ne pourrez pas valider le lancement.

### Quantité en stock disponible

{% embed url="https://www.screencast.com/t/SnYnZdnY6" %}
Quantié en stock suffisante
{% endembed %}

Quand la quantité est disponible le rectangle de droite à un contour vert et vous avez accès au bouton <mark style="background-color:blue;">**Valider le lancement**</mark>. Les préparations passent alors au statut **Lancé** et redescendent sur le nomade (en fonction de votre paramétrage des types de livraison). Le stock disponible de chaque référence contenues dans les préparations est décrémenté.&#x20;

### Quantité en stock indisponible

{% embed url="https://www.screencast.com/t/RREOKE2rz" %}
Quantié en stock insuffisante
{% endembed %}

Quand la quantité est indisponible le rectangle de droite à un contour rouge et la préparation passe d'orange à rouge. De plus, une section **Manque quantité sur** apparaît, elle indique en fonction des préparations sur qu'elle référence il y a un problème de quantité. Vous avez comme information la référence demandée la quantité disponible et la quantité demandée. Le bouton <mark style="background-color:blue;">**Vérifier le stock**</mark> n'a pas changé, vous devez enlever la préparation problématique pour pouvoir lancer une préparation.

