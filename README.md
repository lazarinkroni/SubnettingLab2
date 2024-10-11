# SubnettingLab2

Cisco Packet Tracer Subnetting Lab 2

English Version

Overview
This project demonstrates subnetting a network (192.168.1.0/24) into three smaller subnets using Cisco Packet Tracer. The configuration includes two PCs, two routers, and two switches. The network is divided as follows:

Subnet A: 192.168.1.0/26
Subnet B: 192.168.1.64/26
Subnet C: 192.168.1.128/26

Topology
The network consists of:

PC1 connected to Switch S1, which is part of Subnet A.
PC2 connected to Switch S2, which is part of Subnet C.
Router R1 connected to Subnet A and Subnet B.
Router R2 connected to Subnet B and Subnet C.

Tasks

Subnet the network: Divide 192.168.1.0/24 into three subnets.

Configure Subnet A (PC1, S1, R1).

Configure Subnet B between the routers.

Configure Subnet C (PC2, S2, R2).

Configure PCs with the first IP address in the subnet.

Configure the routers with the last IP address in the subnet.

Configure the switches with the second IP address in the subnet.

Verify connectivity: Ensure all devices can ping each other.

Step-by-Step Guide

Step 1: Subnet the Network
Divide the original network (192.168.1.0/24) into three /26 subnets:
Subnet A: 192.168.1.0/26 (Range: 192.168.1.1 - 192.168.1.62, Broadcast: 192.168.1.63)
Subnet B: 192.168.1.64/26 (Range: 192.168.1.65 - 192.168.1.126, Broadcast: 192.168.1.127)
Subnet C: 192.168.1.128/26 (Range: 192.168.1.129 - 192.168.1.190, Broadcast: 192.168.1.191)

Step 2: Configure PCs
PC1 Configuration (Subnet A):

IP Address: 192.168.1.1
Subnet Mask: 255.255.255.192
Default Gateway: 192.168.1.62
PC2 Configuration (Subnet C):

IP Address: 192.168.1.129
Subnet Mask: 255.255.255.192
Default Gateway: 192.168.1.190
Step 3: Configure the Routers
Router R1 Configuration:

Interface Gig0/0/0 (Subnet A):
IP Address: 192.168.1.62
Subnet Mask: 255.255.255.192
No Shutdown
Interface Gig0/0/1 (Subnet B):
IP Address: 192.168.1.65
Subnet Mask: 255.255.255.192
No Shutdown
Router R2 Configuration:

Interface Gig0/0/0 (Subnet B):
IP Address: 192.168.1.66
Subnet Mask: 255.255.255.192
No Shutdown
Interface Gig0/0/1 (Subnet C):
IP Address: 192.168.1.190
Subnet Mask: 255.255.255.192
No Shutdown
Step 4: Configure the Switches
Switch S1 (Subnet A):

IP Address: 192.168.1.2
Subnet Mask: 255.255.255.192
Switch S2 (Subnet C):

IP Address: 192.168.1.130
Subnet Mask: 255.255.255.192
Step 5: Verify Connectivity
Use the ping command on PC1 to ping PC2.
Verify that all devices can communicate across the network.

Versione Italiana
Panoramica

Questo progetto dimostra la suddivisione di una rete (192.168.1.0/24) in tre sottoreti più piccole utilizzando Cisco Packet Tracer. La configurazione include due PC, due router e due switch. La rete è divisa come segue:

Sottorete A: 192.168.1.0/26
Sottorete B: 192.168.1.64/26
Sottorete C: 192.168.1.128/26

Topologia
La rete è composta da:

PC1 connesso a Switch S1, che fa parte della Sottorete A.

PC2 connesso a Switch S2, che fa parte della Sottorete C.

Router R1 connesso alla Sottorete A e alla Sottorete B.

Router R2 connesso alla Sottorete B e alla Sottorete C.

Compiti

Sotto-segmentare la rete: Dividere 192.168.1.0/24 in tre sottoreti.

Configurare la Sottorete A (PC1, S1, R1).

Configurare la Sottorete B tra i router.

Configurare la Sottorete C (PC2, S2, R2).

Configurare i PC con il primo indirizzo IP nella sottorete.

Configurare i router con l'ultimo indirizzo IP nella sottorete.

Configurare gli switch con il secondo indirizzo IP nella sottorete.

Verificare la connettività: Assicurarsi che tutti i dispositivi possano comunicare tra loro.

Guida Passo-Passo

Passo 1: Sotto-segmentare la Rete

Dividere la rete originale (192.168.1.0/24) in tre sottoreti /26:
Sottorete A: 192.168.1.0/26 (Intervallo: 192.168.1.1 - 192.168.1.62, Broadcast: 192.168.1.63)
Sottorete B: 192.168.1.64/26 (Intervallo: 192.168.1.65 - 192.168.1.126, Broadcast: 192.168.1.127)
Sottorete C: 192.168.1.128/26 (Intervallo: 192.168.1.129 - 192.168.1.190, Broadcast: 192.168.1.191)

Passo 2: Configurare i PC

Configurazione di PC1 (Sottorete A):

Indirizzo IP: 192.168.1.1
Maschera di Sottorete: 255.255.255.192
Gateway Predefinito: 192.168.1.62

Configurazione di PC2 (Sottorete C):

Indirizzo IP: 192.168.1.129
Maschera di Sottorete: 255.255.255.192
Gateway Predefinito: 192.168.1.190
Passo 3: Configurare i Router

Configurazione di Router R1:

Interfaccia Gig0/0/0 (Sottorete A):
Indirizzo IP: 192.168.1.62
Maschera di Sottorete: 255.255.255.192
No Shutdown
Interfaccia Gig0/0/1 (Sottorete B):
Indirizzo IP: 192.168.1.65
Maschera di Sottorete: 255.255.255.192
No Shutdown

Configurazione di Router R2:

Interfaccia Gig0/0/0 (Sottorete B):
Indirizzo IP: 192.168.1.66
Maschera di Sottorete: 255.255.255.192
No Shutdown
Interfaccia Gig0/0/1 (Sottorete C):
Indirizzo IP: 192.168.1.190
Maschera di Sottorete: 255.255.255.192
No Shutdown

Passo 4: Configurare gli Switch
Switch S1 (Sottorete A):

Indirizzo IP: 192.168.1.2
Maschera di Sottorete: 255.255.255.192

Switch S2 (Sottorete C):

Indirizzo IP: 192.168.1.130
Maschera di Sottorete: 255.255.255.192
Passo 5: Verificare la Connettività
Utilizzare il comando ping su PC1 per pingare PC2.
Verificare che tutti i dispositivi possano comunicare sulla rete.
