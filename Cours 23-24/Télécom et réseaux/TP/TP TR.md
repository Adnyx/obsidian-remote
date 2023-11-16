
Normes : 568A/B

- Paires torçadées (ordre des couleurs important)
	- 568B (plus utilisé car les switches font le job)
		orange blanc
		orange
		vert blanc
		bleu
		bleu blanc
		vert
		brun
		brun blanc
	- 568A
		vert bl
		vert
		orange bl
		bleu
		bleu bl
		orange
		brun bl
		brun

--- 

		- Voir pg 6/7 (Attention QCM)
		U/UTP
		F/UPT -> l'ensemble est protégé par de l'alluminium
		F/FTP -> l'ensemble et les paires torçadées sont protégées par de l'alluminium
		S/FTP -> Protection maximale (souvent pour les usines car beaucoup de perturbations)
		F/UTQ -> plusieurs cables ensembles

--- 

		- pg 18 connaitre connecteurs fibre optique

![[TR1TP_Protocoles de labo_23-24.pdf]]

---

1.0.5)
	Partie 1)
		Routers, switches, hubs, wireless devices, security et WAN emulation
	Partie 2)
		d) ALS1, point_d'accès et  Web server
		e) Laptop_1
		f) sur la table 
	Partie 3)

---

| Classes | Masque réseau | Adresse Réseau              |
| ------- | ------------- | --------------------------- |
| A       | 255.0.0.0     | 1.0.0.0   - 126.255.255.255 |
| B       | 255.255.0.0   | 128.0.0.0 - 191.255.255.255 |
| C       | 255.255.255.0 | 192.0.0.0 - 223.255.255.255 |
| D       | 240.0.0.0     | 224.0.0.0 - 239.255.255.255 |
| E       | Non défini    | 240.0.0.0 - 255.255.255.255 |
\- À finir et connaitre-

 exemple: ==10==.__124.12.203 /8__
Network ID. __Host ID__

10.0.0.0
10.255.255.255

n max d'hotes = n - 2 où n = nbr de bit dans Host ID
$$
2^n-2
$$

| Préfixe         | Plage  IP                   |
| --------------- | --------------------------- |
| 10.0.0.0 /8     | 10.0.0.0 - 10.255.255.255   |
| 172.16.0.0 /12  | 172.16.0.0 - 172.31.255.255 |
| 192.168.0.0 /16 | 192.168.0.0 - 192.168.255.255                        |
