
## Administer Network Traffic

### Module Introduction

L'administration du trafic réseau dans Azure inclut la gestion des solutions de répartition de charge, la configuration des règles de trafic, et la surveillance du réseau. Ce module couvre les principaux composants et outils nécessaires pour gérer efficacement le trafic réseau dans Azure.

### Azure Load Balancer

Azure Load Balancer distribue le trafic réseau entrant vers plusieurs instances de services afin d'assurer une haute disponibilité et une répartition de charge équilibrée :
- **Types de Load Balancer** : Load Balancer public et Load Balancer interne.
- **Fonctionnalités** : Distribution du trafic, surveillance des pools de backend, et redirection de port.
- **Scénarios d'utilisation** : Utilisation du Load Balancer pour les applications web, les services backend, et d'autres ressources.

### Load Balancer Rules

Les règles de Load Balancer définissent comment le trafic entrant est distribué aux instances backend :
- **Configuration des règles** : Définir les règles de trafic basées sur les protocoles, les ports, et les adresses IP.
- **Distribution de trafic** : Répartition du trafic en fonction des règles configurées pour assurer l'équilibre de la charge.

### Session Persistence

La persistance de session, ou affinité de session, assure que les demandes successives d'un client spécifique sont dirigées vers la même instance backend :
- **Types de persistance** : Affinité basée sur IP et affinité basée sur cookie.
- **Configuration de la persistance** : Configurer les paramètres de persistance pour maintenir les sessions de client cohérentes.

### Azure Application Gateway

Azure Application Gateway est un répartiteur de charge de niveau application qui gère le trafic pour les applications web :
- **Fonctionnalités** : Répartition de charge HTTP/HTTPS, pare-feu d'applications web (WAF), et routage basé sur le chemin.
- **Scénarios d'utilisation** : Optimisation de la performance des applications web et sécurisation des applications contre les menaces courantes.

### Application Gateway Components

Les composants de l'Application Gateway incluent :
- **Frontend IP** : Adresse IP publique ou privée utilisée par le gateway.
- **Listeners** : Écouteurs configurés pour écouter le trafic entrant sur des ports spécifiques.
- **Backend Pools** : Groupes de ressources vers lesquelles le trafic est distribué.
- **Rules** : Règles de routage qui déterminent comment le trafic est distribué vers les backend pools.

### Routing Rules

Les règles de routage définissent comment l'Application Gateway gère le trafic entrant :
- **Routage basé sur le chemin** : Distribution du trafic en fonction des chemins URL.
- **Routage multi-site** : Support de plusieurs sites web sur une seule instance d'Application Gateway.
- **Routage de redirection** : Redirection du trafic vers des URL spécifiques basées sur les règles configurées.

### Other Load Balancing Solutions

Azure propose d'autres solutions de répartition de charge pour répondre à différents besoins :
- **Traffic Manager** : Répartition de charge basée sur DNS pour la redirection du trafic aux services globaux.
- **Front Door** : Répartition de charge globale et accélération des applications.
- **Comparaison** : Différences et cas d'utilisation spécifiques pour chaque solution de répartition de charge.

### Network Watcher

Network Watcher est un service de surveillance et de diagnostic du réseau dans Azure :
- **Fonctionnalités** : Capture de paquets, diagnostics de connexion, et surveillance du flux de trafic.
- **Utilisation** : Résolution des problèmes de réseau, surveillance des performances, et analyse du trafic pour la sécurité.
