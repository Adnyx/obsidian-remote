
- Prob 1:
Comment déterminer que kayak est un palindrome ?

	Paramètre d'entrée: Mot
	De sortie: "Est un palindrome" ou "N'est pas un palindrome"
	Pré-condition: Doit être un mot
	Post-condition: Si un palindrome est entré, doit retourner "Est un palindrome" et inversément
	
	Palindrome = même mot à l'envers
	séparer le mot lettre par lettre dans n variables
	ajouter la valeur de toutes ces variables dans l'ordre inverse
	si la réponse est égale au mot de base, c'est un palindrome
	



- Prob 2:
Étant donné cinq entiers positifs [1,2,3,4,5], trouvez les valeurs minimale et maximale qui peuvent être calculées en additionnant exactement quatre de ces cinq entiers. Ensuite, imprimez ces valeurs.

	Paramètre d'entrée:5 entiers positifs
	De sortie: 2 entiers positifs
	Pré-condition: doit être une liste de nombres entiers positifs
	Post-condition: l'entier positif maximum doit être plus grand que le plus grand nombre de la liste
	
	ranger les entiers dans un ordre croissant
	pour la valeur maximale:
		additionner les 4 derniers ensembles
	pour la valeur minimale:
		additionner les 4 premiers ensembles

--- 
		Correction :
			somme totale - le min
			somme tot - max

---

Problème du drapeau hollandais:

	n balles rouges, blanches et bleues: ranger dans le bon ordre (stable)
	
	vérifier la balle: si elle est rouge, l'envoyer au début, si elle est bleue, l'envoyer à la fin, si elle est blanche, passer à la suivante. 

--- 
		Correction: 
			Rouge = 0, Blanc = 1, Bleu = 2
			Liste en 4 sections:
				Low, Mid, Inconnues et High
			Algo: 
				 1:  

---

##### Décodage:
e     e   t   e    n     s    t    e   t   s       /
10 10 00 10 111 010 00 10 00 010 011
t     e     l      n    e     t
00 10 0110 111 10 00
t     e    s    t
00 10 010 00
t     e   /
00 10 0
##### Encodage:
states
010001100010010
notes
11101110010010

E: 102
A: 64
S: 48
C: 35
T: 35
G: 12
H: 9

##### LZW
TOBEORNOTTOBEORTOBEORNOT

T =1
O = 2
B = 3
E = 4
R = 5
N = 6
TO = 7
BE = 8
OR = 9
NO = 10
TT = 11
TOB = 12
ORN = 13
OT = 14
1 2 3 4 2 5 6 2 1 7 8 9 12 4 9 2 1