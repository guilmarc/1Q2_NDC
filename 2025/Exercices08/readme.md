<p align="Center"><img src="../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# 🏋🏻‍♂️ Exercices 08 - Les tableaux
## Consignes :
Vous devez faires ces exercices en utilisant des tableaux statiques, pour des raisons pédagogiques, il est **interdit** d'utiliser des vecteurs.
#### Voir la [structure à utiliser.](../_includes/_rules.md)

## 📝 Question 1 - J'ai de la mémoire !
Programmez un algorithme simple qui demande 5 notes à l'utilisateur et qui affiche ensuite les 5 notes entrées en mémoire de cette façon :
```plaintext
Entrez la note #1 : 90
Entrez la note #2 : 100
Entrez la note #3 : 89
Entrez la note #4 : 76
Entrez la note #5 : 89
Les notes entrés sont : [90, 100, 89, 76, 89]
```

## 🏆 Question 2 - Big Big Big Winner !
Programmez un algorithme qui demande un nombre paramétrable (en code dans une constante NOTES_COUNT) de notes d'examens en validant que l'entrée de l'utilisateur soit entre 0 et 100.  Continuez l'algorithme en détectant la plus haute note entrée ainsi que le numéro de l'étudiant qui a eu cette note :
```plaintext
Entrez la note #1/5 : 101
Entrez la note #1/5 : -10
Entrez la note #1/5 : 90
Entrez la note #2/5 : 98
Entrez la note #3/5 : 68
Entrez la note #4/5 : 79
Entrez la note #5/5 : 80

Recherche de la plus haute note, un instant svp...

La plus haute note est 98.  Obtenue par l'étudiant #2;
```
```plaintext
Entrez la note #1/1 : 90

Recherche de la plus haute note, un instant svp...

La plus haute note est 90.  Obtenue par l'étudiant #1.
```

## 🎲 Question 3 - Jouons aux dés
Nous voulons ici simuler une quantité paramétrable (THROWS_COUNT) de lancers d'un dé possédant un nombre paramétrable de faces (FACES_COUNT) et, par la suite, afficher la quantité de chacune des faces obtenus.

```plaintext
Voici les résultats pour 10 lancers d'un dés de 6 faces.

***************
*  RÉSULTATS  *
***************
*   1 :     2 *
*   2 :     0 *
*   3 :     1 *
*   4 :     0 *
*   5 :     4 *
*   6 :     3 *
***************
```
```plaintext
Voici les résultats pour 100 lancers d'un dés de 12 faces.

***************
*  RÉSULTATS  *
***************
*   1 :     6 *
*   2 :     3 *
*   3 :    11 *
*   4 :     5 *
*   5 :    10 *
*   6 :     7 *
*   7 :     8 *
*   8 :     6 *
*   9 :     7 *
*  10 :    15 *
*  11 :    10 *
*  12 :    12 *
***************
```
```plaintext
Voici les résultats pour 100000 lancers d'un dés de 6 faces.

***************
*  RÉSULTATS  *
***************
*   1 : 16628 *
*   2 : 16719 *
*   3 : 16458 *
*   4 : 16752 *
*   5 : 16769 *
*   6 : 16674 *
***************
```
## 🅰️ Question 4 - Les voyelles à Isabelle
Programmez un calculateur de voyelles à qui on donnera un texte dans une constante et qui sortira le nombre de chacunes des voyelles.

N.B. Une variable de type `string` est l'équivalent d'un tableau de `char` !
### Utiliser ce texte :
- Le C++ est utilisé pour coder des applications mobiles, pour créer des jeux vidéo ou encore pour programmer des logiciels de bureautique. En comparaison avec d'autres langages de programmation, C++ offre les avantages suivants : 1. C++ est relativement simple à maîtriser. Dans la mesure où il fait partie des langages de programmation les plus utilisés, une documentation fournie est disponible en ligne pour apprendre les règles d'écriture du code C++. Le développeur, en outre, accède à de nombreuses classes et fonctions intégrées, depuis la bibliothèque standard de C++, pour programmer facilement son application. Certains développeurs créent des bibliothèques en open source pour accéder à des ressources avancées. Enfin, la POO simplifie l'organisation du code. 2. C++ s'exécute très rapidement. C'est notamment pour cette raison qu'il est particulièrement utilisé en gaming, où les exigences de performance sont élevées. Une étude classe d'ailleurs C++ dans le top 5 des langages de programmation : il figure 3ème au classement en matière de temps d'exécution, devançant Java et Swift ; ses performances sont également notables en matière de consommation maximale de mémoire et de consommation d'énergie.
### Résultat attendu :
```plaintext
**************
*  VOYELLES  *
**************
*  A :    75 *
*  E :   171 *
*  I :    67 *
*  O :    66 *
*  U :    45 *
*  Y :     0 *
**************
* Tot:   424 *
**************
```

## 🎲🎲 Question 5 (défi) - Jouons aux dés optimisé
Optimiser le code de la question #3 en s'assurant de n'obtenir qu'un maximum de `17` ligne de code incluant les `{}`.

<hr><p align="Center"><img src="../_includes/end.png" alt="drawing" width="150"/></p>