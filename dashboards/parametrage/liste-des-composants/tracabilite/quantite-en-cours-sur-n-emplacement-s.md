# Quantité en cours sur n emplacement(s)

Ce composant permet de savoir le nombre total d'unités logistiques présent sur les emplacements sélectionnés.&#x20;

Sur ce composant, il faut obligatoirement renseigner le champ **Choix des emplacements** qui permet de sélectionner les emplacements sur lesquels on vient compter les unités logistiques présentes.

D'autres paramétrages sont disponibles :&#x20;

* **Afficher le délai de traitement (Les emplacement choisis doivent avoir un délai de paramétré)** : cochez ce paramétrage afin de voir le temps restant avant que vous soyez en retard dans votre traitement des UL déposés sur les emplacements paramétrés. Lorsqu'un colis est déposé sur un emplacement, un compteur correspondant au délai placé sur cet emplacement commence à tourner. Le temps affiché sur le composant correspond à ce compteur et donc au temps restant avant que le colis le plus ancien dépasse le délai de l'emplacement. Si plusieurs emplacements sont paramétrés sur le composant, c'est le temps restant le plus court qui est affiché. Si ce temps est dépassé, "A traiter sous :" se transforme en "En retard de :" et le temps correspond au temps de dépassement, avec le texte en rouge.&#x20;
* **Afficher le nom des emplacements sous le titre** : en cochant ce paramétrage, vous afficherez le nom des emplacements choisis pour ce composant sous le titre. S'il y a beaucoup d'emplacements paramétrés, les noms défileront. Ce paramétrage est pertinent à activer si vous avez plusieurs emplacements paramétrés sur un composant.
* **Rediriger au clic vers la page Encours** : si vous cochez ce paramétrage, en cliquant sur le composant, la page _Traçabilité | Encours_ s'ouvrira, filtrée sur les emplacements paramétrés sur le composant (ceux qui ont des délais paramétrés)
* **Afficher en urgence** : cochez ce paramétrage pour ajouter des logos Warning autour du titre du composant et pour passer le nombre d'UL en rouge. Les logos et le texte en rouge seront effectifs dès que la quantité dépasse 0. Les paramétrages de taille et couleurs de texte ainsi que de logo autours du titre ne sont pas pris en compte dès que la quantité dépasse 0. Ceux de **Afficher en urgence** prennent le dessus
* **Logo titre** : sous **Couleur fond composan**t, ce paramétrage est disponible seulement sur ce composant est permet d'ajouter un logo (2 fois le même) de chaque côté du titre

{% embed url="https://www.screencast.com/t/zqmVqAJkT" %}
Paramétrage composant
{% endembed %}

