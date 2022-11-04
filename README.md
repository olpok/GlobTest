# GlobTest


## Enoncé

[Echo](https://www.instagram.com/globalisecho/?hl=fr), mascotte de l'équipe de [Globalis](https://www.globalis-ms.com/), a découvert une fonction `foo()` bien mystérieuse. Hélas, il n'a pas accès au code. Curieux et grand amateur de [rétro-ingénierie](https://fr.wikipedia.org/wiki/R%C3%A9tro-ing%C3%A9nierie), Echo s'est amusé à appeler cette fonction, en injectant des données en entrée et en récoltant les sorties. Le comportement de la fonction `foo()` est le suivant :

|  Appel     |  Sortie     |
| ---   |:-:    |
| `foo([[0, 3], [6, 10]])` | `[[0, 3], [6, 10]]` |
| `foo([[0, 5], [3, 10]])` | `[[0, 10]]` |
| `foo([[0, 5], [2, 4]])` | `[[0, 5]]` |
| `foo([[7, 8], [3, 6], [2, 4]])` | `[[2, 6], [7, 8]]` |
| `foo([[3, 6], [3, 4], [15, 20], [16, 17], [1, 4], [6, 10], [3, 6]])` | `[[1, 10], [15, 20]]` |

Le challenge, si vous l'acceptez, serait d'aider Echo à comprendre ce que fait cette fonction et à la recoder. Vous êtes partant ? ;)

### Question 1

Expliquez, en quelques lignes, ce que fait cette fonction.

La fonction foo() prend en paramètres des tableaux et renvoie 2 tableaux :
Si 2 tableaux en entrée : 
si le 2ème élément de premier tableau est plus petit que le premier élément du second tableau
on renvoie les mêmes tableaux ;
sinon on renvoie les valeurs min et max ;

Si plus de tableaux en entrée :
On récupère le plus petit et le plus grand nombre inférieur au premier élément du tableau ayant la plus grand somme
On renvoie en premier le tableau contenant le plus petit et grand nombre suivi du tableau ayant la plus grand somme

### Question 2

Codez cette fonction.
Merci de fournir un fichier contenant :

- la fonction, 
- l'appel de la fonction, avec un jeu de test en entrée,
- l'affichage du résultat en sortie.

### Question 3

Précisez en combien de temps vous avez implémenté cette fonction.

J'ai trouvé la logique et codé la fonction hier soir en 1h-1h20 approximativement, mais je voulais soumettre un code « clean » ce matin. 

## Merci

Par avance, un grand merci pour le temps que vous consacrerez à ce challenge, en espérant vous voir rejoindre très prochainement [nos équipes](https://www.globalis-ms.com/jobs/) ;) 