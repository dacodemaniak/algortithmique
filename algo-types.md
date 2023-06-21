## Les types en algorithmique
### Algorithme : Définition des types
### Role : Voir les différents types scalaires simples
### Résultat : aucun
```
DEBUT
    VAR chaine: CHAINE <- "Sans limite de taille"
    VAR autre_chaine: CHAINE[5] <- "31200"

    VAR longueur: ENTIER <- LONG(chaine) // Nombre de caractère de la variable chaine

    // Concaténation : ajouter des chaînes entre elles
    VAR nom_cp: CHAINE <- chaine + autre_chaine
    // Sans limite de taille31200
    VAR pretty_cp: CHAINE <- chaine + " " + autre_chaine
    // Sans limite de taille 31200

    VAR alphabet: CARACTERE <- "A"
    alphabet <- SUCC(alphabet) // alphabet vaudra B
FIN
```
### Algorithme : Booléens
### Role : définition et opérations sur les booléens
### Résultat : aucun
```
DEBUT
    VAR trouve: BOOLEEN <- VRAI
    VAR cache: BOOLEEN <- FAUX
    VAR montre: BOOLEEN <- VRAI

    // Illustration de l'opérateur ET
    VAR resultat: BOOLEEN <- trouve ET cache // FAUX

    // Illustration de l'opérateur OU
    resultat <- trouve OU cache // VRAI

    // Illustration du OU exclusif
    cache <- NON cache // VRAI
    resultat <- cache XOU montre // FAUX
FIN
```

### Algorithme : Numériques
### Role : Définitions et opération sur les numériques
### Résultat : aucun
```
DEBUT
    VAR entier_1, entier_2: ENTIER <- 5
    VAR reel_1: REEL <- 2.5

    VAR carre: ENTIER <- entier_1 * entier_2

    VAR result_1 <- entier_1 + entier_2 * entier_1
    // 1. entier_2 * entier_1 => 25
    // 2. entier_1 + 25 => 30

    VAR result_2 <- (entier_1 + entier_2) * entier_1
    // 1. entier_1 + entier_2 => 10
    // 2. 10 * 5 => 50

    VAR div_entiere: ENTIER <- reel_1 DIV entier_1 // 0.5 => 0
    VAR modulo: ENTIER <- reel_1 MOD entier_1 // 0.5 => 5
    VAR division: REEL <- reel_1 / entier_1 // 0.5

    VAR est_vrai: BOOLEEN <- entier_1 > reel_1
    // >, <, >=, <=, =, <> (ou noté !=)
FIN
```

