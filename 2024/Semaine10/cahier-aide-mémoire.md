
# Aide mémoire - Examen 2
<div style="page-break-after: always;"></div>

# Boucles
## for
```cpp
for (initialisation; condition; incrémentation) {
    // instructions à exécuter à chaque itération
}
```
- Utilisée quand on connait le nombre d'itération à faire.
- `Initialisation` : Cette section initialise une ou plusieurs variables avant que la boucle ne démarre (souvent un compteur).
- `Condition` : Tant que cette condition est vraie, la boucle continue de s'exécuter. Quand la condition devient fausse, la boucle s'arrête.
- `Incrémentation` : À chaque itération, cette étape est exécutée après le bloc de code. Elle permet de modifier la ou les variables du compteur, par exemple en les incrémentant.

## while

```cpp
while (condition) {
    // instructions à répéter
}
```
- Utilisée lorsque l'on ne connait pas le nombre total d'itération.
- `condition` : une expression booléenne qui est évaluée avant chaque itération de la boucle.
  - Si la condition est vraie (true), le bloc d'instructions est exécuté.
  - Si la condition est fausse (false), la boucle s'arrête.

## do...while

```cpp
do {
    // Instructions à exécuter
} while (condition);
```
- Utilisée lorsque l'on ne connait pas le nombre total d'itération qu'il y aura mais qu'il faut qu'au moins une itération soit faite.
- `condition` : une expression booléenne qui est évaluée avant chaque itération de la boucle.
  - Si la condition est vraie (true), le bloc d'instructions est exécuté.
  - Si la condition est fausse (false), la boucle s'arrête.

# Switch

```cpp
char choix;
...

switch (choix) {
case '1':
    //Code ici
    break;
case '2':
    //Code ici
    break;
case '3':
    cout << "Au revoir!" << endl;
    break;
default:
    cout << "Choix invalide..." << endl;
    break;
}

```
# Tableaux
```cpp
void utilisationTableau() {
	int notes[] = { 90, 89, 75, 99, 95 };
	cout << notes; // <-- ceci est l'adresse mémoire du tableau de notes.\n";
	cout << notes[0]; // " <-- ceci est la valeur de la 1ère note (index = 0).\n";
	cout << notes[4]; // " <-- ceci est la valeur de la dernière note (index = 4).\n";
	cout << notes[5]; // " <-- l'index 5 n'existe pas (OutOfBound).\n";
  notes[4] = 100; //Injection d'une valeur dans le tableau (à la fin)
	cout << "Il y a " << size(notes) << " notes entrées"; //size() pour connaître le nombre d'éléments dans le tableau
}
```


# Valeurs aléatoires
```cpp
srand((unsigned int)time(0)); //Pour utiliser le temps actuel pour générer le seed 
int nombreAleatoire = (rand() % (max - min + 1)) + min 
```

# Lire un seul caractère du clavier
```cpp
#include <conio.h>

void accelererDecelerer() {
	char touche;
	cout << "Utilisez les flèches W / S pour accélérer ou décélérer (esc pour quitter)." << endl;
	do {
		touche = _getch();
		//Permettra d'effacer le texte de la console.
		system("CLS");
		switch (touche) {
			case 'w': cout << "Accélérer" << endl; break;
			case 's': cout << "Décélérer" << endl; break;
		}
	} while (touche != 27); //27 est le code ASCII pour la touche ESC
}
```
# Formatter l'affichage
  - `fixed`: s'assure de pouvoir fixer le nombre de décimal désirées.
  - `setprecision`: si utilisée avec `fixed`, précise le nombre de décimal à afficher.
  - `setw()`: fonction qui formate le texte qui suit en lui attribuant un nombre fixe de case d'affichage.  Utile pour aligner des montant par exemple.
```cpp
#include <iomanip>

void affichageFormate() {
	double notes[] = { 100, 89.4, 75.1, 99, 95.2 };
	for (int i = 0; i < size(notes); i++) {
		cout << "Note #" << i + 1 << " : " << fixed << setprecision(1) << setw(5) << notes[i] << endl;
	}
}
```
### Résultat en sortie
```plaintext
Note #1 : 100.0
Note #2 :  89.4
Note #3 :  75.1
Note #4 :  99.0
Note #5 :  95.2
```

