
# Guide de Révision pour l'Examen AZ-104

---

## 1. Configurer des Réseaux Virtuels

### Planifier et Créer des Réseaux Virtuels
- **Planification** : Identifier les besoins en connectivité, sécurité, et performance pour concevoir un réseau adapté.
- **Création des Sous-Réseaux** : Diviser les réseaux virtuels en sous-réseaux pour une gestion granulaire des ressources.
- **Adressage IP** : 
  - **Public** : Utilisé pour les services nécessitant une accessibilité depuis l'extérieur.
  - **Privé** : Réservé pour la communication interne au sein du réseau virtuel.

### Configuration de l'Adressage IP
- **Création d'Adresses IP Publiques** : Affecter des IP publiques pour les services nécessitant un accès externe.
- **Attribution d'Adresses IP Privées** : Utilisation pour la communication interne et sécurisée entre les ressources du réseau.

---

## 2. Configurer des Groupes de Sécurité Réseau (NSG)

### Implémentation des NSG
- **Fonctionnalité** : Contrôle d'accès au réseau en définissant des règles d'autorisation ou de refus pour le trafic entrant et sortant.
- **Création des Règles** :
  - Règles de sécurité pour autoriser ou bloquer le trafic.
  - Règles effectives qui combinent les règles par défaut et les règles personnalisées.
- **Groupes de Sécurité d’Applications** : Appliquer des règles de sécurité en fonction des applications spécifiques plutôt que des IP ou des sous-réseaux.

### Vérification des Règles NSG
- **Simulation de Labo** : Pratiquer l'implémentation et la vérification des règles NSG dans un environnement sécurisé.

---

## 3. Configurer un Peering de Réseaux Virtuels Azure

### Configuration du Peering
- **Utilité** : Permettre la communication entre deux réseaux virtuels différents dans Azure.
- **Création du Peering** : Établir la connexion via le portail Azure ou les commandes CLI.
- **Extensions du Peering** :
  - Routes définies par l'utilisateur.
  - Chaînage de services pour des configurations plus complexes.

---

## 4. Configurer le Routage et les Points de Terminaison Réseau

### Configurer des Routes Réseau
- **Routes Système** : Gérées automatiquement par Azure pour le routage interne.
- **Routes Définies par l'Utilisateur** : Personnaliser le routage pour répondre à des besoins spécifiques de sécurité ou de performance.

### Points de Terminaison et Liaisons Privées
- **Points de Terminaison de Service** : Sécuriser les connexions aux services Azure sans exposer de ressources publiques.
- **Liaisons Privées** : Connecter les réseaux virtuels via des connexions privées directes, contournant l'internet public.

---

## 5. Configurer Azure Load Balancer

### Azure Load Balancer
- **Fonctionnalités** :
  - Répartition du trafic pour les applications critiques pour améliorer la disponibilité.
  - Support pour des équilibreurs de charge publics et internes.
- **Création des Pools de Back-Ends et Sondes d'Intégrité** : Gérer les services connectés et surveiller leur état de santé.
- **Configuration des Règles d’Équilibrage** : Définir comment le trafic est distribué entre les instances.

---

## 6. Configurer Azure Application Gateway

### Azure Application Gateway
- **Implémentation** : Configurer une passerelle applicative pour gérer le trafic HTTP/HTTPS avec des fonctionnalités avancées comme le routage basé sur le chemin et le routage basé sur plusieurs sites.
- **Routage** : Déterminer comment le trafic est acheminé en fonction des règles de la passerelle.

### Composants Clés
- **Composants de l’Application Gateway** :
  - Listeners, Backend Pools, Rules.
  - Configurer ces composants pour gérer efficacement le trafic d'application.

---

## 7. Concevoir un Schéma d'Adressage IP pour Azure

### Schéma d'Adressage IP
- **Objectif** : Fournir une structure flexible qui peut s'adapter à la croissance tout en garantissant une intégration fluide avec les réseaux locaux.
- **Planification** : Concevoir l’adressage IP en tenant compte de la communication entre les services et de la sécurité des systèmes.

### Exercice Pratique
- **Conception et Implémentation** : Pratiquer la mise en place d'un schéma d'adressage IP pour un déploiement réel dans Azure.

---

## 8. Distribuer les Services sur les Réseaux Virtuels avec le Peering

### Peering des Réseaux Virtuels
- **Intégration** : Connecter des services de manière sécurisée à travers plusieurs réseaux virtuels.
- **Commandes CLI** : Utiliser Azure CLI pour configurer et vérifier les connexions de peering.

---

## 9. Héberger votre Domaine sur Azure DNS

### Azure DNS
- **Fonctionnalité** : Gestion DNS pour les domaines hébergés dans Azure.
- **Configuration** : Créer des zones DNS et des enregistrements pour mapper des domaines aux adresses IP.
- **Résolution Dynamique** : Utiliser des enregistrements d’alias pour mapper dynamiquement les ressources Azure.

---

## 10. Gérer le Flux de Trafic avec des Routes Personnalisées

### Routes Personnalisées
- **Fonctionnalités** : Diriger le trafic au sein des réseaux virtuels en fonction des besoins spécifiques.
- **Appliance Virtuelle Réseau (NVA)** : Utiliser des appliances virtuelles pour gérer le routage du trafic de manière avancée.

### Exercices Pratiques
- **Créer et Gérer les Routes** : Implémenter des routes personnalisées et configurer les appliances virtuelles pour contrôler le flux de trafic.

---

## 11. Améliorer la Scalabilité avec Azure Load Balancer

### Scalabilité et Résilience
- **Azure Load Balancer** : Utiliser l'équilibrage de charge pour améliorer la scalabilité et la disponibilité des applications.
- **Comparaison des Équilibreurs de Charge** : Choisir le type d'équilibreur de charge (public ou interne) en fonction des besoins de l'application.

### Exercice Pratique
- **Configurer un Équilibreur de Charge** : Pratiquer la configuration d'un équilibreur de charge public et interne pour différentes applications.

---

## Conseils de Révision
- **Pratique Active** : Faites des exercices pratiques pour bien maîtriser la configuration des réseaux, des NSG, des Load Balancers, et des routes personnalisées.
- **Révisez les Concepts Clés** : Concentrez-vous sur les schémas d'adressage IP, le peering, et la sécurisation des réseaux avec les NSG.
- **Utilisez les Simulations de Labo** : Profitez des simulations interactives pour renforcer vos compétences avant l'examen.

