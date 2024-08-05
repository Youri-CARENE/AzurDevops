
## Administer Azure Storage

### Module Introduction

L'administration du stockage Azure couvre la gestion des comptes de stockage, la redondance des données, l'accès aux points de terminaison de stockage, la sécurité des données, et plus encore. Ce module vous guide à travers les concepts et les outils nécessaires pour gérer efficacement le stockage dans Azure.

### Storage Accounts

Les comptes de stockage Azure permettent de stocker des objets, des fichiers, des disques et des tables :
- **Types de comptes de stockage** : Stockage standard et premium.
- **Services de stockage** : Blobs, Files, Queues, Tables et Disques gérés.
- **Création et configuration** : Paramètres de performance, d'accès et de sécurité.

### Storage Redundancy

La redondance de stockage assure la disponibilité et la durabilité des données :
- **LRS (Local Redundant Storage)** : Réplication des données dans un datacenter.
- **ZRS (Zone Redundant Storage)** : Réplication des données dans des zones de disponibilité.
- **GRS (Geo-Redundant Storage)** : Réplication des données entre régions géographiques.
- **RA-GRS (Read-Access Geo-Redundant Storage)** : GRS avec accès en lecture aux réplicas secondaires.

### Accessing Storage Endpoints

L'accès aux points de terminaison de stockage est essentiel pour interagir avec les services de stockage :
- **Types de points de terminaison** : Public, privé et service endpoints.
- **Configuration de l'accès** : Utilisation des clés d'accès et des signatures d'accès partagé (SAS).

### Azure Containers

Les conteneurs Azure permettent de stocker et organiser des blobs dans des comptes de stockage :
- **Création de conteneurs** : Organiser les blobs en groupes logiques.
- **Gestion des blobs** : Chargement, téléchargement, et gestion des blobs.

### Storage Tiers

Les niveaux de stockage permettent de gérer les coûts et les performances du stockage :
- **Niveaux** : Hot, Cool et Archive.
- **Cas d'utilisation** : Utilisation appropriée des niveaux pour optimiser les coûts et les performances.

### Lifecycle Management

La gestion du cycle de vie permet d'automatiser les transitions de niveau de stockage et la suppression des données :
- **Politiques de cycle de vie** : Définir des règles pour gérer les données à différentes étapes de leur cycle de vie.
- **Automatisation** : Configuration de l'automatisation pour la transition et la suppression des données.

### Creating Azure File Share

Azure File Share permet de créer des partages de fichiers accessibles via SMB :
- **Création de partages de fichiers** : Configuration des partages de fichiers dans les comptes de stockage.
- **Gestion des fichiers** : Chargement, accès et gestion des fichiers dans les partages de fichiers.

### Securing Storage Endpoints

La sécurisation des points de terminaison de stockage est cruciale pour protéger les données :
- **Firewall et règles de réseau** : Configuration des règles pour limiter l'accès aux points de terminaison de stockage.
- **VNet Service Endpoints** : Intégration avec des réseaux virtuels pour sécuriser l'accès.

### Storage Service Encryption (SSE) and Azure Disk Encryption (ADE)

Le chiffrement des services de stockage et des disques assure la protection des données au repos :
- **SSE** : Chiffrement des données pour les services Blob, File, Queue et Table.
- **ADE** : Chiffrement des disques gérés et non gérés avec Azure Key Vault.

### Configuring Storage Access

La configuration de l'accès au stockage permet de gérer les permissions et les contrôles d'accès :
- **Niveaux d'accès** : Public, privé et restreint.
- **Gestion des permissions** : Utilisation de RBAC et de SAS pour contrôler l'accès.

### Storage Account Access Keys

Les clés d'accès aux comptes de stockage permettent l'authentification des requêtes :
- **Gestion des clés** : Rotation régulière des clés pour des raisons de sécurité.
- **Utilisation des clés** : Utilisation des clés d'accès pour interagir avec les services de stockage.

### Shared Access Signatures

Les signatures d'accès partagé (SAS) permettent de déléguer l'accès aux ressources de stockage avec des permissions spécifiques et une durée limitée :
- **Création de SAS** : Générer des SAS pour déléguer l'accès.
- **Gestion des SAS** : Contrôler et révoquer l'accès en fonction des besoins.

### Microsoft Entra ID Authentication

L'authentification via Microsoft Entra ID (anciennement Azure AD) permet une gestion sécurisée et centralisée des accès :
- **Intégration avec Entra ID** : Utilisation des identités pour authentifier l'accès aux ressources de stockage.
- **RBAC** : Configuration des rôles et des permissions basées sur les identités.
