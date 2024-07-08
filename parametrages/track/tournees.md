---
description: >-
  Cette page de paramétrage va avoir un impact sur l'ensemble du processus d'une
  tourné du l'heure de départ des livres jusqu'au motif de fin d'une livraison
  ou collecte.
---

# Tournées

### Calcul kilométrage et durée

Vous pouvez renseigner différentes adresses (ou la même) sur les 3 points. Cela peut être intéressant pour votre facturation.&#x20;

* **Point de départ km** : le point à partir duquel le calcule kilométrique de la tourné va commencer&#x20;
* **Point de départ calcul des horaires** : le point à partir duquel le calcule du temps passé sur la tournée va commencer&#x20;
* **Point d'arrivée** : Le dernier point de la livraison

**Heure(s) de départ** : correspond à l'heure de départ des livreurs pour débuter la tournée, cela donnera alors une estimation de passage chez les clients lors de la création de la tournée.&#x20;

Dans le tableau, vous renseignez **l'heure** (HH:MM) et le(s) **livreur(s)** associé(s). Pour ajouter une ligne cliquée sur le <mark style="background-color:blue;">**+**</mark>. Pour modifier une valeur cliquée dans le tableau.

{% embed url="https://www.screencast.com/t/ciNudUVteT" %}
Ajout d'une heure de départ
{% endembed %}

**Temps de passage moyen (minutes)** : indiquez le temps que passera votre livreur pour déposer ou récupérer des colis, pour les livraisons, les collectes et les livraisons/collectes.

### Colis écartés

**Motifs d'écartement** : lors du chargement des colis dans le camion un livreur peut écarter des colis, c'est à dire qu'il ne va pas prendre certains colis. Il devra indiquer la raison, c'est dans ce paramétrage que vous indiquez les différents choix qu'il peut avoir. _Par exemple : Colis non conforme, colis abîmé, colis absent._

### Collectes / Livraisons

* **Motifs de non livraison** : indiquez les motifs que pourra choisir le livreur s'il n'a pas pu effectuer la livraison, la liste sera la même pour les livraisons/collectes. La livraison passera alors au statut Non livrée.&#x20;
* **Motifs de non collecte** : indiquez les motifs que pourra choisir le livreur s'il n'a pas pu effectuer la collecte, la liste sera la même pour les livraisons/collectes. La collecte repassera au statut patient à contacter pour que ce transport soit à nouveau placé sur une tournée.&#x20;
* **Fin du workflow collecte pour les motifs** : indiquez les motifs que pourra choisir le livreur s'il n'a pas pu effectuer la collecte, la liste sera la même pour les livraisons/collectes. La collecte passera au statut Non collecté.

### Conditions de fin de tournée

* **Emplacements de fin de tournée** : Pour valider la fin d'une tournée, le livreur doit flasher un (ou des) emplacement que vouas avez paramétré. (Emplacements issus du référentiel)
* **Natures de colis obligatoires à déposer** : au cours de sa tournée, un livreur peut avoir des colis qu'il n'a pas pu livrer, vous pouvez décider quelle nature de colis il doit obligatoirement déposer à son retour. S'il ne les dépose pas, il ne pourra pas finir la tournée. (Nature issus du référentiel)

### Dépose des objets collectés

**Emplacements de dépose des objets collectés** : Pour les colis collectés, vous pouvez paramétrer un (ou des) emplacement sur lequel le livreur va déposer les colis collectés à la fin de sa tournée. (Emplacements issus du référentiel)

### Dépose des colis non livrés

Emplacements de retour des colis non livrés :  Pour les colis non livrés, vous pouvez paramétrer un (ou des) emplacement sur lequel le livreur va déposer ces colis à la fin de sa tournée. (Emplacements issus du référentiel)
