# Exercices 01

## Question #1 - Écriture d'un programme
L'objectif de votre premier exercice est de vous familiariser avec la syntaxe de C++ et de trouver par vous-même l'emplacement de certains caractères spéciaux sur votre clavier.

 Vous devez, dans cet exercice, ré-écrire au complet le programme suivant (pas de copier-coller) et ce, de façon à réussir à le faire fonctionner dans Visual Studio : 
```cpp
#include <iostream>
#include <vector>

using namespace std;
const int THROW_COUNT_MAX = 10000;

int main() {
  setlocale(LC_ALL, "");
  int throwsCount;
  do {
    cout << endl << "Combien de fois voulez-vous lancer le dé? (0 pour quitter) : ";
    cin.clear();
    cin >> throwsCount;

    if (throwsCount > THROW_COUNT_MAX) {
      cout << "Entrée invalide (" << throwsCount << ").  Veuillez entrer un nombre entre 0 et " << THROW_COUNT_MAX << ".\n";
    }
    else if (throwsCount > 0) {
      vector<int> throws(throwsCount);
    
      //Lancer le dé le nombre de fois demandé.
      for (int i = 0; i < throwsCount; i++) {
        throws[i] = rand() % 6 + 1;
      }

      //Classer le nombre d'occurence de chaque face du dé.
      int occurences[6] = { 0, 0, 0, 0, 0, 0 };
      for (int value : throws) occurences[value - 1]++;
      

      //Afficher les résultats à l'écran.
      cout << left << "Face " << "Occurences" << endl;
      for (int i = 1; i <= 6; i++) {
        cout << left << i << " -> " << occurences[i - 1] << endl;
      }
    }
  } while (throwsCount != 0);

  cout << "Fin du programme" << endl;
  return 0;
}
```
## Question #2 - Que fais ce programme ?
## Question #3 - Avez-vous réussis à le faire fonctionner sans copier-coller ?
