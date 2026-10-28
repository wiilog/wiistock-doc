# Détrompeurs

Chemin : **Paramétrage | Mouvements | Détrompeurs**

Un détrompeur se déclenche lorsqu'une unité logistique (UL) scannée remplit une condition. Selon le paramétrage, l'opérateur doit confirmer la prise ou est bloqué. Les détrompeurs fonctionnent sur les mouvements de traçabilité **nomade** et **web**.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FijeGIM2EVJ84NGsKhlAo%2Fimage.png?alt=media&#x26;token=e6a7475d-29dc-445c-9c81-7cd57b0f3de1" alt="Paramétrage des détrompeurs"><figcaption><p>Paramétrage des détrompeurs</p></figcaption></figure>

### Créer un détrompeur

1. Choisissez l'action : **Bloquer** ou **Faire confirmer** la prise.
2. Choisissez la condition de déclenchement :
   * le code de l'UL commence par une ou plusieurs valeurs ;
   * le code de l'UL ne commence pas par une ou plusieurs valeurs ;
   * l'UL existe ;
   * l'UL n'existe pas ;
   * l'UL est présente sur l'emplacement de prise ;
   * le code de l'UL ne contient pas entre _min_ et _max_ caractères (inclus) ;
   * l'UL a une nature autorisée ;
   * l'UL n'a pas une nature autorisée.
3. Sélectionnez les **rôles** et les **fonctionnalités** concernés.
4. Rédigez le **message** affiché à l'opérateur.

### Ce que voit l'opérateur

Sur le web comme sur le nomade, une pop-up s'affiche dès qu'un détrompeur se déclenche sur l'UL scannée.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FUeuO3R2EAo3Lm9jtfOtT%2Fimage.png?alt=media&#x26;token=2acd83bd-dd9b-422f-8e86-0c927db93b1d" alt="Pop-up de détrompeur sur le web"><figcaption><p>Pop-up de détrompeur sur un mouvement web</p></figcaption></figure>

#### Plusieurs détrompeurs déclenchés en même temps

| Combinaison                 | Affichage                                                           |
| --------------------------- | ------------------------------------------------------------------- |
| Blocage + Confirmation      | Seul le message de blocage s'affiche.                               |
| Confirmation + Confirmation | Une pop-up liste les messages, avec un seul bouton de confirmation. |
| Blocage + Blocage           | Une pop-up liste les messages, avec un seul bouton **OK**.          |
