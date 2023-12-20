
![[PDF-TRIntro.pdf]]


		PG 35: def réseaux
		PG 36:
			PAN (Personal Area Network)
			LAN (Local Area Network)
			MAN (Metropolitan Area Network)
			WAN (Wide Area Network)
		PG 40: Diff entre unicast, multicast et broadcast
		PG 50: Def Internet, intranet, extranet
		PG 59: Multiplexage et segmentation
		PG 60 -> 63: 4 caractéristiques de base
			La redondance n'est pas possible à tous les niveaux
		PG 64: BYOD
		PG 65 -> 67: Vitrualisation
		PG 67: Cloud computing
		PG 70: CPL

--- 

![[PDF-TRchap5.pdf]]


---


![[02 - TR1TR1 - chapitre 2 2023 2024 (new) fini.pdf]]

---

![[05 - TR1TR1 - chapitre 5 2023 2024 (new) fini.pdf]]

---

![[03 - TR1TR1 - chapitre 3 2023 2024 (new) fini.pdf]]



### Adressage IP

- Classes A, B et C

adresse réseau et broadcast ne sont pas attribuables

Unicast addresses (d'un hôte à un autre)
broadcast (vers tous les hôtes)
multicast (groupes d'hôtes)


---
11111111.11111111.11111111.111

2^32-SM

1. 122.60.42.50 255.255.255.224 (/27)

- Adresse réseau: 122.60.42.50
- Adresse broadcast: 122.60.42.255
- nbr hôtes théorique / pratique: 
	- $2^{32-27} = 2^{5} = 32$
	- $2^{32-27}-2 = 2^{5}-2 = 30$
- Plage d'adresse utilisable: de 122.60.40.51 à 122.60.42.72

2. 10.20.30.200 255.255.255.248 (/29)

- Adresse réseau:10.20.30.200
- Adresse broadcast: 10.20.30.208
- nbr hôtes théorique / pratique:
	- $2^{32-29} = 2^{3} = 8$
	- $2^{32-29} -2= 2^{3}-2 = 6$
- Plage d'adresse utilisable: 10.20.30.201 - 10.20.30.207 

3. 172.76.111.200 /21 

- Adresse réseau: 172.76.104.0
- Adresse broadcast: 172.76.111.255
- nbr hôtes théorique / pratique:
	- 16
	- 14
- Plage d'adresse utilisable: 172.76.104.1 - 172.76.111.254

5. 192.168.70.45 /23 (+8)

- Adresse réseau: 192.168.70.0
- Adresse broadcast: 292.168.70.2
- nbr hôtes théorique / pratique: 
	- 2
	- 1
- Plage d'adresse utilisable: 192.168.70.1

6. 161.98.122.187 /26

- Adresse réseau: 161.98.122.187
- Adresse broadcast: 161.98.122.251
- nbr hôtes théorique / pratique: 
	- $2^{32-26} = 2^{6} = 64$
	- $2^{32-26}-2 = 2^{6}-2 = 62$
- Plage d'adresse utilisable:


---

32 - 1
31 - 2
30 - 4
29 - 8
28 - 16
27 - 32
26 - 64
25 - 128


   192.168.100.100
$a_{i}$= 3     2     1     0

si le subnet mask est inférieur à 25, y ajouter 8 et ajouter 1 à i (de $a_{i}$)


---

1) 115.92.12.50 255.255.255.192 (/26)
	- Adresse réseau: 115.92.12.50
	- Adresse broadcast: 115.92.12.114
	- nbr hôtes théorique / pratique:
		- 64
		- 62
	- Plage d'adresse utilisable: 115.92.12.51 - 115.92.12.113

2) 16.17.18.19 /24
	- Adresse réseau: 16.17.18.0
	- Adresse broadcast: 16.17.19.255
	- nbr hôtes théorique / pratique:
		- 2
		- 1
	- Plage d'adresse utilisable: 16.17.18.20

3) 172.16.43.82 /22
	- Adresse réseau: 172.16.43.0
	- Adresse broadcast: 172.16.44.255
	- nbr hôtes théorique / pratique:
		- 
	- Plage d'adresse utilisable:

4) 195.212.98.15 /18
	- Adresse réseau:
	- Adresse broadcast:
	- nbr hôtes théorique / pratique:
	- Plage d'adresse utilisable:

5) 10.100.206.43 /21
	- Adresse réseau:
	- Adresse broadcast:
	- nbr hôtes théorique / pratique:
	- Plage d'adresse utilisable: