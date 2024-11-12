# Les fonctions
Une fonction est un nom que l’on donne à un groupe d’instructions. On peut alors placer ces instructions en dehors du main. Lorsqu’il faut exécuter ces instructions, on appelle la fonction par son nom et le programme va exécuter les instructions de la fonction et revient continuer son code à l'endroit où il était lors de l'appel de la fonction.

## Signature de fonction
### Le nom de la fonction
- Peut contenir des lettres, chiffres et le caractère de soulignement _.
- Dans le cadre du cours, on continue avec le camelCase pour les noms de fonctions.
- Ne peut pas commencer par un chiffre.
- Sensible à la casse : fonctionA et fonctiona sont deux noms différents.
### Le type des paramètres (s'il y en a)
- Placés dans les parenthèses de la définition de la fonction.
### Le type de retour
- Le type de retour est le type de la valeur que la fonction renvoie après son exécution. Si la fonction ne retourne rien, le type de retour est void. Les types sont les mêmes que pour les variables (int, char, string, une struct, etc.)
- On ne peut pas retourner de tableau (on étudiera cette structure plus tard)
- Un retour est une valeur ou un groupe de valeurs qui résulte du traitement dans la fonction.  Exemple, une fonction qui retourne l'âge selon la date de naissance.

## Appel d'une fonction simple
Voici le code présentant l'appel d'une fonction simple.  Ici on a hardcodé les jeux...
```cpp
void afficherMenu() {
	cout << "**********************************" << endl;
	cout << "* EGAMES | Choississez votre jeu *" << endl;
	cout << "**********************************" << endl;
	cout << "* 1. Fortnite                    *" << endl;
	cout << "* 2. Minecraft                   *" << endl;
	cout << "* 3. Grand Theft Auto V          *" << endl;
	cout << "* 4. Call of Duty : MWII         *" << endl;
	cout << "* 5. Roblox                      *" << endl;
	cout << "**********************************" << endl;
}


void validerChoix() {
	unsigned short choix;

	do {
		afficherMenu();
		cout << "Entrez un choix entre 1 et 5 : ";
		cin >> choix;
		system("cls");
	} while (choix < 1 || choix > 5);
	cout << "Choix #" << choix << " validé.";
}
```
Cela fonctionne mais cause un problème de taille; il faut reprogrammer la fonction `afficherMenu()` pour chaque changement de jeu.  Que faire si le jeu provient d'une



<p align="Center">
<img src="./images/end.png" alt="drawing" width="150"/></p>