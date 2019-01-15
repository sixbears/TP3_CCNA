# TP3_CCNA

## 4. Configuration réseau d'une machine CentOS
### a. utilisez une commande pour prouver que vous avez internet depuis la VM

Pour vérifier que l'on a accès à internet depuis la VM on peut utiliser `curl -sl www.google.com` (par exemple). On recuperera le fichier HTML si l'on est bien connecté à internet.

### b. prouvez que votre PC hôte et la VM peuvent communiquer

Pour Prouver que les machines peuvent communiquer il faut `ping` l'IP notre VM depuis notre PC et inversement. 

### c. affichez votre table de routage sur la VM et expliquez chacune des lignes

Pour afficher la table de routage il faut taper `ip route` 
Chaque numero correspond à une de nos carte réseau suivi de son nom.

## 5. Faire joujou avec quelques commandes

### Ping 

*`ping` hôte -> VM  
  `ping 172.168.127.10` je `ping` l'adresse ip de ma VM depuis mon PC.
  
*`ping` VM -> hôte
  `ping 10.33.3.183` Je `ping` l'adresse ip de mon PC depuis ma VM.
  
Pour connaitre son adresse IP `ipconfig /all` sous Windows et `ip a` sous Linux

### Afficher la table de routage

*De l'hôte
sous Windows pour afficher la tabel de routage `netstat -arn`

*De la VM
Sous Linux pour afficher la table de routage `ip route`

*la ligne qui leur permet de se connecter est 
  
