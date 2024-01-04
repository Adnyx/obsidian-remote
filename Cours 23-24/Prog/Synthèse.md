# Déclarer une variable

Pour déclarer une variable, il suffit d'y mettre un mot ou une lettre suivi d'un signe égal. Ce mot doit commencer par une lettre et ne peut pas contenir d'espaces. Il existe quelques conventions pour nommer des variables:
- Ne pas commencer par une majuscule;
- Utiliser des underscores \_ si besoin d'utiliser plusieurs mots ou coller les mots et commencer le 2e par une majuscule
- Utiliser des noms de variables précis correspondant à leur utilisation.
- etc...

Exemples: 
```python
x = 1
strng = "Hello"
threeWordsVariable = "This is a 3 word variable"
three_words_variable= "Same as above"
```
En python, on peut déclarer plusieurs variables sur une même ligne:
x, y, z = 1, 2, 3 # Ici, x vaut 1, y vaut 2 et z vaut 3
ou 
x = y = z = 3 # Ici, x, y et z valent tous 3
# Les commentaires

En programmations, un commentaire sert à donner des informations supplémentaires sur notre code. Ces commentaires seront ignorés lors de l'interprétation ou la compilation du code.
En python, on déclare un commentaire en utilisant "#". Tout ce qui suivra un hashtag sur une même ligne sera ignoré. 
Pour déclarer un commentaire de plusieurs lignes, on encadre le commentaire par 3 apostrophes.

Exemples:
```python
while True: # This prints "Hello world" forever ! (this is the comment btw)
	print("Hello world")

''' 
This is a
multiple line
	comment.
'''
```
# Les Arrays

Il y a 4 types d'arrays en python:
- Les listes: Ordonnée et changeable (peut comprendre des dupliqués)
	On les déclare avec des [ ] et des virgules entre chaque éléments.
	On accède à un élément de tel façon: print(list[1]) # 1 étant le 2e élément
	On peut utiliser un index négatif: print(list[-1]) # -1 étant le dernier élément
	Ranges: 
	```python
	thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"] 
	print(thislist[2:5])
	```
	Ouput: "cherry", "orange", "kiwi"

	Changer une valeur:
	```python
	thislist = ["apple", "banana", "cherry"] 
	thislist[1] = "blackcurrant" 
	print(thislist)
	```
	Output: ["blackcurrant", "banana", "cherry"] 

	Loop: 
	```python
	thislist = ["apple", "banana", "cherry"] 
	for x in thislist: 
		print(x)
	```
	Output: 
		apple 
		banana 
		cherry

	Conditionnel
	```python
	thislist = ["apple", "banana", "cherry"] 
	if "apple" in thislist: 
		print("Yes, 'apple' is in the fruits list")
	```
	Output: Yes, 'apple' is in the fruits list

	print(len(liste)) pour déterminer la longueur de la liste
	liste.append("orange") pour ajouter "orange" à la fin
	liste.insert(1, "orange") pour ajouter "orange" en position 1
	liste.pop() pour enlever l'élément à l'index spécifié (le dernier si rien n'est précisé)
	del liste[0] pour enlever l'élément à l'index spécifié (toute la liste si rien n'est précisé)
	liste.clear() pour vider la liste
	liste2 = liste1.copy() pour copier la liste dans une autre
	liste3 = liste1 + liste2 pour joindre les 2 listes
	ou
	```python
	for i in liste2:`
		`liste1.append(i)`
	```
	ou
	```python
	list1.extend(list2)
	```
- Les tuples: Ordonné et inchangeable (peut comprendre des dupliqués)
	On déclare un tuple avec des () et des virgules entre chaque éléments 
	Les différentes utilisations des tuples sont similaires aux listes, la différence étant qu'on ne peut pas changer un tuple. La seule façon est de convertir le tuple en liste puis le reconvertir en tuple.
	On ne peut pas supprimer d'éléments d'un tuple mais on peut supprimer complètement un tuple: `del tuple1
	`tuple3 = tuple1 + tuple2` pour joindre 2 tuples

- Les sets: Désordonné et non-indexé (ne peut pas comprendre des dupliqués)
	On déclare un set avec des {} et des virgules entre chaque éléments.
	Un set n'a pas d'indexes puisqu'il est désordonné mais on peut accéder à ses éléments grâce à une for loop.
	On ne peut pas changer les éléments d'un set mais on peut y ajouter des éléments 
	```python
	thisset.add("coucou")`
	```
	On peut ajouter plusieurs éléments à un set avec la méthode update()
	```python
	thisset = {"apple", "banana", "cherry"} 
	thisset.update(["orange", "mango", "grapes"])
	```
	On peut supprimer un élément d'un set avec les méthodes .remove() ou .discard()
	On peut supprimer le dernier élément d'un set avec le .pop() mais puisqu'ils sont désordonnés, on ne saura pas quel élément est supprimé.
	.clear() vide le set.
	`del set1` supprime le set.
	Le reste et similaire aux listes

- Les dictionnaires: Désordonné, changeable et indexé (ne peut pas comprendre des dupliqués)
	Pour déclarer un dictionnaire, on utilise des {} chaque valeur doit être accompagnée d'une clé, les valeurs sont séparées des clés par des : et les groupes sont séparés par des virgules:
	```python
	dict = {"key1" : "value1", "key2" : "value2"}
	```
	```python
	for x in thisdict.values(): 
		print(x)
	```
	va afficher les valeurs du dictionnaire
	```python
	for x, y in thisdict.items():
		print(x, y)
	```
	va afficher les clés et les valeurs

	Pour ajouter des valeurs:
	```python
	dict["newKey"] = "newValue"
	```
	Le reste est similaire aux autres types d'arrays


# Les conditions 

- Equals: a == b
- Not Equals: a != b
- Less than: a < b
- Less than or equal to: a <= b
- Greater than: a > b
- Greater than or equal to: a >= b

if, elif et else. Attention à l'indentation
# Les boucles

### For loops

Avec un for, on peut exécuter du code pour chaque élément, par exemple, d'une liste, d'un dictionnaire, d'un tuple, d'un set,...
Exemple:
```python
fruits = ["apple", "banana", "cherry"] 
for x in fruits: 
print(x)
```
Output: `["apple", "banana", "cherry"] 

Avec `continue`, on peut passer une itération et passer à la suite:
```python
fruits = ["apple", "banana", "cherry"] 
for x in fruits: 
	if x == "banana": 
		continue 
	print(x)
```
Output: `["apple",  "cherry"] 

On peut casser la boucle `for` avec un `break`:
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits: 
	if x == "banana": 
		break 
print(x)
```
Output: `["apple"]`

Il est possible d'exécuter une for loop un certain nombre de fois avec la fonction `range()`
```python
for x in range(6)
	print(x)
```

À noter: la for loop exécutera le code de 0 à 5 et pas de 1 à 6 ou de 0 à 6

### While loops

Une boucle while exécutera le code indenté tant que la condition est vraie.
Un "while True:" ne s'arrêtera donc jamais sauf si un "break" est contenu dans la boucle.

Exemples:

```python
while True: # Ce code ne s'arrêtera jamais
	print("Hello World !")
```

```python
while True: # Ce code s'exécutera une fois
	print("Hello World !")
	break
```

Il est possible de créer une boucle while qui se fini avec un compteur:
```python
counter = 0 #Sets the counter to a default value
while counter < 10: #Code is gonna execute until the counter is smaller than 10
	print(counter) #Prints the current value of the counter
	counter += 1 #Adds 1 to the counter

```

Un `else` peut être utilisé après un `while` pour exécuter du code lorsque la condition n'est plus vraie.

# Les fonctions

Pour déclarer une fonction on utilise le mot clé `def`:
```python
def fonction1(): #Defines the function
	print("Je suis une fonction")

fonction1() #Calls the function
```
Output: `Je suis une fonction`

Une fonction peut avoir besoin d'arguments pour fonctionner:

```python
def fonction1(x):
	print(x+3)

fonction1(4)
```
Output: `7`

On peut également donner des arguments par défaut à une fonction:
```python
def fonction1(x=5):
	print(x+3)

fonction1(4)
fonction1()
```
Output: 
`7`
`8`

Il est aussi possible de faire passer une liste comme argument de fonction:
```python
def my_function(food): 
	for x in food: 
		print(x) 
	
fruits = ["apple", "banana", "cherry"] 
my_function(fruits)
```
Output: `["apple", "banana", "cherry"]`

Pour qu'une fonction retourne une valeur, on utilise le mot clé `return`

```python
def fonction1(x=5):
	return x+3

fonction1(4) #Il ne se passe rien de visuel. on peut utiliser:
x = fonction(4)
print(x) #Outputs 7
print(fonction1(4)) #Outputs 7
```

Les fonctions ne peuvent pas rester vide. Si vous devez en écrire une mais voulez la laisser pour plus tard, utilisez le mot clé `pass`:
```python
def myFunction():
	pass
```

### Fonctions récursives

Une fonction récursive est une fonction qui s'appelle elle même. Il est important de faire attention de ne pas créer de fonction qui ne fini pas ou qui utilise trop de CPU power ou de mémoire. Dans l'exemple suivant, la fonction `tri_recurtion()` s'appellera elle-même. Elle utilisera la variable `k` comme donnée à qui on soustraira 1 à chaque récursion. La récursion se finira lorsque la condition est <= à 0. La meilleure façon de comprendre c'est d'expérimenter. 

```python
def tri_recursion(k): 
	if(k>0): 
		result = k+tri_recursion(k - 1) 
		print(result) 
	else: 
		result = 0 
	return result 

print(" \ n \nRecursion Example Results") 

tri_recursion(6)
```

# Fichiers

Pour travailler avec des fichiers en python, il est impératif de les ouvrir avant leur utilisation et de les fermer après les avoir utilisés.
La fonction `open()` utilise 2 paramètres: Le nom du fichier et le mode d'ouverture
Modes d'ouvertures:
- "r" - Read, mode par défault
- "a" - Append
- "w" - Write
- "x" - Créer un fichier (erreur si le fichier existe déjà)
- "t" - mode texte
- "b" - mode binaire

voici comment l'utiliser:
```python
file = open("fichier.txt", "r")
```

Maintenant, voici le fichier `demofile.txt`
```
Bonjour, ceci est un test. Je suis ton ami
```

Pour lire ce fichier, on peut utiliser la fonction `read()`

```python
file = open("demofile.txt")
print(file.read())
```
Output: `Bonjour, ceci est un test.`

On peut donner un argument int à `read()` et il lira les x premiers charactères du fichier.
Il existe également la fonction `readline()` qui permet de lire une ligne du fichier. Si on utilise 2 fois `readline()`, python lira les  premières lignes du fichier.

##### Fermer un fichier
Pour fermer un fichier, on utilise la méthode `.close()`:
```python
file = open("demofile.txt")
print(file.read())
file.close()
```

Si on ouvre un fichier avec l'argument "w", on peut écrire dans le fichier:
```python
file = open("demofile.txt","w")
file.write("Attention, ceci a écrasé tout ce qui se trouvé dans le fichier")
file.close()
```

Pour éviter tout désagrément de type écrasage de données, on peut ajouter du text avec l'argument "a".
```python
file = open("demofile.txt","a")
file.write("Ce texte s'est ajouté à la fin du fichier")
file.close()
```

##### Supprimer un fichier

Pour supprimer un fichier, il faut importer le module os:

```python
import os

os.remove(demofile.txt)
print("You deleted your only friend :(")
```

Pour supprimer un dossier, on peut utiliser la fonction `rmdir()` du module os

```python
import os

os.rmdir("monDossier") #Supprime le dossier uniquement s'il est vide.
```

# Les exceptions

Les exceptions servent à controller les potentielles erreurs et éviter les crashs. 

##### Try - Except

En python, pour gérer les erreurs, on va utiliser la notation 
```python
try:
	#code here
except #exceptions:
	#code here
```

Par exemple, si le code demande de diviser par un input utilisateur, il va de soi que l'input ne puisse pas être 0, ça mènerait à une `ZeroDivisionError`. Mais on ne veut pas que le programme crash pour autant si ça arrive. On peut donc utiliser une structure du genre:

```python
while true:
	try:
		print("Que voulez-vous diviser ?(x/y)")
		x = input("x: ")
		y = input("y: ")
		print(x/y)
	except ZeroDivisionError:
		print("Veuillez ne pas diviser par 0")
```

#### Erreurs de base:

- ZeroDivisionError:
	Quand on force python à diviser par 0
- ValueError
	Lorsqu'une fonction reçoit un argument d'un type approprié mais d'une valeur inacceptable
- TypeError
	Lorsqu'une donnée n'a pas le bon type
- AttributeError
	Lorsqu'on essaie d'activer une méthode qui n'existe pas
- SyntaxError
	Lorsqu'on commet une erreur de syntaxe