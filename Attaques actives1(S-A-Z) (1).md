![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.001.png)![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.002.png)

`  `Rapport  du TP2![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.003.png)

Attaques actives ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.004.jpeg)

REALISER PAR : ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.005.png)![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.006.png)

` `ZINEB EL RHAZOUANI  SAID EL OUARDI  ADIL ERRAD 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.007.png)

1. Introduction……………………………………………………………..1  
   1. Objectif du TP…………………………………………………………1.1 
2. Implémentation d’attaques actives…………………………...2  
2. Test de quelques outils d’attaques……………………………..3 

A. Attaque DHCP starvation…………………………………………….a.3 

2. Attaque “Man In The Middle” basée sur l'attaque “ARP        

spoofing”………………………………………………………………………………….b.3 

3. Attaque “usurpation d’identité”…………………………………...c.3 
3. Attaque “ARP cache poisoning”……………………………………d.3 
3. Attaque « Inondation de la table de commutation »…….e.3 

Introduction : 

Les attaques actives sont mises en place par l’injection, la modification ou la suppression de paquets. L’attaquant peut ainsi laisser les traces des attaques qu’il lance. Ces traces peuvent être exploitées par l’administrateur réseau pour déceler l’existence d’attaques et identifier l’attaquant si possible. 

v Objectifs de ce TP: 

- Implémenter quelques attaques et les tester. 
  - Mise en place de quelques attaques en 

utilisant des outils d’attaques. 

Implémentation d’attaques actives ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.008.jpeg)         Exercice 1 : my\_ping.c 

Exercice 2 : pingsur2frag.c ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.009.jpeg)

Exercice 3 : pingfragments.c ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.010.jpeg)

Exercice 4 : demandeconntcp.c ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.011.jpeg)

Test de quelques outils d’attaques ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.012.jpeg)

A. Attaque DHCP starvation 

DHCP starvation : L’attaquant inonde le serveur DHCP avec des messages DHCPREQUEST afin de réserver toutes les adresses IP disponibles sur le serveur DHCP. L’attaquant doit utiliser une nouvelle adresse MAC pour chaque requête. 

- installer des utilitaires pour dhcpstarv (Install utils for dhcpstarv).

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.013.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.014.jpeg)

- Install dhcpstarv 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.015.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.016.png)

- Configuration DHCP ![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.017.jpeg)
- Status DHCP  

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.018.jpeg)

- Test DHCP 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.019.jpeg)

- Lance l’attaque 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.020.png)

- dossier de bail avant l’attaque (lease file 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.021.jpeg)

before the attack) 

- dossier de bail avant l’attaque (lease file before the attack) 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.022.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.023.png)

- Result 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.024.jpeg)

2. Attaque “Man In The Middle” basée sur l'attaque “ARP        

spoofing ”  .    

- Etape 1 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.025.png)

- Etape2.1 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.026.jpeg)

- Etape2.2 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.027.jpeg)

- Etape3 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.028.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.029.jpeg)

3. Attaque “usurpation d’identité” 
- Etape1 : configure mac adresse 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.030.jpeg)

- etape2 : configure adresse IP 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.031.jpeg)

- Etape3 : send echo request 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.032.jpeg)

- Etape4 : send echo reply 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.033.jpeg)

- Etape 5 : Echo reply last package 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.034.jpeg)

4. Attaque “ARP cache poisoning”
- etape1 :Vérifier  la connectivite 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.035.jpeg)

- Etape2 :Arp 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.036.jpeg)

- Etape3  

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.037.jpeg)

- Etape 4 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.038.jpeg)

- Etape 5 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.039.jpeg)

5. Attaque « Inondation de la table de commutation » 
- Etape1 : adresse IP 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.040.jpeg)

- Etape1.2 : test ping 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.041.jpeg)

- 2.1 install arpflood 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.042.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.043.png)

- Test ping with arpflood 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.044.jpeg)

- Install vsftpd 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.045.png)

- Add user in vsftpd 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.046.jpeg)

- Configuration vsftpd 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.047.jpeg)

- configuration vsftpd-add user 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.048.png)

- configuration vsftpd  server 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.049.jpeg)

- Retrouver sur la troisième machine les trames correspondant 

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.050.jpeg)

![](Aspose.Words.d1438f71-9bd8-484b-b3c6-ee7391c29f42.051.jpeg)
