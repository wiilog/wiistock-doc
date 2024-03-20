# Nombre d'acheminements quotidiens

Ce composant permet d'avoir un suivi sur les demandes d'acheminement selon leur statut et la date de référence sélectionnée.&#x20;

{% hint style="info" %}
Attention, vous devez avoir des dates d'échéances sur vos acheminements pour qu'ils soient comptabilisés sur le graphique.
{% endhint %}

Les paramétrages disponibles sont :&#x20;

* **Type(s) d'acheminements\*** : champ obligatoire. Sélectionnez les types d'acheminements que vous souhaitez afficher sur le graphique. Si vous souhaitez afficher tous les acheminements, cliquez sur le bouton <mark style="background-color:blue;">**Tous les types**</mark> pour sélectionner tous les types d'acheminements paramétrés.
* **Distinguer les acheminements par type** : cochez ce switch pour avoir un barre par jour et par type d'acheminement au lieu que tous les acheminements soient rassemblés dans une seule barre si vous avez sélectionné plusieurs types
* **Statut(s)\*** : champ obligatoire. Sélectionnez les statuts des types sélectionnés pour voir seulement les acheminements qui sont à ce(s) statut(s). Si vous voulez voir tous les acheminements à tous les statuts, cliquez sur <mark style="background-color:blue;">**Tous les statuts**</mark>
* **Voir sur les \[1] \[2]** : champ obligatoire. Pour choisir sur quelle période vous souhaitez avoir le suivi des acheminements.
  * **\[1]** : pour le premier champ, vous pouvez choisir sur combien de jours vous souhaitez suivre les acheminements. Vous pouvez aller jusqu'à 7 jours glissants
  * **\[2]** : sur ce deuxième champ, vous venez choisir entre "derniers jours" et "prochains jours"
    * _**derniers jours**_ : pour avoir le suivi de ce qu'il s'est passé sur les x derniers jours
    * _**prochains jours**_ : pour avoir la visibilité de ce qu'il va se passer sur les x prochains jours
* **Date de référence\*** : champ obligatoire. Ce champs permet de savoir sur quelle date se baser pour comptabiliser les acheminements&#x20;
  * **Date d'échéance "Du"** : on regardera la première date d'échéance positionnée sur les acheminements pour compter combien d'acheminement aux statuts et types sélectionnés il y a sur chaque journée présentée sur le graphique. Ainsi, on peut visualiser la charge à venir pour les demandes d'acheminement
  * **Date d'échéance "Au"** : on regardera la deuxième date d'échéance positionnée sur les acheminements pour compter combien d'acheminement aux statuts et types sélectionnés il y a sur chaque journée présentée sur le graphique. Ainsi, on peut visualiser la charge à venir pour les demandes d'acheminement
  * **Date de validation** : on regardera à quelle date a été validée les acheminements pour afficher combien d'acheminement aux statuts et types sélectionnés ont été validées sur les dates affichées sur le graphique
  * **Date de traitement** : on regardera la date de traitement des acheminements aux statuts et types sélectionnées pour afficher combien d'acheminements ont été traitées sur les dates affichées sur le graphique

{% embed url="https://www.screencast.com/t/mBXHq5daF53" %}
