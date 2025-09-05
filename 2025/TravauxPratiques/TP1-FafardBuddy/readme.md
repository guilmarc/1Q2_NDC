<p align="Center"><img src="../../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# TP1 - Fafard Buddy (5%)
<p align="Center"><img src="./images/team.avif" alt="drawing" width="350"/></p>

## Introduction
Capitaine Patenaude, responsable de la conduite du Romano-Fafard, un vaisseau spacial inter-planétaire, a du mal à calculer la vitesse qu'il doit atteindre afin de  s'éloigner d'une planète.  Cette dernière, à cause de sa masse, le ramène trop souvent vers elle quand le vaisseau ne va pas assez vite.

Mr. Patenaude a communiqué avec vous et vous a attribué la mission de lui fournir un outils le guidant dans la vitesse à atteindre.  Il souhaite pouvoir sélectionner la planète du système solaire à quitter ainsi que la distance entre le vaisseau et cette planète.

Il a déjà préparé des sorties d'écran qu'il vous demande de respecter à la lettre autant au niveau des fonctionnalités que du visuel.

## Étapes à réaliser
1. Faire afficher le message d'invite.
2. Demander le chiffre de la planète où se trouve Capitaine Patenaude (1 à 8).
3. À l'aide d'un switch, enregistrer les bonnes valeurs dans les variables et validez que le numéro de planète est valide.
4. Demander l'altitude à laquelle le vaisseau se trouve actuellement (en mètres).
5. Effectuer le calcul nécessaire.
6. Afficher le résultat à l'écran.
   
## Sorties d'écran
### Décollage de la terre à 2500m d'altitude
```
************************************************
*                 Fafard Buddy                 *
************************************************
[1] - Mercure            [5] - Jupiter
[2] - Venus              [6] - Saturne
[3] - Terre              [7] - Uranus
[4] - Mars               [8] - Neptune
************************************************
Vous voulez quitter quelle planète ? : 3
Vous êtes à quelle altitude en mètres ? : 2500
************************************************
Calcul en cours de la vitesse à atteindre sur
la planète terre à 2500 mètres d'altitude...
************************************************

Capitaine Patenaude, mettez les gaz à 40255km/h !
```

### Décollage de Jupiter à 40000m d'altitude
```
************************************************
*                 Fafard Buddy                 *
************************************************
[1] - Mercure            [5] - Jupiter
[2] - Venus              [6] - Saturne
[3] - Terre              [7] - Uranus
[4] - Mars               [8] - Neptune
************************************************
Vous voulez quitter quelle planète ? : 5
Vous êtes à quelle altitude en mètres ? : 40000
************************************************
Calcul en cours de la vitesse à atteindre sur
la planète jupiter à 40000 mètres d'altitude...
************************************************

Capitaine Patenaude, mettez les gaz à 216772km/h !
```

### Gestion des erreurs
```
************************************************
*                 Fafard Buddy                 *
************************************************
[1] - Mercure            [5] - Jupiter
[2] - Venus              [6] - Saturne
[3] - Terre              [7] - Uranus
[4] - Mars               [8] - Neptune
************************************************
Vous voulez quitter quelle planète ? : 9

ERREUR - Planète invalide !
```

## Un peu de théorie
Lorsqu’un objet ou un astre est en orbite autour d’un autre astre, il possède une vitesse d’évasion. Si cette vitesse est atteinte, l’objet quittera son orbite et s’éloignera définitivement de l’astre central.

### Formule de la vitesse d'évasion
$$
v_{e} = \sqrt{\frac{2 * G * M}{r}}
$$

- $v_{e}$ : Vitesse d’évasion recherchée (en mètres par seconde).
- G : La constante gravitationnelle $6.6743 \times 10^{-11}$.
- M : Masse de la planète en question.
- r : Distance entre le vaisseau et le centre de la planète.

### Masse et diamètres
| # | Planète   | Masse (kg)                  | Diamètre (km) |
|---|-----------|-----------------------------|---------------------------|
| 1 | Mercure   | 3.30 × 10^23                | 4 879                     |
| 2 | Vénus     | 4.87 × 10^24                | 12 104                    |
| 3 | Terre     | 5.97 × 10^24                | 12 742                    |
| 4 | Mars      | 6.42 × 10^23                | 6 779                     |
| 5 | Jupiter   | 1.90 × 10^27                | 139 820                   |
| 6 | Saturne   | 5.68 × 10^26                | 116 460                   |
| 7 | Uranus    | 8.68 × 10^25                | 50 724                    |
| 8 | Neptune   | 1.02 × 10^26                | 49 244                    |

<hr>
<p align="Center"><img src="./images/end.png" alt="drawing" width="150"/></p>