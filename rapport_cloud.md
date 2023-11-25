# Rapport

### Allouache Ayhem  Grp02| ISI
### Satoutah Haithem Grp01| ISI

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


# VMware

# Définition 
VMware est une entreprise spécialisée dans la virtualisation et les solutions de cloud computing. La virtualisation VMware permet de créer des machines virtuelles sur un même matériel physique, permettant ainsi d'exécuter plusieurs systèmes d'exploitation simultanément.

# Histoire
 VMware a été fondée en 1998. Son produit phare, VMware Workstation, a été lancé en 1999. Depuis, la société a développé plusieurs produits de virtualisation, notamment VMware ESXi (un hyperviseur), VMware vSphere (une suite de virtualisation de serveurs), et d'autres solutions liées au cloud computing.

# Fonctionnalités
 Les fonctionnalités de VMware dépendent du produit spécifique, mais en général, elles incluent la migration à chaud des machines virtuelles, la gestion centralisée des ressources, la création de clones de machines virtuelles, la sauvegarde et la restauration rapides, ainsi que des fonctionnalités de sécurité avancées.

# Utilisations
 VMware est largement utilisé dans les entreprises pour la consolidation des serveurs, la gestion de data centers, la création d'environnements de tests et de développement, la fourniture de bureaux virtuels (VDI), et la mise en place de solutions de cloud computing.


# VirtualBox

# Définition
 VirtualBox est un logiciel de virtualisation open source développé par Oracle. Il permet aux utilisateurs de créer et de gérer des machines virtuelles sur leurs ordinateurs.

# Histoire
 VirtualBox a été initialement développé par la société allemande Innotek, qui a été rachetée par Sun Microsystems en 2008. Oracle a acquis Sun Microsystems en 2010, et depuis lors, VirtualBox est maintenu par Oracle.

# Fonctionnalités
 VirtualBox offre des fonctionnalités telles que la prise en charge de divers systèmes d'exploitation invités, la possibilité de créer des instantanés (snapshots) pour revenir à un état antérieur, la prise en charge de l'accélération matérielle, la gestion de réseau avancée, et une interface utilisateur conviviale.

# Utilisations
 VirtualBox est couramment utilisé pour des besoins de développement, de tests, d'éducation et d'expérimentation. Il est également populaire chez les utilisateurs individuels qui souhaitent exécuter plusieurs systèmes d'exploitation sur une seule machine physique, par exemple, pour tester des logiciels dans différents environnements.

# Tableau comparatif entre Vmware et Virtual Box

| Critères | VMware | VirtualBox |
| --- | --- | --- |
| Types de Virtualisation | Hyperviseur de Type 1 (bare-metal) et Type 2 (hosted) | Hyperviseur de Type 2 (hosted) |
| OS Supportés | Large support pour les systèmes d'exploitation invités, y compris Windows, Linux, macOS, et d'autres | Support étendu pour divers OS, y compris Windows, Linux, macOS, Solaris, etc. |
| Migration de VM | Migration à chaud des machines virtuelles via vMotion dans les solutions professionnelles comme VMware vSphere | Possibilité de déplacer des machines virtuelles en utilisant des fonctionnalités telles que "Clone" et "Export" |
| Sécurité | Offre des fonctionnalités avancées de sécurité, y compris le chiffrement des disques virtuels, l'authentification à deux facteurs, et la gestion des accès | Moins axé sur les fonctionnalités de sécurité avancées, convient davantage à un usage personnel ou de développement |
| Performances | Performances élevées, surtout dans des environnements professionnels avec des solutions telles que VMware ESXi | Bonnes performances pour des besoins individuels, mais peut être moins optimisé pour des environnements à grande échelle |
| Gestion des Ressources | Gestion avancée des ressources avec des fonctionnalités telles que DRS (Distributed Resource Scheduler) pour une répartition dynamique des charges de travail | Gestion des ressources adaptée aux besoins individuels, mais moins robuste que les solutions professionnelles de VMware |
| Communauté et Support | Forte communauté et support professionnel disponible avec une gamme de produits variés | Communauté active, mais le support professionnel est limité par rapport à VMware |
| Coût | Souvent considéré comme plus onéreux, surtout pour les solutions professionnelles | Gratuit en tant que logiciel open source, avec des options d'extension pour un support commercial |
| Convivialité | Interfaces utilisateur conviviales et bien développées, adaptées aux utilisateurs professionnels | Interface utilisateur conviviale, idéale pour les utilisateurs individuels et les petites entreprises |