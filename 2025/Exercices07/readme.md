<p align="Center"><img src="../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# 🏋🏻‍♂️ Exercices 07 - Les boucles `while(){}`

#### Voir la [structure à utiliser.](../_includes/_rules.md)

## Question 1 - Lance et... compte !

Écrire un algorithme qui effectue le compte et le décompte jusqu'à / depuis un nombre référence entré par l'utilisateur.

### Critères

- Vous n'avez droit de déclarer que deux variables ou moins.

```plaintext
Entrez le nombre de référence : 25
0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25
25 24 23 22 21 20 19 18 17 16 15 14 13 12 11 10 9 8 7 6 5 4 3 2 1 0
```

## Question 2 - C'est un facteur !

Écrire un algorithme qui calcule la factorielle d'un nombre référence entré par l'utilisateur.

```plaintext
Entrez un nombre : 15
La factorielle de 15 est 1307674368000.
```

## Question 3 - Que la force soit avec toi !

Écrire un algorithme qui distribue une quantité variable de points de force parmi 2 à 5 joueurs.

```plaintext
Combien de points de force voulez-vous distribuer ? [10 à 100] : 100
Combien de joueurs dans cette partie ? [2 à 5] : 5
Il reste 100 points de forces.  Combien voulez-vous en donner au joueur #1 ? : 29

Il reste 71 points de forces.  Combien voulez-vous en donner au joueur #2 ? : 17

Il reste 54 points de forces.  Combien voulez-vous en donner au joueur #3 ? : 28

Il reste 26 points de forces.  Combien voulez-vous en donner au joueur #4 ? : 14

Le dernier joueur (#5) reçoit 12 points.
```

## Question 4 - Hey! ces lapins.

Écrire un algorithme qui demande un emplacement référence dans la [suite de Fibonacci](https://fr.wikipedia.org/wiki/Suite_de_Fibonacci) et qui affiche ensuite la suite jusqu'à cet emplacement.

```plaintext
Entrez le nombre de termes de la suite de Fibonacci [3 à 100] : 10
Suite de Fibonacci : [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```

```plaintext
Entrez le nombre de termes de la suite de Fibonacci [3 à 100] : 100
Suite de Fibonacci : [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, 10946, 17711, 28657, 46368, 75025, 121393, 196418, 317811, 514229, 832040, 1346269, 2178309, 3524578, 5702887, 9227465, 14930352, 24157817, 39088169, 63245986, 102334155, 165580141, 267914296, 433494437, 701408733, 1134903170, 1836311903, 2971215073, 4807526976, 7778742049, 12586269025, 20365011074, 32951280099, 53316291173, 86267571272, 139583862445, 225851433717, 365435296162, 591286729879, 956722026041, 1548008755920, 2504730781961, 4052739537881, 6557470319842, 10610209857723, 17167680177565, 27777890035288, 44945570212853, 72723460248141, 117669030460994, 190392490709135, 308061521170129, 498454011879264, 806515533049393, 1304969544928657, 2111485077978050, 3416454622906707, 5527939700884757, 8944394323791464, 14472334024676221, 23416728348467685, 37889062373143906, 61305790721611591, 99194853094755497, 160500643816367088, 259695496911122585, 420196140727489673, 679891637638612258, 1100087778366101931, 1779979416004714189, 2880067194370816120, 4660046610375530309, 7540113804746346429, 12200160415121876738, 1293530146158671551, 13493690561280548289, 14787220707439219840, 9834167195010216513, 6174643828739884737, 16008811023750101250, 3736710778780434371, 1298777728820984005]
```

## Question 5 - Palin Qui ?

Écrire un algorithme qui détecte les [palindrome](https://fr.wikipedia.org/wiki/Palindrome) et quitte seulement lorsque l'utilisateur entre 0 comme nombre.

```plaintext
Entrez un nombre : 121
Palindrome !
Entrez un nombre : 12345678987654321
Palindrome !
Entrez un nombre : 101010
Pas de chance !
Entrez un nombre : 12321
Palindrome !
Entrez un nombre : 0
```

## Question 6 - Ça chauffe ???

Écrire un algorithme qui se choisi un nombre mystère au hasard entre un et NOMBRE_MAX (constante paramétrable dans le code) et qui demande à répétition un nombre à l'utilisateur jusqu'à-ce qu'il trouve le nombre mystère. L'algorithme assiste l'utilisateur en disant :

- `Trop petit!` si le nombre est trop petit et éloigné du nombre mystère.
- `Trop petit mais tu chauffe!` si le nombre essayé est à moins de 10% (par rapport au NOMBRE_MAX) de distance du nombre mystère.
- `Trop petit mais tu chauffe. Tu brûle même!` si le nombre essayé est à moins de 0.5% (par rapport au NOMBRE_MAX) de distance du nombre mystère
- Même chose pour `Trop grand!`

### Consignes

- Il est obligatoire d'être totalement DRY lors du développement de cet algorithme.
- Il est possible de jouer sans fin en répondant `o` à chaque fin de jeu.

### Exemple d'exécution

```plaintext
*************************************
* Devinez un nombre entre 1 et 1000 *
*************************************
Essais #1 : 500
Trop grand!
Essais #2 : 300
Trop petit mais tu chauffe!
Essais #3 : 310
Trop petit mais tu chauffe!
Essais #4 : 340
Trop petit mais tu chauffe!
Essais #5 : 390
Trop grand mais tu chauffe!
Essais #6 : 350
Trop grand mais tu chauffe. Tu brûle même!
Essais #7 : 345
Trop petit mais tu chauffe. Tu brûle même!
Essais #8 : 347

Bravo, vous avez trouvé le nombre 347 en 8 essais !
Jouer une autre partie ? [(o)ui ou (n)on]
```

## Question 7 (Défi) - Ça chauffe encore plus

Reprendre le numéro 6 et ajouter-y :

- La notion de nombre d'essaie maximum (paramétrable).
- Un algorithme de calcul d'un score (utilisez votre créativité).

## Question 8 (Défi) - Vraiment on brûle !!!

Reprendre le numéro 7 et ajoutez-y :

- La possibilité à l'aide de menus de paramétrer le nombre maximum (NOMBRE_MAX).
- La possibilités d'aller consulter la liste des 5 meilleurs scores et des noms de joueurs associés.

### N.B. Informez l'enseignant si vous avez fait un ou des défis.

<hr><p align="Center"><img src="../_includes/end.png" alt="drawing" width="150"/></p>
