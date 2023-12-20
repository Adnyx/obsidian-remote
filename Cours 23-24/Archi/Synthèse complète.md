
### Débit

Unité: bps, b/s, bit/s
		 Bps, B/s, octet/s

Pour augmenter le débit:
- Augmenter les fréquences
- Augmenter le nbr de canaux

### Latence

La latence est une durée en ms, µs ou ns

Synonymes: __Lag, Ping__

On ne peut pas dépasser la vitesse de déplacement des électrons dans un cable cuivre ou des photons dans une fibre optique

### CPU, Central Processing Unit

Sert à calculer et diriger les données

Composé de: 
- Transistors (pour calculer)
	- Interrupteurs à commande électrique, calcules grâces aux portes logiques
- Mémoires (pour fournir les données aux transistors)
- Bos de données (i/o)

##### Architecture interne du CPU

- Unité de contrôle
- ALU, Arithmetic Logical Unit
- Registres
- FPU, Floating Point Unit
- Unité vectorielle
- Mémoire cache L1et L2
- I/O

#### Big.LITTLE

![[Big.LITTLE.png]]

##### Finesse de gravure

Plus la finesse est élevée, plus les transistors sont petits, moins ils consomment, moins ils chauffent, moins ils prennent de place

##### Overclocking

Augmenter la fréquence du CPU
Pour overclocker, on peut devoir augmenter la tension -> chauffe plus. (risqué)

### TDP, Thermal Design Power

$TDP = k{V^2}f$

k = constante (fonction du processeur)
V = tension électronique
f = fréquence

TDP s'exprime en watts (W)

##### Différents types de refroidissements
- Passifs (big chunk O' copper)
- Actifs (Big fan)

##### FLOPS 

$FLOPS = nbrCoeurs * fréquence * \frac{FLOP}{cycle}$

##### Jeu d'instructions

- x86 (x86, x64, x86-64) - la plupart des pc
- ARM (Smart tv, gps,...)

