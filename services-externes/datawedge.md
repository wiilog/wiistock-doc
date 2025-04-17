---
description: >-
  DataWedge de Zebra permet de capturer des données à partir de codes-barres et
  de QR codes, puis de les convertir en un format utilisable par Follow-GT.
---

# Datawedge

DataWedge utilise des profils pour établir une connexion entre les applications et les données capturées par le lecteur de codes-barres. Lors de l'installation initiale de Follow GT sur votre terminal Zebra ([https://wiilog.gitbook.io/wiilog-tracabilite-et-stock-pour-lindustrie/services-externes/stagenow](https://wiilog.gitbook.io/wiilog-tracabilite-et-stock-pour-lindustrie/services-externes/stagenow)),  un profil WIISTOCK a été créé dans l'application DataWedge pour assurer cette liaison entre le lecteur de codes-barres et l'application.

Si vous souhaitez modifier le comportement de saisie des données, vous devrez modifier ce profil. Par exemple, si vous souhaitez ajouter une tabulation après chaque saisie pour que l'application passe automatiquement au champ suivant du formulaire, vous pouvez ajouter ce paramètre de deux manières différentes.

## Méthode 1 :

1 : Sur votre appareil, lancez  DataWedge.\
&#x20;\
&#x20;         <img src="../.gitbook/assets/Capture d&#x27;écran 2024-06-04 141654.png" alt="" data-size="original">

2 : Dans DataWedge Profiles, sélectionnez **WIISTOCK**.

&#x20;        ![](<../.gitbook/assets/Capture d'écran 2024-06-04 142025 (1).png>)

3. Faites défiler jusqu'à "**Sortie de touches**" et cocher l'option Activé.![](<../.gitbook/assets/Capture d'écran 2024-06-04 142756.png>)
4. Séléctionnez "**Formatage des données de base**"                            ![](<../.gitbook/assets/Capture d'écran 2024-06-04 143124 (4).png>)
5. Activez l'option "**Envoyer la touche TAB**"                                                                                                               ![](<../.gitbook/assets/Capture d'écran 2024-06-04 143741 (1).png>)          &#x20;





Méthode 2 :\



Utiliser StageNow : \


1. Supprimez le profil WIISTOCK déjà présent dans DataWedge en suivant les étapes suivantes :
   1. Ouvrez DataWedge.
   2. Appuyez longuement sur le profil WIISTOCK.
   3. Sélectionnez "Supprimer le profil".
   4. Scannez le QR code suivant en utilisant Stagenow : &#x20;

&#x20;                          ![](<../.gitbook/assets/image (148).png>)

5. Le profil WIISTOCKtab a été ajouté dans Datawedge.
