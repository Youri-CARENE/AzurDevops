
## Administer Azure Virtual Machines

### Module Introduction

L'administration des machines virtuelles (VM) Azure couvre la planification, la création, la gestion des tailles et du stockage des VM, la connexion, la configuration de la haute disponibilité et le déploiement de groupes de machines virtuelles identiques (scale sets). Ce module vous guidera à travers les concepts et les meilleures pratiques pour gérer les VM dans Azure.

### Planning VMs

La planification des machines virtuelles implique la sélection des tailles et des configurations appropriées pour répondre aux besoins de performance et de coût :
- **Choix de la taille** : Sélectionner la taille de la VM en fonction des besoins en CPU, mémoire et stockage.
- **Images** : Utiliser des images préconfigurées ou créer des images personnalisées pour les VM.
- **Réseau** : Configurer les réseaux virtuels, sous-réseaux et groupes de sécurité réseau (NSG).

### Managing VM Sizes

La gestion des tailles de VM permet d'optimiser les performances et les coûts :
- **Redimensionnement** : Modifier la taille des VM en fonction des besoins changeants.
- **Séries de VM** : Comprendre les différentes séries de VM (B, D, E, F, etc.) et leurs cas d'utilisation.
- **Optimisation des coûts** : Sélectionner les tailles de VM qui offrent le meilleur rapport coût/performance pour les charges de travail spécifiques.

### Virtual Machine Storage

Le stockage des VM Azure inclut la gestion des disques et des options de stockage disponibles :
- **Disques gérés** : Utilisation des disques gérés pour simplifier la gestion et améliorer la disponibilité.
- **Types de disques** : Disques SSD Premium, SSD Standard et HDD Standard.
- **Snapshots et sauvegardes** : Créer des snapshots et configurer des sauvegardes pour protéger les données.

### Creating VMs

La création de machines virtuelles implique plusieurs étapes clés :
- **Portail Azure** : Utiliser le portail Azure pour créer et configurer des VM.
- **Azure CLI / PowerShell** : Automatiser la création de VM avec des scripts Azure CLI ou PowerShell.
- **Modèles ARM** : Utiliser des modèles ARM pour déployer des VM de manière déclarative et cohérente.

### Connecting to VMs

La connexion aux VM Azure peut se faire de différentes manières en fonction du système d'exploitation :
- **Connexion RDP** : Utiliser le protocole RDP pour se connecter aux VM Windows.
- **Connexion SSH** : Utiliser SSH pour se connecter aux VM Linux.
- **Diagnostics et dépannage** : Utiliser les outils de diagnostic pour résoudre les problèmes de connexion.

### Configuring high availability

La configuration de la haute disponibilité assure que les VM restent accessibles même en cas de défaillance :
- **Zones de disponibilité** : Déployer des VM dans des zones de disponibilité différentes pour une haute disponibilité régionale.
- **Ensembles de disponibilité** : Utiliser des ensembles de disponibilité pour répartir les VM sur plusieurs hôtes physiques au sein d'un datacenter.
- **Load Balancer** : Configurer des load balancers pour distribuer le trafic et augmenter la résilience.

### Deploying Virtual Machine Scale Sets

Les Virtual Machine Scale Sets (VMSS) permettent de déployer et gérer un groupe de VM identiques pour gérer les charges de travail à grande échelle :
- **Création de VMSS** : Utiliser le portail Azure, Azure CLI ou des modèles ARM pour déployer des VMSS.
- **Autoscaling** : Configurer des règles d'autoscaling pour ajuster automatiquement le nombre de VM en fonction de la demande.
- **Gestion des mises à jour** : Gérer les mises à jour et les déploiements sans interruption de service.
