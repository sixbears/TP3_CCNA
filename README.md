# TP3_CCNA

# I. Création et utilisation simples d'une VM CentOS

## 4. Configuration réseau d'une machine CentOS

### utilisez une commande pour prouver que vous avez internet depuis la VM

Pour vérifier que l'on a accès à internet depuis la VM on peut utiliser `curl -sl www.google.com` (par exemple). On recuperera le fichier HTML si l'on est bien connecté à internet.

### prouvez que votre PC hôte et la VM peuvent communiquer

Pour Prouver que les machines peuvent communiquer il faut `ping` l'IP notre VM depuis notre PC et inversement. 

### affichez votre table de routage sur la VM et expliquez chacune des lignes

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

*la ligne qui leur permet de se connecter est  ????

### depuis la VM utilisez curl (ou wget) pour télécharger un fichier sur internet

`curl -t` suivi de l'URL à télécharger 
surl -SLO?

### depuis la VM utilisez dig pour connaître l'IP de :

Pour utiliser Dig il faut le télécharger avant, j'ai utlisé `sudo yum install bind-utils`

*`dig ynov.com`
*`dig google.com`

# II. Notion de ports et SSH

## 1. Exploration des ports locaux

### utilisez la commande ss pour lister les ports TCP sur lesquels la machine virtuelle écoute

## 2. SSH 

![screen_putty](putty.png)
  
