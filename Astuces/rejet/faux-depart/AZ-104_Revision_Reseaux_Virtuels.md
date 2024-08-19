
# Révision pour la certification AZ-104 : Configurer et gérer les réseaux virtuels

## Configurer des réseaux virtuels

### Créer et configurer des réseaux virtuels et des sous-réseaux
- **Réseaux virtuels (VNet)** : Représentent votre réseau dans le cloud. Ils permettent de relier des VNets entre eux, d'établir des connexions sécurisées entre les VM et de créer des connexions privées entre les VM et d'autres services Azure.
- **Espace d'adressage** : Géré à l'aide du bloc CIDR, avec des adresses privées et publiques spécifiées lors de la création d'un VNet.
- **Sous-réseaux** : Segmentation des adresses pour les différentes charges de travail, amélioration de l'allocation des adresses IP.

### Créer et configurer le peering de réseaux virtuels
- **Peering VNet** : Permet la connexion de VNets dans la même région ou dans des régions différentes, facilitant la communication privée entre eux.

### Configurer des adresses IP privées et publiques
- **Adresses IP privées** : Utilisées pour les communications internes au sein du VNet.
- **Adresses IP publiques** : Utilisées pour les communications externes, comme l'accès à Internet.

### Configurer des routes réseau définies par l'utilisateur
- **Routes définies par l'utilisateur (UDR)** : Permettent de contrôler la manière dont le trafic est dirigé au sein d'un réseau virtuel.

### Configurer Azure DNS
- **Azure DNS** : Service DNS pour gérer les noms de domaine et résoudre les noms de domaine pour les services Azure.

## Configurer un accès sécurisé aux réseaux virtuels

### Créer et configurer des groupes de sécurité réseau (NSG) et des groupes de sécurité d'application (ASG)
- **NSG** : Applique des règles de sécurité au niveau du sous-réseau ou de la machine virtuelle.
- **ASG** : Permet de regrouper des machines virtuelles pour appliquer des règles de sécurité à l'échelle du groupe.

### Évaluer les règles de sécurité effectives
- **Évaluation des règles de sécurité** : Important pour s'assurer que les règles répondent aux besoins de l'organisation tout en protégeant les ressources.

### Implémenter Azure Bastion
- **Azure Bastion** : Service PaaS pour offrir une connectivité RDP/SSH sécurisée aux VM sans avoir besoin de VPN ou d'exposer les VM à Internet.

### Configurer les points de terminaison de service et les points de terminaison privés
- **Points de terminaison de service** : Sécurisent les ressources Azure en limitant l'accès à partir de réseaux virtuels spécifiques.
- **Points de terminaison privés** : Connectent de manière privée les services Azure à votre VNet via une adresse IP privée.

## Configurer le load balancing

### Configurer Azure Application Gateway
- **Azure Application Gateway** : Un service de passerelle d'application web offrant des fonctionnalités d'équilibrage de charge au niveau 7 (HTTP/HTTPS).

### Configurer un load balancer interne ou public
- **Azure Load Balancer** : Un service d'équilibrage de charge au niveau 4 pour répartir le trafic réseau entre plusieurs instances de l'application.
  - **Load balancer public** : Exposé à Internet, avec une adresse IP publique.
  - **Load balancer interne** : Non exposé à Internet, avec une adresse IP privée.

### Résoudre les problèmes de load balancing
- **Surveillance des sondes de santé** : Assurer que les serveurs backend peuvent traiter les demandes et que les règles d'équilibrage de charge sont configurées correctement.

## Surveiller le réseau virtuel

### Surveiller la connectivité sur site
- **Surveillance de la connectivité** : Vérifier la connectivité entre les réseaux sur site et Azure, et s'assurer de la bonne configuration des connexions VPN et du peering VNet.

### Configurer et utiliser Azure Monitor pour les réseaux
- **Azure Monitor** : Outil pour surveiller la performance et la disponibilité des réseaux virtuels en collectant des métriques et des journaux.

### Utiliser Azure Network Watcher
- **Azure Network Watcher** : Fournit des outils de diagnostic et de surveillance pour les réseaux virtuels Azure, y compris l'analyse du trafic et la résolution des problèmes de configuration.

### Résoudre les problèmes de réseau externe et de connectivité réseau virtuel
- **Résolution des problèmes de connectivité** : Inclut la surveillance de la connectivité entre les réseaux sur site et Azure, ainsi que la résolution des problèmes liés aux VPN, au peering de réseaux virtuels, et aux points de terminaison de service.

