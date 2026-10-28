# Configurations

### Mouvements

| Option                                                                                        | Effet                                                                                                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Vider et rester sur la modale de création de mouvement**                                    | Sur le web, la modale de création reste ouverte et se vide après chaque mouvement.                                                                                                                                                                                      |
| **Afficher le détrompeur sur les mouvements de prise si UL non disponible sur l'emplacement** | Web et nomade : un message prévient l'opérateur s'il prend une UL sur un autre emplacement que celui où elle a été déposée. _Exemple : UL déposée sur RECEPTION puis prise sur un autre emplacement._ Pour des contrôles plus fins, voir [Détrompeurs](detrompeurs.md). |
| **Afficher le champ « Début de délai manuel »**                                               | Permet de modifier le T0 du chrono d'une UL lors d'un mouvement. Ne sert que si vous utilisez des chronos sur vos flux d'UL.                                                                                                                                            |
| **Utilisation RFID Prise / Dépose mobile**                                                    | Permet de scanner des tags RFID en prise et en dépose sur le nomade. Les terminaux doivent être compatibles RFID : contactez Wiilog.                                                                                                                                    |

### Groupage / Dégroupage

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2F4ddrovgtkYmdXz13WL8Q%2FCapture%20d%E2%80%99e%CC%81cran%202026-03-24%20a%CC%80%2009.42.25.png?alt=media&#x26;token=a97a48ae-c126-4825-ae09-b7294916acbd" alt=""><figcaption></figcaption></figure>

| Option                                                                                                  | Effet                                                                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Dépose des groupes automatiquement sur l'emplacement des UL du groupage et association de la nature** | À la création d'un groupe, si au moins une UL a un délai de traitement en cours, le groupe est déposé sur l'emplacement de l'UL au chrono le plus court (ou en retard) et prend sa nature.                                     |
| **Remontée des délais de traitement des UL sur leur groupe**                                            | Le groupe prend la nature et le délai de l'UL qui a le délai le plus court.                                                                                                                                                    |
| **Transformer un groupe en UL lorsqu'il est vide**                                                      | Dès que la dernière UL sort du groupe, le groupe devient une UL. Ce changement apparaît dans son historique de traçabilité.                                                                                                    |
| **Groupage d'un groupe autorisé**                                                                       | Un groupe peut être groupé dans un autre. _Exemple : groupe\_1 contient UL\_1 et UL\_2. Si vous groupez groupe\_1 dans groupe\_2, UL\_1 et UL\_2 passent dans groupe\_2, et groupe\_1 devient une UL contenue dans groupe\_2._ |

### Mails de relance

**Déclencher un mail de relance si colis sur point de livraison dropzone à 7 j, 15 j, 30 j et 42 j**

Quand cette option est cochée, le destinataire d'un colis reçoit un mail de relance après 7, 15, 30 puis 42 jours, tant que le colis reste sur le groupe d'emplacements de son emplacement de dépose. Aucun mail n'est envoyé après 42 jours.

Conditions :

* l'emplacement de dépose est paramétré comme **Point de livraison** ;
* le colis est associé à un destinataire dans l'arrivage d'unités logistiques.

Les groupes d'emplacements se gèrent dans **Référentiel | Emplacements | Groupes**.

Le bouton **Déclencher les mails de relance** envoie les relances immédiatement, sans cocher l'option.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FRiyLAkcW6ToWIKoW0PXN%2FCapture%20d%E2%80%99e%CC%81cran%202025-08-14%20a%CC%80%2014.54.51.png?alt=media&#x26;token=a566bff6-ae10-4a26-ba10-c9e3842c06fb" alt=""><figcaption></figcaption></figure>
