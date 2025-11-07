<p align="Center"><img src="../_includes//logo.jpg" alt="drawing" width="100"/></p>
<h5 align="Center">1Q2 - Programmation structurée</h5>

# 🏋🏻‍♂️ Exercices 09 - Les Fonctions

## Conditions

- Tous les numéros doivent s'exécuter sans aucun avertissement dans Visual Studio et doivent être conforme à l'affichage présenté.

## Question 1 - On passe au cash !

Compléter l'algorithme suivant en créant les fonctions manquantes :

```cpp
#include <iomanip>

void question01() {
  float montant = fournirMontantValide();
  float total = calculerMontantTotal(montant);
  cout << "Le total est de : " << fixed << setprecision(2) << total << endl;
}
```

```plaintext
Entrez le montant de achats : 95
Le total est de : 109.23
```

## Question 2 - Maxime le Maximum

Compléter l'algorithme suivant en créant les fonctions manquantes :

```cpp
void question02() {
  const int TAILLE_TABLEAU = 10;
  const int NOMBRE_MIN = 1;
  const int NOMBRE_MAX = 1000;
  int nombres[TAILLE_TABLEAU];

  remplirTableauNombresAleatoires(nombres, size(nombres), NOMBRE_MIN, NOMBRE_MAX);

  cout << "Le tableau de nombres est : ";
  afficherTableau(nombres, size(nombres));
  cout << endl;

  int max = trouverMax(nombres, size(nombres));
  cout << "Le maximum du tableau est : " << max << endl;
}
```

```plaintext
Le tableau de nombres est : [42, 468, 335, 501, 170, 725, 479, 359, 963, 465]
Le maximum du tableau est : 963
```

## Question 3 - C'est moi le premier !

Compléter l'algorithme suivant en créant les fonctions manquantes :

```cpp
void question03() {
  const unsigned short NOMBRE_MAX = 100;
  int min, max;
  cout << "Entrez le nombre du début de l'interval [0 à " << NOMBRE_MAX << "] : ";
  min = fournirNombreValide(0, 100);
  cout << "Entrez le nombre de la fin de l'intervale [" << min << " à 100] : ";
  max = fournirNombreValide(min, 100);
  cout << "Voici le nombres premiers de " << min << " à " << max << " : " << endl;
  for (int i = min; i < max; i++) {
    if (estNombrePremier(i)) {
      cout << i << "\t";
    }
  }
}
```

```plaintext
Entrez le nombre du début de l'interval [0 à 100] : 50
Entrez le nombre de la fin de l'intervale [50 à 100] : 90
Voici le nombres premiers de 50 à 90 :
53      59      61      67      71      73      79      83      89
```

## Question 4 - Suis-je réutilisable ?

Compléter l'algorithme suivant en créant les fonctions manquantes :

```cpp
void question04() {
  const int TAILLE_TABLEAU = 10;
  const int NOMBRE_MIN = 1;
  const int NOMBRE_MAX = 1000;
  int nombres[TAILLE_TABLEAU];

  remplirTableauNombresAleatoires(nombres, size(nombres), 1, 1000);

  cout << "Le tableau de nombres est : ";
  afficherTableau(nombres, size(nombres));
  cout << endl;

  float moyenne = calculerMoyenne(nombres, size(nombres));
  cout << "La moyenne des " << size(nombres) << " nombres est de " << moyenne << endl;
}
```

```plaintext
Le tableau de nombres est : [42, 468, 335, 501, 170, 725, 479, 359, 963, 465]
La moyenne des 10 nombres est de 450.7
```

## Question 5 - Cantine chez Rodrique.

Compléter l'algorithme suivant en créant la fonction manquante. Ici on simule un `hot-dog` représenté en `string`. Le but est simple; être capable d'y ajouter des ingrédients.

```cpp
void question05() {
  string hotdog = "pain saucisse";
  string ingredient;
  cout << "Entrez les ingrédients pour garnir le hot-dog (terminer avec 'servir') : ";
  do {
    cin >> ingredient;
    if (ingredient != "servir") {
      garnirHotDog(hotdog, ingredient);
    }
  } while (ingredient != "servir");
  cout << "Le hot-dog est prêt : " << hotdog << endl;
}
```

```plaintext
Entrez les ingrédients pour garnir le hot-dog (terminer avec 'servir')
ketshup
relish
moutarde
servir
Le hot-dog est prêt : pain saucice ketshup relish moutarde
```

## Question 6 (défi) - Call Me !

Dans ce numéro vous devrez créer une première fonction `question06()` qui va appeler une fonction `fibonacci()` fonctionnant en mode `récursif` et qui, au final, ne contient que deux ligne de code dans la fonction.

```plaintext
Entrez le position du nombre de fibonacci que vous désirez obtenir [1 à 100] : 20
Le nombre de fibonacci à la position 20 est : 6765
```

### N.B. Informez l'enseignant si vous avez fait un ou des défis.

<hr><p align="Center"><img src="../_includes/end.png" alt="drawing" width="150"/></p>
