# Exercices 05
Lien vers les [notes de cours](https://slides.com/hkoncept/1q2-05/fullscreen?token=6ntlmUIx#/7) sur les boucles `for()`.

## Conditions

N.B. Tous les numéros doivent s'exécuter sans aucun avertissement dans Visual Studio et doivent être conforme à l'affichage présenté.

## Question 1 - Table de multiplication

Écrire un programme qui demande un multiplicateur et multiplicande, et qui ensuite écrit la table de multiplication de ce multiplicande jusqu’au nombre multiplicateur :

```plaintext
Entrez un multiplicande : 7
Entrez le nombre de multiplicateurs : 8
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
```

## Question 2 - Factorielle

Écrire un programme qui demande un nombre à l'utilisateur et qui calcule la `factorielle` de ce nombre.

```plaintext
Entrez un nombre [1 à 10] : 2
La factorielle de 2 est 2.
```

```plaintext
Entrez un nombre [1 à 10] : 10
La factorielle de 10 est 3628800.
```

## Question 3 - Affichage ASCII

En utilisant une seule boucle `for()`, écrire un programme qui affiche une partie de la table des caractères ASCII à partir du caractère 120 jusqu'au dernier caractère de la table.

Vous aurez besoin de connaître le code de transformation d'un nombre en caractère ascii. Pour ce faire, il faut le caster en char comme suit :

```cpp
cout << (char)nombre;
```

Votre affichage doit être identique à celui-ci :

```plaintext
120=x   121=y   122=z   123={   124=|   125=}   126=~   127=    128=?   129=?
130='   131=ƒ   132="   133=.   134=┼   135=╬   136=^   137=%   138=S   139=<
140=O   141=?   142=Z   143=?   144=?   145='   146='   147="   148="   149=
150=-   151=-   152=~   153=T   154=s   155=>   156=o   157=?   158=z   159=Y
160=    161=¡   162=¢   163=£   164=¤   165=¥   166=¦   167=§   168=¨   169=©
170=ª   171=«   172=¬   173=­    174=®   175=¯   176=°   177=±   178=²   179=³
180=´   181=µ   182=¶   183=·   184=¸   185=¹   186=º   187=»   188=¼   189=½
190=¾   191=¿   192=À   193=Á   194=Â   195=Ã   196=Ä   197=Å   198=Æ   199=Ç
200=È   201=É   202=Ê   203=Ë   204=Ì   205=Í   206=Î   207=Ï   208=Ð   209=Ñ
210=Ò   211=Ó   212=Ô   213=Õ   214=Ö   215=×   216=Ø   217=Ù   218=Ú   219=Û
220=Ü   221=Ý   222=Þ   223=ß   224=à   225=á   226=â   227=ã   228=ä   229=å
230=æ   231=ç   232=è   233=é   234=ê   235=ë   236=ì   237=í   238=î   239=ï
240=ð   241=ñ   242=ò   243=ó   244=ô   245=õ   246=ö   247=÷   248=ø   249=ù
250=ú   251=û   252=ü   253=ý   254=þ   255=ÿ
```

## Précisions

- N.B. Pour ce numéro et les prochains numéros, nous présumerons que les caractères affichées à l'écran sont carré (et non rectangulaire comme en vérité) pour des raisons de simplicité. Nous considérons donc un 5 caractères par 5 caractères comme un carré.

## Question 4 - Rectangle

En utilisant une boucle for() dans une boucle for(), écrivez un programme qui permet de dessiner un rectangle (ou un carré) avec le nombre d'étoiles entrés en paramètres comme présenté dans l'affichage suivant :

```plaintext
Entrer la largeur du rectangle : 20
Entrer la hauteur du rectangle : 5
********************
********************
********************
********************
********************
```

## Question 5 - Triangle

En utilisant une boucle `for()` dans une boucle `for()`, écrivez un programme qui permet de dessiner un triangle-rectangle dont les deux côtés de l'angle droit sont de même longueur en considérant l'affichage suivant :

```plaintext
Entrer la hauteur du triangle-rectangle : 10
*
**
***
****
*****
******
*******
********
*********
**********
```

## DÉFI Question 6 - Triangle inversé

Reprendre la Question 5 mais inverser le triangle :

```plaintext
Entrer la hauteur du triangle-rectangle : 10
         *
        **
       ***
      ****
     *****
    ******
   *******
  ********
 *********
**********
```

## DÉFI Question 7 - Pyramide

En utilisant des boucles `for()`, écrivez un programme qui permet de dessiner une pyramide en considérant l'affichage suivant :

```plaintext
Entrer la hauteur de la pyramide : 5
    *
   ***
  *****
 *******
*********
```

<p align="Center"><img src="./images/end.png" alt="drawing" width="150"/></p>
