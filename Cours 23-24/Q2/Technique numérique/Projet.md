Projet 5, due 22 avril

1- Déterminer la table de vérité. -------OK
2- Déterminer les expressions simplifiées des sorties (a, b, c, d, e, f, g) en
fonction des entrées A, B et C.
3- Donner le circuit logique de commande.
4- Simuler sur multism et tinkercad

## Table de vérité

| A   | B   | C   | a     | b     | c     | d     | e     | f     | g     |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| 0   | 0   | 0   | x     | x     | x     | x     | x     | x     | x     |
| 0   | 0   | 1   | 0     | 0     | 0     | ==1== | 0     | 0     | 0     |
| 0   | 1   | 0   | ==1== | 0     | 0     | 0     | 0     | 0     | ==1== |
| 0   | 1   | 1   | ==1== | 0     | 0     | ==1== | 0     | 0     | ==1== |
| 1   | 0   | 0   | ==1== | ==1== | 0     | 0     | 0     | ==1== | ==1== |
| 1   | 0   | 1   | ==1== | ==1== | 0     | ==1== | 0     | ==1== | ==1== |
| 1   | 1   | 0   | ==1== | ==1== | ==1== | 0     | ==1== | ==1== | ==1== |
| 1   | 1   | 1   | x     | x     | x     | x     | x     | x     | x     |

d = C

