# Cas d'usage "Tournée automatisée"

## Objectif

Ce cas d'usage va permettre de paramétrer la fonctionnalité des tournées de sorte à ce que l'opérateur puisse décider des emplacements de sa tournée, en fonction des UL récupérées. Il va pouvoir ajouter des emplacements au fur et à mesure, et toutes les informations (PJ, signature, commentaire). de chaque mouvements/UL seront centralisées dans sa tournée.

### Avantage

Cela permet à l'opérateur d'optimiser sa tournée et de ne pas être bloqué par un seul chemin. Ce paramétrage permet également de servir comme "demande d'acheminement" pour certaines UL.

## Paramétrage étiquettes

Il est important que les étiquettes des UL soient bien paramétrées pour faire apparaître leur emplacement de destination finale. L'opérateur aura alors l'information pour pouvoir les amener.&#x20;

Dans Paramétrage > Trace > Arrivage UL > Étiquettes, il faut cocher la ligne "Afficher l'emplacement de dropzone".&#x20;

L'emplacement de dropzone est associé au destinataire. Il est paramétrable depuis l'utilisateur > dropzone.&#x20;

Cet emplacement servira de destination finale à l'UL. C'est à dire qu'à réception d'UL, cette dernière sera posée sur un emplacment ype : arrivage. Et sa destination correspond  au destinataire, donc sa dropzone.&#x20;

Au formulaire de création d'arrivage UL, il est nécessaire d'y indiquer le destinataire pour faire apparaitre sa dropzone sur l'étiquette.&#x20;

<figure><img src="../.gitbook/assets/Capture d’écran 2026-01-07 à 16.12.46.png" alt=""><figcaption></figcaption></figure>

## Paramétrage Tournée

1. Dans paramétrage > Trace > Tournées, il faut créer un type qui sera associé à ce type de tournée. Il faut, dans le paramétrage de ce type, y indiquer un seul emplacement où les UL seront à récupérer par l'opérateur. La tournée pour ce type contient donc un seul empalcement.
2. Le reste du paramétrage est ensuite à compléter en fonction des informations que vous souhaitez voir apparaître.

On retrouve donc les détails de notre tournée avec l'emplacement de récupération d'UL défini.

<figure><img src="../.gitbook/assets/Capture d’écran 2026-01-07 à 15.27.31.png" alt=""><figcaption></figcaption></figure>

### Démarrer la tournée et ajouter de nouveaux emplacements

Lors de la création de tournée, il faut selectioner le type de tournée qui ne possède qu'un seul emplacement. Ici --> Tournée récurrente

On arrive donc sur la page des détails de la tournée avec un seul emplacement, celui où se trouve les UL de l'arrivage.

L'opérateur va démarrer sa tournée puis&#x20;
