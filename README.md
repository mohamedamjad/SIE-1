# TP Sécurité

## Consignes
-Trouver 3 vulnérabilités sur metasploitable
-Expliquer la vulnérabilité
-Corriger la vulnérabilité

## Premier vulnérabilité

### IRC

![image](SIE/images/irc.png)
#### Constat
La vulnérabilité exploite un backdoor dans le code de l’archive Unreal IRCD, ce backdoor était présent dans l’archive du code entre novembre 2009 et Juin 2010.
#### Lien du CVE
[cve link](https://www.rapid7.com/db/modules/exploit/unix/irc/unreal_ircd_3281_backdoor)
#### Solution : Mettre à jour
Pour corriger, il faut mettre à jour la version du package unreal ircd mais on ne peut pas tester car la machine de metasploitable ne peut pas télécharger des packages.
Pour palier à ce problème, il faut télécharger sur notre machine local le package Unreal ircd et l'enlever par scp sur la machine metasploitable.
Les commandes à suivre :
-./Config
-make
-make install                
![image]()
## Deuxieme vulnérabilité

### VSFTPD
![image]()
#### Constat
La vulnérabilité exploite un backdoor dans le code de l'archive de vsftpd dans la vision 2.3.4.
#### Lien du CVE
[cve link](https://www.rapid7.com/db/modules/exploit/unix/ftp/vsftpd_234_backdoor)
#### Solution : Mettre à jour
[installation](http://www.thegeekstuff.com/2010/11/vsftpd-setup/)
Pour corriger, il faut mettre à jour la version du package vsftpd, même erreur que précédent.
Il faut envoyer par scp le package.
![image]()

## Troisieme vulnérabilité

### APACHE

#### Constat

#### Lien du CVE
[cve link](https://www.rapid7.com/db/modules/exploit/multi/http/apache_mod_cgi_bash_env_exec)
#### Solution :
