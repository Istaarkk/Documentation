
1. UARTS :
	1. Communication **asynchrone**
	2. 2 fils : TX, RX
	3. Pas d’horloge → les deux doivent avoir le **même baudrate**
	4. Très courant 
2. I²C :
	1. 2 fils : SDA (données), SCL (horloge)
	2. Un **maître** et plusieurs **esclaves** (adressés)
	3. Vitesse : 100 kHz à 3.4 MHz
3. SPI :
	1. 4 fils : MOSI, MISO, SCK, SS
	2. Communication **full-duplex**
	3. Très rapide : jusqu’à plusieurs dizaines de MHz	4. 
4. USB : 
	1. Remplace RS-232
	2. Plug & Play
	3. Débits : USB 1.1 → USB4 (40 Gbit/s)

| Protocole | Nb fils     | Vitesse      | Distance     | Mode         | Usage                  |
|-----------|-------------|--------------|--------------|--------------|-------------------------|
| UART      | 2           | Faible       | Grande       | Asynchrone   | Modules simples         |
| I²C       | 2           | Moyenne      | Courte       | Synchrone    | Capteurs                |
| SPI       | 4+          | Élevée       | Courte       | Synchrone    | Périphériques rapides   |
| USB       | 2 diff.     | Très élevée  | Moyenne      | Paquets      | PC, mobiles             |
| PCIe      | Lanes diff. | Extrême      | Très courte  | Point à point| GPU, NVMe               |

