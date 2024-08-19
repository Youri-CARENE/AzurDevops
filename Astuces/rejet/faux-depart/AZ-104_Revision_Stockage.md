
# Révision pour la certification AZ-104 : Mettre en œuvre et gérer le stockage

## Configurer l'accès au stockage

### Configurer les pare-feu et les réseaux virtuels d'Azure Storage
- Définir des règles de pare-feu pour restreindre l'accès aux comptes de stockage.
- Configurer des réseaux virtuels pour permettre un accès sécurisé et contrôlé aux ressources de stockage.

### Créer et utiliser des jetons de signature d'accès partagé (SAS)
- Utiliser les SAS pour fournir un accès sécurisé et délégué aux ressources Azure Storage sans partager les clés d'accès.
- Bonnes pratiques :
  - Définir une **date/heure d'expiration**.
  - Limiter la distribution des jetons SAS.
  - Utiliser **HTTPS** pour sécuriser les communications.
  - Durée limitée pour respecter le principe du moindre privilège.

### Configurer les stratégies d'accès stockées
- Les stratégies d'accès stockées permettent un contrôle supplémentaire sur les SAS au niveau du service sur le serveur.
- Configurer un maximum de **5 stratégies d'accès** sur un conteneur, une table, une file d'attente ou un partage à la fois.
- Révoquer ou modifier une stratégie d'accès stockée en modifiant l'identifiant signé ou la date d'expiration.

### Gérer les clés d'accès
- Gérer les clés d'accès pour sécuriser les communications avec Azure Storage.
- Options d'autorisation :
  - **Azure AD** pour la gestion d'identité et d'accès.
  - **Signatures d'accès partagé** pour un accès limité et temporaire.
  - **Clés partagées** pour une autorisation basée sur les clés d'accès.

### Configurer l'accès basé sur l'identité pour Azure Files
- Configurer Azure Files pour utiliser Azure AD pour l'authentification et l'accès aux partages de fichiers.

## Azure Storage

Azure Storage est un service de stockage cloud permettant de stocker des fichiers, des messages, des tables, et d'autres types d'informations de manière sécurisée, évolutive, et accessible.

### Types de données et services de stockage
- **Données non structurées** : 
  - **Blobs** : objets binaires volumineux accessibles via des APIs REST.
  - **Azure Data Lake Storage** : gestion des systèmes de fichiers en tant que service.
- **Données structurées** :
  - **Tables** : stockage NoSQL sans schéma.
  - **Cosmos DB** : base de données distribuée globalement.
  - **Azure SQL DB** : base de données relationnelle.

### Services Azure Storage
- **Azure Containers** : stockage d'objets pour des données textuelles et binaires non structurées.
- **Azure Files** : gestion des partages de fichiers pour les déploiements cloud ou sur site.
- **Azure Tables** : stockage NoSQL pour les données structurées.
- **Azure Queues** : gestion des communications entre les composants d'une application via des files d'attente.

### URL des objets stockés
- Chaque objet stocké a un URL unique :
  - **Conteneurs** : `http://storageacctname.blob.core.windows.net`
  - **Fichiers** : `http://storageacctname.file.core.windows.net`
  - **Tables** : `http://storageacctname.table.core.windows.net`
  - **Files d'attente** : `http://storageacctname.queue.core.windows.net`
- Les domaines personnalisés peuvent être configurés après validation.

## Redondance du stockage

### Types de redondance
- **Stockage localement redondant (LRS)** :
  - Réplication synchrone trois fois dans un seul centre de données.
  - Protection limitée contre les pannes de racks ou de disques.

- **Stockage redondant par zone (ZRS)** :
  - Réplication synchrone entre trois zones de disponibilité dans la région principale.
  - Haute disponibilité et durabilité avec protection contre les pannes de zone.

- **Stockage géo-redondant (GRS)** :
  - Réplication synchrone dans la région principale (LRS), puis asynchrone dans une région secondaire.
  - Les données de la région secondaire ne sont pas accessibles pour la lecture/écriture sauf en cas de basculement.

- **Stockage géo-zone-redondant (GZRS)** :
  - Réplication synchrone dans trois zones de disponibilité, puis asynchrone dans une région secondaire.
  - Combine les avantages de ZRS dans la région principale et de GRS dans la région secondaire.

## Chiffrement du stockage

### Chiffrement des services de stockage (SSE)
- Activé par défaut avec un chiffrement AES 256 bits.
- Options pour la gestion des clés :
  - **Clés gérées par Microsoft** : rotation automatique par Microsoft.
  - **Clés gérées par le client** : stockage dans Azure Key Vault.

## Outils de stockage

### Explorateur de stockage Azure
- Outil graphique pour gérer les comptes et abonnements de stockage.
- Supporte Windows, macOS, et Linux.

### AzCopy
- Outil en ligne de commande pour copier des données vers et depuis le blob, le fichier, et le stockage de table.
- Supporte Windows, macOS, et Linux.

## Configurer Azure Files et Azure Blob Storage

### Configurer un partage de fichiers et un conteneur Blob
- Créer et configurer des partages de fichiers dans Azure Storage.
- Créer et configurer des conteneurs dans Blob Storage.
- Configurer les niveaux de stockage, les instantanés, et la suppression réversible.

### Stockage immuable pour Blob Storage
- **Stockage WORM (Write Once, Read Many)** :
  - Les données ne peuvent pas être modifiées ou supprimées pendant une période définie.
  - Deux types de politiques : **basées sur le temps** et **de conservation légale**.

