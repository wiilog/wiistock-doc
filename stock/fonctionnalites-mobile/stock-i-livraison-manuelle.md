# Stock I Livraison manuelle

La livraison manuelle est la fonctionnalité disponible seulement sur nomade, elle permet de faire rapidement une sortie de stock via le system de livraison.&#x20;

Elle diffère de la création de demande de livraison sur le nomade ou web (Demande ⎮ Livraison), car à la validation, il n'y a pas de traitement à faire, un ordre de livraison est créer et déjà traité.

{% hint style="info" %}
Vous ne pouvez utiliser cette fonctionnalité que sur les articles et les unités logistiques. Les références ne peuvent pas être scannées.
{% endhint %}

## Création livraison manuelle

Renseigner les informations de votre livraison (selon le paramétrage des champs fixes vous pouvez afficher ou non Date attendue et Projet) :&#x20;

* **Type\*** : Indication du type de livraison
* **Commentaire** : commentaire de la livraison
* **Date attendue** : Date souhaitée de livraison
* **Projet** : Indication du projet de la livraison issu du référentiel projet

Puis scanner les articles ou unités logistiques que vous souhaiter ajouter à votre livraison. Scanner ou prendre en photo via ![](<../../.gitbook/assets/Capture d’écran 2023-04-18 à 14.37.51.png>) le code barre de l'article ou de l'UL.&#x20;

Sur la vignette, vous pouvez notamment voir son emplacement de stockage et la quantité de l'article. Si vous vous êtes trompé, appuyez sur la poubelle pour annuler le scan.

Quand vous avez fini d'ajouter vos articles ou UL, <mark style="background-color:blue;">**Valider**</mark>. Vous devez ensuite choisir l'emplacement de livraison. C'est sur cet emplacement que se fera la sortie de stock. <mark style="background-color:blue;">**Valider**</mark> pour confirmer.

Suite à cette livraison manuelle, un ordre de livraison est créé au statut "traité" contenant les articles flashés. La livraison a aussi créer des mouvements de sortie de stock des articles.
