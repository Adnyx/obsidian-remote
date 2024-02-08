
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

##### Benchmarks
Logiciel développé dans le but d'évaluer les performances

#### RAM (Random access memory (Très chouette album de daft punk))
La RAM contient les données nécessaires au CPU pour calculer.
Ces données sont stockées temporairement.
Les informations peuvent y être accédées directement
##### DRAM et SRAM
La DRAM est moins cher et plus compacte;
La SRAM est plus cher, plus complexe et plus rapide.

Il existe plusieurs format de RAM: DIMM et SO-DIMM
Savoir comment connaitre la latence par rapport au timing (flemme)

##### UDIMM et RDIMM
UDIMM: unbuffered, le CPU s'occupe de l'addressage RAM (grand publique)
RDIMM: registered, mini CPU sur la RAM qui s'occupe de l'addressage (souvent pour serveurs)

##### ECC
Error correction code, détection des éventuelles erreurs dans la RAM
##### RANK
Single rank: une seule rangée de mémoires
Double ranks: deux rangées de mémoires qui peuvent êtres accédées simultanément

#### Disques durs
HDD: lents
SSD: rapides
Favoriser un temps d'accès petit -> Un débit 2 fois plus élevé avec un temps d'accès plus lent peut être plus lent qu'un petit débit avec un temps d'accès réel plus court.

##### Fragmentation
Un HDD mets les données à un emplacement physique. Si l'emplacement n'est pas assez grand, il coupe la donnée et met la fin ailleurs avec un lien entre elles. La défragmentation sert à regrouper les parties de données séparées. Ne pas défragmenter un SSD.

##### IOPS
Input/output operations per second
IOPS séquentiel (l'un à la suite de l'autre) est à l'image du débit.
IOPS aléatoire est à l'image des temps d'accès.

##### SSD
Les SSD sont purement électroniques, plus rapides, plus résistants aux choques, moins dans le temps.

##### NAND Flash
SLC - single level cell: plus cher, plus efficace
MLC - multi level cell: cher, efficace (attention, censé être 2 bits mais les vendeurs se servent de l'appellation pour vendre des + de 2bits)
TLC - triple level cell, moins efficace, moins cher
QLC - quadruple level cell, bof bof, pas cher

##### RAID
Segmenter sur 2 disques physiques pour augmenter la sécurité et la performance
Raid0: performance x2
raid1: performance et sécurité
raid5: 4 disques

RAID logiciel: segmentation faite par le CPU
RAID pseudo-matériel: 

#### Carte-mère
C'est l'élément qui connecte tous les autre éléments du PC.
##### BIOS 
Interface graphique qui permet une configuration spécifique.
Permet de démarrer l'OS
##### Chipset
Chef d'orchestre de la carte mère. 

##### VRM
Les VRMs permettent de mieux gérer les variations de tension dans une carte mère. Elles sont importantes.

##### Formats
EATX, ATX, MICRO-ATX, MINI-ATX,...
Le format standard est ATX

#### PSU (power supply unit (très chouette album de paft dunk))
Une alim doit livrer des tensions stables, avoir assez de puissance, avoir un bon rendement, être silencieuse, 

Les alims transforment le courant 240V AC en 12V DC (chaleur à évacuer)
Calculer l'alim nécessaire: $1,5.(TDP_{CPU}+TGP_{GPU}+100W)$ ou utiliser un outil en ligne

##### Rendement
Bronze, silver, gold, platinum, titanium. Prendre au moins gold (pour faire des économies sur le long terme)

#### GPU
Calculs graphiques (cher) ou scientifiques (très très très très cher)
Entrée PCI-Express 16x
Sorties écran
Alim
VRAM (RAM pour GPU)

##### Formats:
GPU's with integrated graphics (pas ouf)
Soudé à la carte mère (pc portable et certains serveurs)
Carte graphique (dedicated gpu)

##### Pour choisir:
Pour le jeu
1) Marques réputées
2) Bande passantes
3) Consommation
4) Refroidissements intégrés
5) dimensions
Pour le calcul
1) La marque
2) Bande passante
3) Quantité VRAM
4) Interface
5) Support logiciel

##### Bande passante
Ne dois pas être sous-estimé ! 
Fréquence de fonctionnement * largeur de bus = bande passante





