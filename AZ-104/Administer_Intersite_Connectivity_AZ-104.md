
## Administer Intersite Connectivity

### Module Introduction

L'administration de la connectivité intersite dans Azure couvre les techniques et les outils pour connecter différents réseaux virtuels et sites. Ce module vous guidera à travers les concepts de connectivité intersite, les peering de réseaux virtuels, les passerelles VPN, et plus encore.

### Intersite connectivity

La connectivité intersite permet de connecter des réseaux virtuels et des sites physiques afin de créer un environnement réseau intégré et sécurisé. Les options de connectivité incluent les peering de réseaux virtuels, les passerelles VPN, et les connexions express.

### Virtual Network Peering

Le peering de réseaux virtuels permet la connexion de deux réseaux virtuels dans la même région ou dans des régions différentes :
- **Connexion de VNets** : Permettre la communication entre VNets sans passer par une passerelle Internet.
- **Transfert de données** : Transfert de données à faible latence et haute bande passante entre VNets.
- **Sécurité et isolation** : Maintien des frontières de sécurité tout en permettant la connectivité.

### VPN Gateway

Les passerelles VPN fournissent des connexions sécurisées entre des réseaux virtuels et des sites locaux ou d'autres réseaux virtuels :
- **Types de VPN** : VPN basés sur les routes (Route-based) et VPN basés sur les politiques (Policy-based).
- **Configuration des passerelles** : Configurer les passerelles VPN pour la connectivité intersite.
- **Sécurité** : Utilisation de protocoles de sécurité tels que IPsec pour sécuriser les connexions VPN.

### Site-to-Site and Point-to-Site

Les connexions Site-to-Site et Point-to-Site permettent une connectivité flexible entre les réseaux :
- **Site-to-Site VPN** : Connexion permanente entre un site local et un réseau virtuel Azure.
- **Point-to-Site VPN** : Connexion VPN pour les utilisateurs individuels à partir de leurs ordinateurs personnels vers un réseau virtuel Azure.
- **Cas d'utilisation** : Scénarios d'utilisation et configuration des deux types de VPN.

### Gateway Transit

Le transit de passerelle permet à un réseau virtuel de se connecter à un autre via une passerelle VPN dans un VNet de transit :
- **Configuration de transit** : Configurer le transit de passerelle pour permettre la connectivité entre VNets via une passerelle partagée.
- **Avantages** : Simplification de la gestion des passerelles et optimisation des coûts de réseau.

### User Defined Routes

Les routes définies par l'utilisateur (UDR) permettent un contrôle plus granulaire du routage du trafic dans Azure :
- **Création de routes** : Définir des routes personnalisées pour contrôler le chemin du trafic réseau.
- **Application des UDR** : Assigner des UDR aux sous-réseaux pour personnaliser le routage.
- **Scénarios d'utilisation** : Utilisation des UDR pour des cas spécifiques tels que l'acheminement du trafic via des appliances virtuelles.

### Service Endpoints

Les points de terminaison de service permettent aux réseaux virtuels de se connecter directement aux services Azure, en contournant l'Internet public :
- **Activation des points de terminaison** : Configurer les points de terminaison de service pour des services Azure spécifiques.
- **Sécurité et performances** : Amélioration de la sécurité et des performances des connexions aux services Azure.
- **Scénarios d'utilisation** : Cas d'utilisation courants des points de terminaison de service pour les bases de données, le stockage, etc.

### Private Endpoint

Les points de terminaison privés permettent aux ressources Azure de se connecter à des services de manière sécurisée via des adresses IP privées :
- **Configuration des points de terminaison privés** : Créer et configurer des points de terminaison privés pour les services Azure.
- **Sécurité et isolation** : Garantir que le trafic reste dans le réseau privé sans exposer les services sur Internet.
- **Scénarios d'utilisation** : Utilisation des points de terminaison privés pour sécuriser l'accès aux services critiques.
