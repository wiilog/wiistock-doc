# Configurations

## Configurations

Cette section règle le comportement à la création d'un arrivage UL.

| Option                                                                          | Effet                                                                                                                                    |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Redirection vers l'arrivage UL créé**                                         | Après la création, vous êtes redirigé vers le détail de l'arrivage. Si l'option n'est pas cochée, le formulaire reste ouvert et se vide. |
| **Envoyer un email après nouvel arrivage UL**                                   | Un mail est envoyé au destinataire de l'arrivage dès sa création.                                                                        |
| **Impressions cochées par défaut**                                              | Les cases **Impression UL** et **Imprimer arrivage** (si ce champ est affiché) sont cochées par défaut à l'ouverture du formulaire.      |
| **Impression en double de l'étiquette d'UL d'arrivage si champ "Douane" coché** | Les étiquettes sont imprimées en double quand **Douane** est coché.                                                                      |
| **Utilisation des arrivages camion**                                            | Permet d'utiliser les numéros de tracking transporteur issus des arrivages camion.                                                       |

## Emplacements de dépose automatique

À la validation de l'arrivage, les UL sont déposées automatiquement sur l'un des emplacements suivants :

| Option                                                               | Utilisé quand…                           |
| -------------------------------------------------------------------- | ---------------------------------------- |
| **Emplacement de destination des arrivages UL**                      | Cas par défaut.                          |
| **Emplacement de dépose des arrivages UL si champ "douane" coché**   | **Douane** est coché.                    |
| **Emplacement de dépose des arrivages UL si urgence détectée**       | L'arrivage est détecté comme urgent.     |
| **Emplacement de dépose des arrivages UL si destinataire renseigné** | Le champ **Destinataire(s)** est rempli. |

Si plusieurs cas s'appliquent, l'ordre de priorité est le suivant :

1. Douane
2. Urgence
3. Emplacement saisi sur le formulaire (si le champ est affiché)
4. Destinataire
5. Emplacement par défaut

## Format du numéro

**Format du numéro généré pour l'arrivage UL** : choisissez le format des numéros d'arrivage, par exemple `aammjjhhmmss-xx`.
