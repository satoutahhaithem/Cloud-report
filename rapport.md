# Partie VM VirtualBox
<<<<<<< HEAD
## Definition de la machine virtuellle : 
Une machine virtuelle (VM), en informatique, est une émulation logicielle d'un ordinateur physique. Elle permet à un seul ordinateur physique (appelé hôte) d'exécuter plusieurs systèmes d'exploitation simultanément. Chaque machine virtuelle fonctionne comme un ordinateur autonome avec son propre système d'exploitation (invité) et ses applications, mais elle partage les ressources matérielles de l'hôte, telles que le processeur, la mémoire et le stockage.

L'utilisation de machines virtuelles offre plusieurs avantages, notamment l'isolation des environnements, la consolidation des ressources, la facilité de gestion, la migration des applications entre différentes plates-formes, et la possibilité de tester des logiciels dans des environnements contrôlés. Les hyperviseurs (ou moniteurs de machines virtuelles) sont des logiciels ou des matériels qui permettent de créer et de gérer ces machines virtuelles sur l'hôte physique.

En résumé, une machine virtuelle est une instance logicielle d'un ordinateur qui fonctionne de manière indépendante sur un serveur physique, permettant ainsi l'exécution de plusieurs systèmes d'exploitation et applications sur une seule machine physique.

## Hyperviseur 
Un hyperviseur, également appelé moniteur de machines virtuelles, est un logiciel ou un matériel qui permet la création et la gestion de machines virtuelles sur un serveur physique. Il existe deux types d'hyperviseurs :

### Hyperviseur de type 1 (ou natif) :
Il s'exécute directement sur le matériel physique et n'a pas besoin d'un système d'exploitation hôte. Il a un accès direct aux ressources matérielles, offrant ainsi des performances généralement meilleures. Exemples : VMware ESXi, Microsoft Hyper-V.

### Hyperviseur de type 2 (ou hébergé) : 
Il s'exécute comme une application sur un système d'exploitation hôte. Il utilise les ressources du système d'exploitation sous-jacent pour créer et gérer des machines virtuelles. Exemples : VMware Workstation, Oracle VirtualBox.
## Emulateur :
Un émulateur est un logiciel ou un matériel qui permet à un système informatique (l'hôte) de reproduire le comportement d'un autre système informatique (l'invité) de manière à pouvoir exécuter des logiciels conçus pour cet autre système. Les émulateurs sont souvent utilisés pour exécuter des programmes conçus pour une architecture matérielle ou un système d'exploitation différent.
## Comparaison entre Hyperviseur et Emulateur :
### Niveau d'isolation :
Les hyperviseurs créent des machines virtuelles qui partagent les ressources physiques mais fonctionnent de manière isolée les unes par rapport aux autres.
Les émulateurs émulent complètement le matériel, permettant l'exécution d'un système d'exploitation différent, mais généralement avec une performance moindre.
### Performance 
Les hyperviseurs, en particulier de type 1, ont généralement de meilleures performances car ils ont un accès direct aux ressources matérielles.
Les émulateurs peuvent être plus lents car ils doivent émuler complètement le matériel, ce qui peut entraîner une surcharge.
### Utilisation :
Les hyperviseurs sont couramment utilisés dans la virtualisation de serveurs et de data centers.
Les émulateurs sont souvent utilisés pour exécuter des applications conçues pour des plates-formes différentes (par exemple, exécuter des jeux conçus pour une console sur un PC).
### Exemple d'application :
Les hyperviseurs sont utilisés pour la virtualisation de machines et la gestion des ressources dans des environnements professionnels.
Les émulateurs sont utilisés pour exécuter des jeux vidéo, des anciens systèmes d'exploitation, ou des applications spécifiques.
En résumé, les hyperviseurs sont principalement utilisés pour la virtualisation de machines, tandis que les émulateurs sont utilisés pour exécuter des logiciels conçus pour d'autres systèmes ou architectures matérielles.

# Some possible problem 
=======

# Les problemes renceontres 
>>>>>>> 4f685ba0b7e8f5bd98c41f2100d18aa3ab9ecfa3
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
<div style="text-align:center;">
  <img src="img/installation.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/installation2.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/configuration1.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/configurationHardDrive.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/finishInstallation2.png" alt="Untitled" width="70%">
</div>

## windows 7 installation
<div style="text-align:center;">
  <img src="img/windowsConf1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/windowsConf2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/windowsConf3.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/windowsConf4.png" alt="Untitled" width="70%">
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
<br>
<br>
<br>
<br>
<br>
<br>


## widows 7 clone
<div style="text-align:center;">
  <img src="img/windows7Clone.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/windowsCloneFinish.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/windows7Cloning.png" alt="Untitled" width="70%">
</div>


## shared file ubuntu

> - we need to click on Devices on the top menu of the virtual machine 
> - then we click to shared folder setting 
> - after click on the + on the right 
> - we configure the path on the host 
> - check auto-mount and make it permanent 
> - make the vboxuser suder user 
> - also we nedd to to add the user as vboxsf

<div style="text-align:center;">
  <img src="img/3.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.3.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.4.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.5.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.6.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.8.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.9.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.10.png" alt="Untitled" width="70%">
</div>

## shred file windows 7
> - Install vbox guest addition 
> - Turn on network discovery
> - configure shared folder setting ( shared folder path on host machine and make it permanent and auto-mount)
<div style="text-align:center;">
  <img src="img/3.11.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.12.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.13.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.14.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.15.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.16.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.17.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.18.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.19.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.20.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/3.21.png" alt="Untitled" width="70%">
</div>



## share periphirique
> - insert the guest addition cd image 
> - enable bidirectionnal drag and drop
> - enable usb controller and select it 
<div style="text-align:center;">
  <img src="img/bidirectionnalDragAndDrop.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/sharedPeripherique.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/$1.pngimg/addUSB.png" alt="Untitled" width="70%">
</div>


## Take and restore snapshot
> - Go to machine and click to take snapshot
> - to restore click on vm and select snapshor after click to restore snapshot
<div style="text-align:center;">
  <img src="img/takeSnapshot.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/restore_snapshot.png" alt="Untitled" width="70%">
</div>

## 6. Mettre les VMs dans un réseau privé (Host-Only) :
### − Utiliser le serveur DHCP virtuel pour attribuer des adresses IP aux VMs
> -  Go to tool after host only networks 
> -  configure adapter manually 
> - enable dhcp server and give it range of values²
<div style="text-align:center;">
  <img src="img/6.1.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.1.2.png" alt="Untitled" width="70%">
</div>

## Vérifier les adresses IP attribuées aux VMs.
<div style="text-align:center;">
  <img src="img/6.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.2.2.png" alt="Untitled" width="70%">
</div>

## Mettre l’hôte sur le même sous réseau que les VMs (vous pouvez utiliser un adressage statique pour mettre les VMs et l’hôte sur le même sous réseau).
<div style="text-align:center;">
  <img src="img/6.3.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.3.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.3.3.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.3.4.png" alt="Untitled" width="70%">
</div>

## Tester la communication/connexion inter VMs et entre les VMs et l’hôte (n’oubliez pas de désactiver le pare-feu).

> - we can ping between all the vms and host becasue we are under the same network
<div style="text-align:center;">
  <img src="img/6.4.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.4.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.4.3.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.4.4.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.4.5.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/6.4.6.png" alt="Untitled" width="70%">
</div>

# 7. Mettre les VMs sur le mode de réseau virtuel NAT (NAT pour VMware Workstation et réseau NAT pour Oracle VM VirtualBox).
## − Utiliser le serveur DHCP virtuel pour attribuer des adresses IP aux VMs.
> - enable the dhcp server
<div style="text-align:center;">
  <img src="img/7.1.png" alt="Untitled" width="70%">
</div>

## − Vérifier les adresses IP attribuées aux VMs ainsi que la passerelle par défaut.

<div style="text-align:center;">
  <img src="img/7.2.png" alt="Untitled" width="70%">
</div>

## − Connecter l’hôte à internet (vous pouvez utiliser le partage Internet entre vos smartphones et l’hôte).
<div style="text-align:center;">
  <img src="img/7.3.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/7.3.2.png" alt="Untitled" width="70%">
</div>

## − Tester la communication inter VMs, entre les VMs et l’hôte et l’accès des VMs à Internet.
> - we can ping normally
<div style="text-align:center;">
  <img src="img/7.4.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/7.4.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/7.4.3.png" alt="Untitled" width="70%">
</div>

## − Créer et tester une règle de redirection de port (Port Forwarding).
> - install the apache server with the command 
```
sudo apt-get install apache2
```
> - lunch the server with the commmand 
```
sudo systemctl status apache2
```
<div style="text-align:center;">
  <img src="img/7.5.5.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/7.5.4.png" alt="Untitled" width="70%">
</div>

> - define the regle of port forwarding on the configuration

<div style="text-align:center;">
  <img src="img/7.5.1.png" alt="Untitled" width="70%">
</div>

> - test apache on the vm 

<div style="text-align:center;">
  <img src="img/7.5.2.png" alt="Untitled" width="70%">
</div>

> - use the port defined on the rule of port forwarding 8080 on the host machine 
<div style="text-align:center;">
  <img src="img/7.5.3.png" alt="Untitled" width="70%">
</div>





# 8. Mettre les VMs sur le mode de réseau virtuel Bridged.
## − Utiliser le serveur DHCP externe pour attribuer des adresses IP à l’hôte et aux VMs (vous pouvez utiliser le serveur DHCP de vos smartphones).
<div style="text-align:center;">
  <img src="img/8.1.png" alt="Untitled" width="70%">
</div>

## Utiliser le mode automatique pour la connexion directe avec le réseau externe (bridged to), sinon choisir l’interface réseau physique de l’hôte connectée au réseau externe.
<div style="text-align:center;">
  <img src="img/8.3.png" alt="Untitled" width="70%">
</div>



## − Vérifier les adresses IP attribuées à l’hôte et aux VMs ainsi que la passerelle par défaut (li faut s’assurer que l’hôte et les VMs se trouvent dans le même sous réseau)

<div style="text-align:center;">
  <img src="img/8.4.png" alt="Untitled" width="70%">
</div>

## − Vérifier que l’hôte est connecté à Internet
<div style="text-align:center;">
  <img src="img/8.5.png" alt="Untitled" width="70%">
</div>

## Tester la communication inter VMs, entre les VMs et l’hôte et l’accès des VMs à Internet.
> - ping work between all machines
<div style="text-align:center;">
  <img src="img/8.6.1.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/8.6.2.png" alt="Untitled" width="70%">
</div>
<div style="text-align:center;">
  <img src="img/8.6.3.png" alt="Untitled" width="70%">
</div>



# 9. Mettre les deux VMs sur deux modes de réseau virtuel différents (une VM sur le mode Host-Only et l’autre sur le mode réseau NAT).
<div style="text-align:center;">
  <img src="img/9.0.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/9.0.2.png" alt="Untitled" width="70%">
</div>

## Désactiver le serveur DHCP virtuel pour les deux modes.
<div style="text-align:center;">
  <img src="img/9.1.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/9.2.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/9.3.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/9.5.png" alt="Untitled" width="70%">
</div>

> - we can't ping on this case 
<div style="text-align:center;">
  <img src="img/9.6.png" alt="Untitled" width="70%">
</div>

<div style="text-align:center;">
  <img src="img/9.7.png" alt="Untitled" width="70%">
</div>






