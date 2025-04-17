# Configurations

* **Vider et rester sur la modale de création de mouvement** : si ce paramétrage est coché, lorsque vous créez des mouvements via la supervision, la modale de création de mouvement restera toujours ouverte à la création d'un mouvement et se videra
*   **Afficher le détrompeur sur les mouvements de prise si UL non disponible sur l'emplacement** : si ce paramétrage est coché, lorsque vous réaliser un mouvement de prise d'une Unité Logistique, sur Web ou Nomade, vous aurez un message pour vous prévenir si l'Unité Logistique n'a pas été prise sur un emplacement sur lequel elle avait été déposée.&#x20;

    _Par exemple : Je fais mon arrivage UL sur l'emplacement RECEPTION, si je prends l'UL que je viens de déposer sur un autre emplacement que RECEPTION, alors j'aurais un message pour me prévenir que cette UL n'était pas posée sur cet emplacement._&#x20;
* **Afficher le champ "Début de délai manuel" :** si coché, vous pourrez lors de vos mouvements, modifier le T0 de vos chrono sur vos UL. Ne fonctionne que si vous utilisez des chrono sur vos flux d'UL.&#x20;
* **Utilisation RFID Prise / Dépose mobile :** si coché, vous pourrez faire des scans de tags rfid en prise et en dépose via vos nomades. Attention, vos nomades doivent être compatibles aves les technologies RFID.



**Mails de relance** :&#x20;

* **Déclencher un mail de relance si colis sur point de livraison dropzone à 7j, 15j, 30j, et 42j** :

Si&#x20;

1. Ce paramétrage est coché;
2. L'emplacement de dépose du colis est paramétré comme "Point de livraison";
3. Le colis est associé à un destinataire de l'arrivage d'unités logistiques;
4. Un colis reste un certain temps sur un point de livraison.

alors ce destinataire recevra des mails aux intervalles décrits pour venir récupérer son colis, tant que le colis sera sur cet emplacement.

* Bouton **Déclencher les mails de relance** : ce bouton sert à lancer les mails de relance en un coup sans avoir à cocher le paramétrage.

<figure><img src="../../../.gitbook/assets/Capture d&#x27;écran 2024-07-05 093805.png" alt=""><figcaption><p>Paramétrage | Trace | Mouvements | <strong>Configurations</strong></p></figcaption></figure>
