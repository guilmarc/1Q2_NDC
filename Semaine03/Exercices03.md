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
float m = 12.4;
float k = 12.3;
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

## Question 2
Écrire un programme qui demande un nombre à l’utilisateur, puis qui calcule et affiche le carré de ce nombre.
```plaintext
Entrez un nombre : 3
Le carré de 3 est 9
```

## Question 3
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

## Question 4
Écrire un programme qui demande un nombre à l’utilisateur.  Le nombre sera valide s’il est divisible par 5 mais pas par 7.  Afficher si le nombre est valide ou invalide. Il faut demeurer `DRY` ici aussi.
```plaintext
Entrez un nombre : 50
Le nombre 50 est valide
```
```plaintext
Entrez un nombre : 35
Le nombre 35 est invalide
```

## Question 5
Écrire un programme qui demande une année à l’utilisateur et retourne si c’est une année bissextile ou pas. L’année est bissextile si elle est divisible par quatre mais pas par 100. Toutefois, les années divisibles par 400 sont bissextiles.
```plaintext
Entrez une année : 2020
2020 est une année bissextile
```
```plaintext
Entrez une année : 2001
2001 est une année régulière
```
