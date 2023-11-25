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