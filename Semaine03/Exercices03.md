# Semaine 3
# Exercices 03

## Structure

À l'intérieur de votre `solution` unique pour tout le cours, nommée `1Q2-NDC`, créez un projet nommé `Exercices03` et ajoutez-y un fichier `exercices03.cpp`. Pour chaque question, créez une fonction nommée `questionX_X` où X est le numéro de la question. 

## Question 1

Dire si les conditions suivantes sont vraies ou fausses. (Attention, si vous testez les exercices dans un éditeur de code (Visual Studio), ne pas redéclarer x à chaque fois)

### 1.1
```cpp
int x = 14;
(x - 6 == 10);
(x - 6 < 10);
(10 != x + 6);
```

### 1.2
```cpp
float m = 12.4f;
float k = 12.3f;
(m > k);
(m + k <= 20);
(37 >= 2*k + m)

```

### 1.3
```cpp
int a = 1;
char b = 'W';
(a == b);
(a < b);
(a != b);
(a == true);
```

### 1.4
```cpp
int d = 1;
char c = 'W';
(d = c);
```
#### 1.4.1
Pourquoi un tel résultat de (d = c) ?

## Question 2
Écrire un programme qui demande un nombre à l’utilisateur, puis qui calcule et affiche le carré de ce nombre.
```plaintext
Entrez un nombre : 3
Le carré de 3 est 9
```

## Question 3
Écrire un programme qui demande une base et une puissance à l’utilisateur dans une seule instruction, puis qui calcule et affiche le résultat (`base` élévée à la `puissance`).
```plaintext
Entrez une base et une puissance [exemple 2 8] : 2 8
2 à la puissance 8 = 256.
```
```plaintext
Entrez une base et une puissance [exemple 2 8] : 2 32
2 à la puissance 32 = 4.29497e+09.
```

## Question 4
Écrire un programme qui demande la température de l’eau et qui affiche son état (`solide`, `liquide`, `gazeux`).  Ne pas répéter le texte « L’eau est dans un état » dans le code.  Il faut demeurer `DRY`.
```plaintext
Entrez la température de l'eau en celcius : 99.5
L'eau est dans un état liquide
```
```plaintext
Entrez la température de l'eau en celcius : -10
L'eau est dans un état solide
```
```plaintext
Entrez la température de l'eau en celcius : 100
L'eau est dans un état gazeux
```

## Question 5
Écrire un programme qui demande un nombre à l’utilisateur.  Le nombre sera valide s’il est divisible par 5 mais pas par 7.  Afficher si le nombre est valide ou invalide. Il faut demeurer `DRY` ici aussi.
```plaintext
Entrez un nombre : 50
Le nombre 50 est valide
```
```plaintext
Entrez un nombre : 35
Le nombre 35 est invalide
```

## Question 6
Écrire un programme qui demande une année à l’utilisateur et retourne si c’est une année bissextile ou pas. L’année est bissextile si elle est divisible par quatre mais pas par 100. Toutefois, les années divisibles par 400 sont bissextiles.
```plaintext
Entrez une année : 2020
2020 est une année bissextile
```
```plaintext
Entrez une année : 2001
2001 est une année régulière
```

## Question 7
En utilisant `obligatoirement` un `switch`, écrire un programme qui demande à un étudiant une note d'examen en numérique et qui la converti en cote universitaire simple, sans les + et les - (A à F seulement).

La cote suivra cette logique :
1. `A` pour tout ce qui atteint 90% ou plus.
2. `B` pour 80%.
3. `C` pour 70%.
4. `D` pour 60%.
5. `E` pour le reste.

### Indices pour la réalisation : 
1. Rappelez-vous du comportement la division entière d'un `int`. 
2. Il est possible de placer deux `case` en ligne sans `break` entre les deux pour réaliser le même code pour deux valeurs possibles.
```c++
case 10:
case 9: //code ici;
break;
```
### Voici les résultats attendus :
```plaintext
Entrez la note (0-100) : 100
La cote universitaire est : A
````
```plaintext
Entrez la note (0-100) : 91
La cote universitaire est : A
````
```plaintext
Entrez la note (0-100) : 79
La cote universitaire est : C
````
```plaintext
Entrez la note (0-100) : 59
La cote universitaire est : E
````

```plaintext
Entrez la note (0-100) : 101
Note invalide [101]. Veuillez entrer une valeur entre 0 et 100.
````

