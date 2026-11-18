# Export CSV

Les exports de données se trouvent en général sur les listes des demandes/ordres/mouvements ou autres entités de données.

Les 2 possibilités d'export sont pour des données liées aux références et aux articles présents dans le stock, cela inclut également les champs libres associés. Afin de lancer l'export des articles ou références, il faut cliquer sur le bouton "**Exporter au format CSV"** et ne pas quitter la page tant que l'export n'est pas terminé, car le fait de quitter ou de rafraichir la page annulera l'export. Le système de champ libre multiplie les requêtes dans la base de données, c'est pourquoi l'export total de la base peut prendre un certain temps.

Lors d'un export unique des références, il est possible de limiter les données exportées grâce à deux filtres, afin de réduire le temps de génération :

* **Bornes de dates de création** : les deux dates (minimum et maximum) doivent être renseignées ensemble, et la date minimum ne peut pas être postérieure à la date maximum ;
* **Statut** : un ou plusieurs statuts de référence.

{% hint style="info" %}
Les références et articles exportés sont seulement ceux avec le groupe de visibilité rattaché à  l’utilisateur.
{% endhint %}
