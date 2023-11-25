# Partie VM VirtualBox

# Les problemes renceontres 
## Guest Addition installation problem
Manually Mount Guest Additions:
If the automatic insertion doesn't work, you can try manually mounting the Guest Additions ISO.
1.	In the VirtualBox Manager, select your virtual machine.
2.	Click on "Settings."
3.	Go to the "System" tab.
4.	In the "Motherboard" tab, make sure "Floppy" is not checked.
5.	Click "OK" to save the settings.
6.	Start your virtual machine.
Now, try manually inserting the Guest Additions ISO:
•	In the running virtual machine window, go to the menu and select "Devices" > "Optical Drives" > "Choose a disk file."
•	Navigate to the location where you have the Guest Additions ISO and select it.
## Shared folder windows 7 
. Run Installer as Administrator:
•	Right-click on the VBoxWindowsAdditions-amd64.exe (or the appropriate version for your system) installer.
•	Choose "Run as administrator."
 ## Shared folder windows 7 

```Sudo adduser vboxuser vboxsf```

### Add user with all privileges
```
Su 
Apt install sudo 
Usermod -aG sudo user-name
```
# Configuration of vitual machine 
## ubuntu installation
![Installation](img/installation.png =100x20)
![Installation2](img/installation2.png)
![Installation2](img/configuration1.png)
![Installation2](img/configurationHardDrive.png)
![Installation2](img/finishInstallation2.png)
## windows 7 installation
![InstallationWindows7](img/windowsConf1.png)
![InstallationWindows7](img/windowsConf2.png)
![InstallationWindows7](img/windowsConf3.png)
![InstallationWindows7](img/windowsConf4.png)
## widows 7 clone
![InstallationWindows7](img/windows7Clone.png)
![InstallationWindows7](img/windowsCloneFinish.png)
![InstallationWindows7](img/windows7Cloning.png)

## shared file ubuntu
![InstallationWindows7](img/3.1.png)
![InstallationWindows7](img/3.2.png)
![InstallationWindows7](img/3.3.png)
![InstallationWindows7](img/3.4.png)
![InstallationWindows7](img/3.5.png)
![InstallationWindows7](img/3.6.png)
![InstallationWindows7](img/3.8.png)
![InstallationWindows7](img/3.9.png)
![InstallationWindows7](img/3.10.png)
## shred file windows 7
![InstallationWindows7](img/3.11.png)
![InstallationWindows7](img/3.12.png)
![InstallationWindows7](img/3.13.png)
![InstallationWindows7](img/3.14.png)
![InstallationWindows7](img/3.15.png)
![InstallationWindows7](img/3.16.png)
![InstallationWindows7](img/3.17.png)
![InstallationWindows7](img/3.18.png)
![InstallationWindows7](img/3.19.png)
![InstallationWindows7](img/3.20.png)
![InstallationWindows7](img/3.21.png)


## share periphirique
![InstallationWindows7](img/bidirectionnalDragAndDrop.png)
![InstallationWindows7](img/sharedPeripherique.png)
![InstallationWindows7](img/addUSB.png)

## Take and restore snapshot
![InstallationWindows7](img/takeSnapshot.png)
![InstallationWindows7](img/restore_snapshot.png)
## 6. Mettre les VMs dans un réseau privé (Host-Only) :
### − Utiliser le serveur DHCP virtuel pour attribuer des adresses IP aux VMs
![InstallationWindows7](img/6.1.1.png)
![InstallationWindows7](img/6.1.2.png)
## Vérifier les adresses IP attribuées aux VMs.
![InstallationWindows7](img/6.2.png)
![InstallationWindows7](img/6.2.2.png)
## Mettre l’hôte sur le même sous réseau que les VMs (vous pouvez utiliser un adressage statique pour mettre les VMs et l’hôte sur le même sous réseau).
![InstallationWindows7](img/6.3.1.png)
![InstallationWindows7](img/6.3.2.png)
![InstallationWindows7](img/6.3.3.png)
![InstallationWindows7](img/6.3.4.png)
## Tester la communication/connexion inter VMs et entre les VMs et l’hôte (n’oubliez pas de désactiver le pare-feu).
![InstallationWindows7](img/6.4.1.png)
![InstallationWindows7](img/6.4.2.png)
![InstallationWindows7](img/6.4.3.png)
![InstallationWindows7](img/6.4.4.png)
![InstallationWindows7](img/6.4.5.png)
![InstallationWindows7](img/6.4.6.png)
# 7. Mettre les VMs sur le mode de réseau virtuel NAT (NAT pour VMware Workstation et réseau NAT pour Oracle VM VirtualBox).
## − Utiliser le serveur DHCP virtuel pour attribuer des adresses IP aux VMs.
![InstallationWindows7](img/7.1.png)
## − Vérifier les adresses IP attribuées aux VMs ainsi que la passerelle par défaut.
![InstallationWindows7](img/7.2.png)
## − Connecter l’hôte à internet (vous pouvez utiliser le partage Internet entre vos smartphones et l’hôte).
![InstallationWindows7](img/7.3.1.png)
![InstallationWindows7](img/7.3.2.png)
## − Tester la communication inter VMs, entre les VMs et l’hôte et l’accès des VMs à Internet.
![InstallationWindows7](img/7.4.1.png)
![InstallationWindows7](img/7.4.2.png)
![InstallationWindows7](img/7.4.3.png)
## − Créer et tester une règle de redirection de port (Port Forwarding).
![InstallationWindows7](img/7.5.4.png)
![InstallationWindows7](img/7.5.5.png)
![InstallationWindows7](img/7.5.1.png)
![InstallationWindows7](img/7.5.2.png)
![InstallationWindows7](img/7.5.3.png)




# 8. Mettre les VMs sur le mode de réseau virtuel Bridged.
## − Utiliser le serveur DHCP externe pour attribuer des adresses IP à l’hôte et aux VMs (vous pouvez utiliser le serveur DHCP de vos smartphones).
![InstallationWindows7](img/8.1.png)
## Utiliser le mode automatique pour la connexion directe avec le réseau externe (bridged to), sinon choisir l’interface réseau physique de l’hôte connectée au réseau externe.
![InstallationWindows7](img/8.2.png)


## − Vérifier les adresses IP attribuées à l’hôte et aux VMs ainsi que la passerelle par défaut (li faut s’assurer que l’hôte et les VMs se trouvent dans le même sous réseau)

![InstallationWindows7](img/8.3.png)
## − Vérifier que l’hôte est connecté à Internet
![InstallationWindows7](img/8.5.png)
## Tester la communication inter VMs, entre les VMs et l’hôte et l’accès des VMs à Internet.
![InstallationWindows7](img/8.4.png)


# 9. Mettre les deux VMs sur deux modes de réseau virtuel différents (une VM sur le mode Host-Only et l’autre sur le mode réseau NAT).
![InstallationWindows7](img/9.0.1.png)
![InstallationWindows7](img/9.0.2.png)
## Désactiver le serveur DHCP virtuel pour les deux modes.
![InstallationWindows7](img/9.1.png)
![InstallationWindows7](img/9.2.png)
![InstallationWindows7](img/9.3.png)
![InstallationWindows7](img/9.5.png)
![InstallationWindows7](img/9.6.png)
![InstallationWindows7](img/9.7.png)





# **Partie VMware**

# Créer une duplication (clone) de l’état actuel de la VM Windows 7 (full réplication).

<center>
<div style="text-align:center;"></div>
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled.png" alt="Untitled" width="70%">
</div>

> Une nouvelle machine clone a été créée.


<br>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%201.png" alt="Untitled" width="30%">
</div>

<br>
<br>
<br>
<br>
<br>

# Configurer un partage de fichiers entre la VM et l'hôte.


> - On doit d’abord aller vers les parametre de machine viruelle → options → Shared Folder  et le modifier vers “Always enabled” et ajouter le chemain du dossier dans la machine host
>- On doit installer Vmware Tools pour qu’on puisse faire le partage entre la machine host et guest.
>- On peut voire que le fichier est bien partage entre la machine host et guest.



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%202.png" alt="Untitled" width="70%">
</div>


<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%203.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%204.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%205.png" alt="Untitled" width="70%">
</div>

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

# Configurer un partage des périphériques entre la VM et l'hôte.


> On ajoute un nouveau périphériques. et on notice que l’on peut voire sur la machine host et guest



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%206.png" alt="Untitled" width="70%">
</div>

# Créer et restaurer une image instantanée (snapshot) pour la VM Windows 7.


 > Pour prendre une snapshot dans vmware , on clique sur VM → Snapshot → Take Snapshot



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%207.png" alt="Untitled" width="90%">
</div>


 > Pour restaurer un snaphshot on clique sur : revert to Snapshot : Snapshot windows 7 , et on va voire qu’on a reviendrai dans la meme etat et la position ou on a creee le snapshot


<br>
<br>
<br>

# Mettre les VMs dans un réseau privé (Host-Only) :

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%208.png" alt="Untitled" width="100%">
</div>


 > l’intervalle de reseau et de 192.168.157.128 → 192.168.157.254



### Ip address pour Windows 7 et Ubuntu

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%209.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2010.png" alt="Untitled" width="70%">
</div>


192.168.221.3

<br>
<br>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2011.png" alt="Untitled" width="70%">
</div>

192.168.221.4

> toutes le machine sont dans le meme reseau

> On teste la connectivite

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2012.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2013.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2014.png" alt="Untitled" width="70%">
</div>





# Mettre les VMs sur le mode de réseau virtuel NAT

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2015.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2016.png" alt="Untitled" width="70%">
</div>

192.168.26.128

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2017.png" alt="Untitled" width="70%">
</div>

192.168.26.129

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2018.png" alt="Untitled" width="70%">
</div>

>ping de les vm vers l’hote

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2019.png" alt="Untitled" width="70%">
</div>

>acceder vers l’internet a partir les vms

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2020.png" alt="Untitled" width="70%">
</div>

## Port forwarding

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2021.png" alt="Untitled" width="60%">
</div>


 >on peut acceder vers le server apache a travers notre host



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2022.png" alt="Untitled" width="70%">
</div>


# 8. Mettre les VMs sur le mode de réseau virtuel Bridged.

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2023.png" alt="Untitled" width="70%">
</div>

## L’attribution des addresses IPHost

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2024.png" alt="Untitled" width="70%">
</div>

Ubuntu→ 192.168.34.211

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2025.png" alt="Untitled" width="70%">
</div>

Windows7 → 192.168.34.45

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2026.png" alt="Untitled" width="70%">
</div>
                                                                Host → 192.168.34.99


 >Toutes les machine sont dans le meme sous reseau , et la machine host est connecte a l’internet (on peut pinger 8.8.8.8)
Le pasrelle par default est : 192.168.34.215



## Teste de connectivite entre les machines

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2027.png" alt="Untitled" width="70%">
</div>

>ping ubuntu vers windows7

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2028.png" alt="Untitled" width="70%">
</div>

>ping windows7 vers ubuntu

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2029.png" alt="Untitled" width="70%">
</div>


>ping windows ver ubuntu et windows7

## Teste de connectivite vers l’internet

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2030.png" alt="Untitled" width="70%">
</div>

>Windows7 peut connecter a l’internet

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2031.png" alt="Untitled" width="70%">
</div>

>Ubuntu peut connecter a l’internet

# 9. Mettre les deux VMs sur deux modes de réseau virtuel différents (une VM sur le Nat et autre sur Host-Only)


 >Le server DHCP est desactive dans les deux vm
Windows7 → NAT
Ubuntu → Host-Only



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2032.png" alt="Untitled" width="70%">
</div>


 >On va attribuer un ip static pour chacune des machines virtuelles



<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2033.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2034.png" alt="Untitled" width="70%">
</div>

ip ubuntu : 192.168.1.21

ip windows7 : 192.168.1.20


<div style="text-align:center;">
  <img src="Cloud%20virtualisation%200df1c723f6554204aac3fdc12b061b18/Untitled%2035.png" alt="Untitled" width="70%">
</div>

> On peut pas faire une connection entre  le windows et ubuntu