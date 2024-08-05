
## Administer Virtual Networking

### Module Introduction

L'administration du réseau virtuel dans Azure couvre la configuration et la gestion des réseaux virtuels, des adresses IP, des groupes de sécurité et des services DNS. Ce module vise à vous familiariser avec les concepts et les outils nécessaires pour configurer et sécuriser les réseaux virtuels dans Azure.

### Creating and configuring virtual networks

La création et la configuration des réseaux virtuels (VNets) sont essentielles pour organiser et sécuriser les ressources Azure :
- **Création de VNets** : Définir les réseaux virtuels, y compris les adresses IP et les sous-réseaux.
- **Configuration des sous-réseaux** : Diviser les VNets en sous-réseaux pour segmenter et isoler les ressources.
- **Peering de réseaux virtuels** : Connecter différents VNets pour permettre la communication entre eux sans utiliser de passerelles Internet.

### Private and Public IP addresses

Azure utilise des adresses IP publiques et privées pour la communication réseau :
- **Adresses IP privées** : Utilisées pour la communication interne au sein des VNets.
- **Adresses IP publiques** : Utilisées pour l'accès externe aux ressources Azure.
- **Attribution d'adresses IP** : Statique (fixe) ou dynamique (attribuée automatiquement).
- **Configuration des IP** : Assigner et gérer les adresses IP pour les machines virtuelles et autres ressources.

### Network Security Groups

Les Network Security Groups (NSG) contrôlent le trafic réseau vers et depuis les ressources Azure :
- **Règles NSG** : Définir des règles de sécurité pour autoriser ou bloquer le trafic entrant et sortant.
- **Application des NSG** : Assigner des NSG aux sous-réseaux et interfaces réseau des machines virtuelles.
- **Gestion des règles NSG** : Créer, modifier et supprimer des règles pour adapter la sécurité réseau aux besoins de l'organisation.

### Application Security Groups

Les Application Security Groups (ASG) simplifient la gestion de la sécurité des applications :
- **Groupement des ressources** : Regrouper des machines virtuelles et autres ressources ayant des exigences de sécurité similaires.
- **Simplification des règles NSG** : Utiliser les ASG pour appliquer des règles de sécurité de manière logique plutôt qu'au niveau de chaque ressource individuelle.

### Azure DNS

Azure DNS est un service de gestion des noms de domaine qui permet de gérer et de résoudre les noms DNS dans Azure :
- **Zones DNS** : Créer et gérer des zones DNS pour héberger les enregistrements DNS de vos domaines.
- **Enregistrements DNS** : Ajouter, modifier et supprimer des enregistrements DNS tels que A, CNAME, MX, et TXT.
- **Résolution DNS** : Utiliser Azure DNS pour résoudre les noms de domaine internes et externes de manière efficace.

### Private DNS Zones

Les zones DNS privées permettent la résolution de noms DNS au sein des réseaux virtuels sans exposer les noms DNS sur Internet :
- **Création de zones privées** : Définir des zones DNS privées pour les VNets.
- **Résolution DNS privée** : Configurer des résolveurs DNS pour les réseaux virtuels afin de permettre la résolution de noms DNS privés.
- **Gestion des enregistrements** : Ajouter et gérer des enregistrements DNS au sein des zones DNS privées pour les ressources internes.
