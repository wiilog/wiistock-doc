# Fiabilité par référence

Ce composant présente la valeur du calcul suivant :&#x20;

Nombre de mouvements de correction d'inventaire / nombre d'articles de références ou articles du stock

Avec :&#x20;

* _**nombre de mouvements de correction d'inventaire**_ : lorsque vous faites un inventaire, si vous renseignez une quantité différente de celle en stock, il vous faut ensuite venir confirmer cette quantité dans la partie Anomalie des inventaires. Si la quantité confirmée est toujours différente de la quantité un stock, un mouvement d'entrée ou de sortie de stock d'inventaire est créé pour venir corriger la quantité en stock. Ce sont ces types de mouvements de stock qui sont comptés dans le calcul (tous les mouvements _entrée inventaire_ et _sortie inventaire_)
* _**nombre d'articles de référence ou articles du stock**_ : on vient ici compter le nombre de références actives gérées par références + le nombre d'articles (c'est à dire les articles d'une références en gestion quantité article) actifs

{% embed url="https://www.screencast.com/t/yUkDPDna9" %}
