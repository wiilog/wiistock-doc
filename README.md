# Wiilog & Follow GT : les fondamentaux



<figure><img src=".gitbook/assets/site industriel-vidéo (1).jpg" alt=""><figcaption></figcaption></figure>

Follow GT est l'application web et mobile de Wiilog pour la traçabilité, le stock, la production et les tournées. Vous n'activez que les modules dont vous avez besoin.

### Les modules

| Module         | Usage                                                                           | Fonctionnalités principales                                                                                      |
| -------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Trace**      | Localiser et suivre vos unités logistiques (colis, palettes, caisses)           | Arrivages camion et UL, prises/déposes, groupage, acheminements, services, tournées, urgences, litiges           |
| **Stock**      | Gérer le stock de la réception au bord de ligne                                 | Références et articles, réceptions, livraisons, collectes, transferts, expéditions, achats, inventaires, alertes |
| **Production** | Suivre les ordres de fabrication                                                | Demandes de production, statuts paramétrables, vue planning                                                      |
| **Track**      | Livraisons et collectes au dernier kilomètre (ex. : hospitalisation à domicile) | Demandes de transport, tournées, planning                                                                        |

Fonctions transverses : IoT, RFID, dashboards, imports/exports, [API](interfacage/api-creation-articles.md), entrepôt de données (BI).

### Vos deux instances

* **Production** (`abc1-prod.follow-gt.fr`) : l'environnement utilisé au quotidien.
* **Recette** (`abc1-rec.follow-gt.fr`) : pour tester les nouvelles versions avant leur mise en production.

### Composants

* **Application web** : navigateurs Chromium (Chrome, Edge)
* **Application nomade** : Android 8 à 14
* **Entrepôt de données** : voir [Cartographie des données](entrepot-de-donnees/cartographie-des-donnees.md)
* **Wiispool** : impressions automatisées, voir [WiiSpool V3](services-externes/wiispool-v3.md)

👉 Pour démarrer : [Premiers pas](general/premiers-pas.md)

