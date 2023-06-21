### Algorithme : Déclaration de variables

### Role : Définir des variables en algorithmique

### Résultats : Simple déclaration de variables

```
DEBUT
    VAR ma_variable: CHAINE
    VAR mon_age: ENTIER <- 55

    ma_variable <- "Jean-Luc Aubert"

    ma_variable <- "007"

    // ma_variable vaudra "007"
    // mon_age vaudra 55
FIN
```

### Algorithme : Définition des constantes
### Role : Définir des constantes en algorithmique
### Résultat : aucun

```
DEBUT
    CONST MA_CONSTANTE : REEL <- 0.20

    VAR prix_produit_ht: REEL <- 1.50

    VAR prix_ttc: REEL

    VAR surface: REEL
    CONST RAYON: ENTIER <- 3

    prix_ttc <- prix_produit_ht * (1 + MA_CONSTANTE)

    prix_produit_ht <- 1.75

    prix_ttc <- prix_produit_ht * (1 + MA_CONSTANTE)

    MA_CONSTANTE <- 0.07 // Opération illégale

    surface <- PI * (rayon * rayon)
FIN
```




