# Exercice Rendu Monnaie
### Algorithme : Rendu Monnaie
### Rôle : Ventilation d'un rendu de monnaie en espèce par type de billet et / ou pièce
### Résultat : Obtenir le nombre de billets de 100, de 50, de 20, de 10, de 5 et le nombre de pièces de 2 euros
```
DEBUT
    CONST PRIX_PRODUIT: ENTIER <- 75
    CONST SOMME_VERSEE: ENTIER <- 100
    CONST A_RENDRE: ENTIER  <- SOMME_VERSEE - PRIX_PRODUIT

    VAR billet100, reste100, billet50, reste50, billet20, reste20, billet10, reste10, billet5, reste5, piece2, reste2: ENTIER <- 0

    // Traitement pour les billets de 100
    billet100 <-  A_RENDRE DIV 100 // Dans ce cas 0
    reste100 <- A_RENDRE MOD 100 // Dans ce cas 25 / 100 => 0.25 donc 25

    // Traitement pour les billets de 50
    billet50 <- reste100 DIV 50 // Dans ce cas 0
    reste50 <- reste100 MOD 50 // Dans ce cas 25 / 50 => 25

    // Traitement pour les billets de 20
    billet20 <- reste50 DIV 20 // Dans ce cas 25 / 20 => 1
    reste20 <- reste50 MOD 20 // Dans ce cas 5 / 20 => 5

    // Traitement pour les billets de 10
    billet10 <- reste20 DIV 10 // Dans ce cas 5 / 10 => 0
    reste10 <- reste20 MOD 10 // Dans ce cas 5

    // Traitement pour les billets de 5
    billet5 <- reste10 DIV 5 // Dans ce cas 1
    reste5 <- reste10 MOD 5 // Dans ce cas 0

    // Traite les pièces de 2
    piece2 <- reste5 DIV 2 // Dans ce cas 0
    reste2 <- reste5 MOD 2 // Dans ce cas 0
FIN
```
