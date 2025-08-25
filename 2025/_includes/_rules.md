## 📂 Structure à utiliser

À l'intérieur de votre emplacement central unique pour tout le cours, créez un projet nommé au nom de l'exercice (exemple `Exercices02` ). Pour chaque question, créez une fonction nommée `questionX_X` où X est le numéro de la question. Exemple `question01_2` pour la questions 1.2. Appelez chaque fonction dans la fonction `main`.

#### Exemple :

```cpp
//Fonction pour la question 3.1
void question02_1() {
  cout endl << "Question 2.1" << endl;
  cout << "L'erreur est que..." << endl;
}

//On appelle les fonctions ici
int main() {
  question01();
  question02_1();
  question02_2();
  //question02_3(); //Les // veulent dire que cette fonction ne seras pas déclenchée.
  //...
  return 0;
}
```
