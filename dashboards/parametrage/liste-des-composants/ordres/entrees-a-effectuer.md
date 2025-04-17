# Entrées à effectuer

Ce composant est fait de 3 cellules différentes :&#x20;

* Une cellule qui présente un graphique avec des segments horaires et un nombre d'unités logistiques par nature sur chaque segment horaire. Les unités logistiques comptées sont celles qui sont présentes sur un ensemble d'emplacements paramétrés. Ainsi, si un segment marqué 36h-48h a 25 UL, cela signifie qu'il y a 25 UL sur ces emplacements qui sont à traiter sous 36h-48h. Chaque segment représente le temps restant sur les emplacements paramétrés pour les unités logistiques présentes. Si les UL passent dans le segment retard, cela signifie qu'elles sont depuis plus de 48h sur les emplacements paramétrés (si le temps le plus élevé paramétré est de 48h)
* Une cellule indicateur _Nombre de ligne à traiter_ qui est en haut à droite qui présente le nombre total d'unités logistiques à traiter sur  l'ensemble des emplacements paramétrés
* Une cellule indicateur _Prochain emplacement_ à traiter qui est en bas à droite qui présente l'emplacement, parmi les emplacements paramétrés, sur lesquels l'unité logistique la plus urgente à traiter est présente&#x20;

Les paramétrages possibles sont :&#x20;

* **Infobulle** : pour paramétrer l'infobulle de la cellule contenant le graphique
* **Infobulle "Nombre de lignes à traiter"** : pour paramétrer l'infobulle de la cellule contenant l'indicateur _Nombre de lignes à traiter_
* **Infobulle "Prochain emplacement à traiter"** : pour paramétrer l'infobulle de la cellule contenant l'indicateur _Prochain emplacement à traiter_
* **Natures de colis\*** : champ obligatoire. Ce paramétrage permet de sélectionner quelle nature d'unité logistique afficher. Les natures sont présentés dans des histogrammes côte à côte.&#x20;
* **Emplacements\*** : champ obligatoire. Sélectionnez les emplacements sur lesquels vous souhaitez voir le nombre d'unités logistiques des natures sélectionnées présentes
* **Rediriger vers la page Encours au clic** : si vous cochez ce paramétrage, lorsque vous cliquez sur les cellules _Nombre de lignes à traiter_ ou _Prochain emplacement à traiter_, vous êtes redirigé vers la page _**Traçabilité | Encours**_, filtrée automatiquement sur les emplacements paramétrés sur le composant.&#x20;
* **Segments horaires** : venez paramétrer ici les segments qui s'affichent sur la cellule contenant le graphique. Vous pouvez paramétrer jusqu'à 5 segments. Le segment Retard sera toujours présent. Au moins un segment doit être renseigné. Par défaut, 5 segments allant jusqu'à 48h vous sont proposés. Vous pouvez en supprimer ou changer les horaires. Chaque horaire derrière "à" est modifiable

{% embed url="https://www.screencast.com/t/Bvbdxhdg" %}
