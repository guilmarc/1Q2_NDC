# Exercices 02

## Structure

Créez un projet nommé `Exercices02` et ajoutez-y un fichier `Exercices02.cpp`. Pour chaque question, créez une fonction nommée `exercices02_X_X` où `X` est le numéro de la question. Appelez chaque fonction dans la fonction `main`.

#### Exemple :

```cpp
void exercices02_1_1() {
  cout endl << "Exercices02 1.1" << endl;
  int a, b, c;
  a = 5;
  b = 3;
  c = a + b;
  a = 2;
  c = b - a;
  cout << "a: " << a << ", b: " << b << ", c: " << c << endl;
}

int main() {
  exercices02_1_1();
  exercices02_1_2();
  exercices02_1_3();
  //...
  return 0;
}
```

## Exerice #1

Donnes les valeurs de chacune des variables `a`, `b`, et `c` après l'exécution des codes suivant:

### 1.1

```cpp
int a, b, c;
a = 5;
b = 3;
c = a + b;
a = 2;
c = b - a;
```

### 1.2

```cpp
int a, b, c;
a = 5;
b = 3;
c = a + b;
a = 2;
c = b - a;
```

### 1.3

```cpp
int a, b, c;
a = 3;
b = 10;
c = a + b;
b = a + b;
a = c;
```

### 1.4

```cpp
int a, b, c;
a = 1;
b = a + 3;
a = 3;
```

#### 1.4.1 Pourquoi un tel résultat de `c` ?

### 1.5

```cpp
int a, b, c;
a = 10;
b = 3;
c = a / b;
```

#### 1.5.1 Pourquoi cette valeur non attendue de `c`?

#### 1.5.2 Comment obtenir approximativement `3.333333` dans la variable `c`?

## Exercice #2

Dans une fonction nommée `exercices02_2` :

1. Déclarer une variable nommée `hours` (heures) de type float. Y mettre le nombre d'heure travaillées la semaine passée (inventez-en un si vous ne travaillez pas).
2. Déclarer une variable de type float nommée `rate` (pour taux horaire). Placez-y le taux horaire ($/heure) qui vous ferait plaisir.
3. Déclarer une variable `wage` (paiement) dans lequel on place le nombre d'heures multiplié par le taux horaire. De quel type déclarez-vous la variable salaire?
4. Afficher une phrase complète qui dit quelque chose semblable à ceci: "Si on fait ... heures de travail à un taux de ... $/heure, on fera un salaire de ...
5. DÉFI: Trouvez le moyen d'afficher le salaire avec deux décimales seulement.

## Exercice #3

Dans le main de votre fichier source:

1. Déclarer 2 variables entière: x = 8 et y = 5
2. Trouver une façon pour interchanger (permuter) le contenu des 2 variables de façon dynamique (c'est-à-dire qui s'adaptera et fonctionnera peu importe les valeurs initiales de x et y).
3. Afficher les résultats AVANT et APRÈS la permutation. Par exemple, en console, on devrait voir:

```
Avant permutation x = 5 et y = 8.
Après permutation x = 8 et y = 5.
```

## DÉFI 1

Présumons un ballon étant toujours plein d'eau pure mais ayant un diamètre variable.

Écrire un programme qui demande à l'utilisateur le diamètre du ballon et qui retourne son poids en kg. La sortie doit être identique à l'exemple ci-dessous.

```plaintext
Entrez le diamètre du ballon : 14
Le poids d'un ballon de 14 cm de diamètres remplis d'eau est de 1.44kg.
```
