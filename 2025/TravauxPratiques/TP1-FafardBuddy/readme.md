<p align="Center"><img src="../../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# TP1 - Fafard Buddy (5%)
<p align="Center"><img src="./images/team.avif" alt="drawing" width="350"/></p>

## Introduction
Capitaine Patenaude, responsable de la conduite du Romano-Fafard, un vaisseau spacial inter-planétaire, a du mal à calculer la vitesse qu'il doit atteindre afin de  s'éloigner d'une planète.  Cette dernière, à cause de sa masse, le ramène trop souvent vers elle quand le vaisseau ne va pas assez vite.

Mr. Patenaude a communiqué avec vous et vous a attribué la mission de lui fournir un outils le guidant dans la vitesse à atteindre.  Il souhaite pouvoir sélectionner la planète du système solaire qu'il souhaite quitter ainsi que la distance entre le vaisseau et cette planète.

Il a déjà préparé des sorties d'écran qu'il vous demande de respecter à la lettre autant au niveau des fonctionnalités que du visuel.

## Sorties d'écran
Disponibles bientôt !

## Un peu de théorie
Lorsqu’un objet ou un astre est en orbite autour d’un autre astre, il possède une vitesse d’évasion. Si cette vitesse est atteinte, l’objet quittera son orbite et s’éloignera définitivement de l’astre central.

### Formule de la vitesse d'évasion
$$
v_{e} = \sqrt{\frac{2 * G * M}{r}}
$$

- $v_{e}$ : Vitesse d’évasion recherchée.
- G : La constante gravitationnelle $6.67430 \times 10^{-11} \; \text{m}^3 \, \text{kg}^{-1} \, \text{s}^{-2}$.
- M : Masse de la planète en question.
- r : Distance entre le vaisseau et le centre de la planète.

### Masse et diamètres
| Planète   | Masse (kg)                  | Diamètre (km) |
|-----------|-----------------------------|---------------------------|
| Mercure   | 3.30 × 10^23                | 4 879                     |
| Vénus     | 4.87 × 10^24                | 12 104                    |
| Terre     | 5.97 × 10^24                | 12 742                    |
| Mars      | 6.42 × 10^23                | 6 779                     |
| Jupiter   | 1.90 × 10^27                | 139 820                   |
| Saturne   | 5.68 × 10^26                | 116 460                   |
| Uranus    | 8.68 × 10^25                | 50 724                    |
| Neptune   | 1.02 × 10^26                | 49 244                    |

<p align="Center"><img src="./images/end.png" alt="drawing" width="150"/></p>