<p align="Center"><img src="../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# 🏋🏻‍♂️ Exercices 02 - Les variables

#### Voir la [structure à utiliser.](../_includes/_rules.md)

## 🔎 Question 01

Pour les sous-numéros suivant, vous pouvez répondre en ajoutant simplement des `commentaires //`. Vous pouvez aussi créer une fonction pour chaque sous numéros afin de tester réellement en l'exécutant, une fois la réponse trouvée par vous-même.

Donner les valeurs de chacune des variables `a`, `b`, et `c` après l'exécution des codes suivant:

### Question 1.1

```cpp
int a, b, c;
a = 5;
b = 3;
c = a + b;
a = 2;
c = b - a;
```

### Question 1.2

```cpp
int a, b, c;
a = 5;
b = 3;
c = a + b;
a = 2;
c = c + b * a;
```

### Question 1.3

```cpp
int a, b, c;
a = 3;
b = 10;
c = a + b;
b = a + b;
a = c;
```

### Question 1.4

```cpp
int a, b, c;
a = 1;
b = a + 3;
a = 3;
```

#### Question 1.4.1 Pourquoi un tel résultat de `c` ?

### Question 1.5

```cpp
int a, b, c;
a = 10;
b = 3;
c = a / b;
```

#### Question 1.5.1 Pourquoi cette valeur non attendue de `c`?

#### Question 1.5.2 Comment obtenir approximativement `3.333333` dans la variable `c`?

## 📝 Question 02

1. Déclarer 2 variables entière: x = 8 et y = 5
2. Trouver une façon pour interchanger (permuter) le contenu des 2 variables de façon dynamique (c'est-à-dire qui s'adaptera et fonctionnera peu importe les valeurs initiales de x et y).
3. Afficher les résultats AVANT et APRÈS la permutation. Par exemple, en console, on devrait voir:

```
Avant permutation x = 5 et y = 8.
Après permutation x = 8 et y = 5.
```

ATTENTION: Cela doit fonctionner avec d'autres valeurs de x et y sans rien changer d'autre que les valeurs elles-mêmes dans votre code.

## 📝 Question 03

Écrire un algorithme simple qui affiche le produit de deux nombres réels entrés par l'utilisateurs qui donnera le résultat suivant.

```plaintext
Entrez les valeurs de x, suivi de y : 11.54 9.98
Le produit de 11.54 par 9.98 est de 115.169.
```

## Question 4

Écrire le code pour convertir une température de celcius en fahrenheit.

1. Demander la température en celcius à l'utilisateur.
2. Calculer la transformation (/ pour faire une division).
3. Afficher la température à l'écran.
   La sortie doit être identique à cela :

```plaintext
Entrez la température en celcius: 32
Température = 89.6 fahrenheit.
```

## Question 5

Créez un calculateur de prix total en demandant le total du prix des achats et en calculant les taxes en vigueur au Québec en date du jour (une recherche Internet sera nécessaire).

```plaintext
Entrez le prix total des achats : 100
Le total de la vente est de : 114.75$
```

ATTENTION: Il est possible que vous arriviez à 1 ou 2 cents près. Nous accepterons cette réponse pour l'instant. La réponse sera également acceptable (pour aujourd'hui) peut importe le nombre de décimal.
