
# Guide de Révision pour l'Examen AZ-104

---

## 1. Configurer des Comptes de Stockage

### Implémenter le Stockage Azure
- **Objectif** : Comprendre comment configurer et gérer des comptes de stockage dans Azure.
- **Services à explorer** : Blob Storage, Queue Storage, Table Storage, File Storage.
- **Étapes principales** :
  - Création d'un compte de stockage via le portail Azure.
  - Configuration des options de réplication (LRS, GRS, RA-GRS, ZRS).
  - Définition des points de terminaison pour accéder aux services.

### Types de Comptes de Stockage
- **Comptes de stockage général** :
  - V1 : Utilisé pour la compatibilité avec les anciennes applications.
  - V2 : Offre les fonctionnalités les plus récentes et optimise les coûts.
- **Comptes Blob Storage** : Spécialisé pour le stockage d'objets blob, avec un accent sur les performances et les niveaux d'accès.

### Stratégies de Réplication
- **Locally Redundant Storage (LRS)** : Réplication des données dans un même datacenter.
- **Geo-Redundant Storage (GRS)** : Réplication des données dans un autre datacenter distant pour assurer la résilience géographique.
- **Read-Access Geo-Redundant Storage (RA-GRS)** : Ajoute l'accès en lecture aux répliques géographiquement distantes.

### Sécurisation des Points de Terminaison de Stockage
- **Importance** : Les points de terminaison permettent d’accéder aux services de stockage, il est donc crucial de les sécuriser.
- **Méthodes** :
  - Utilisation des Firewalls et des règles réseau.
  - Activation du HTTPS obligatoire pour les transactions.

---

## 2. Configurer le Stockage Blob Azure

### Implémenter le Stockage Blob Azure
- **Processus** :
  - Créer des conteneurs pour organiser les blobs.
  - Gérer les niveaux d’accès (Hot, Cool, Archive) selon la fréquence d’utilisation des données.
  - Configurer des règles de gestion du cycle de vie pour automatiser le déplacement des blobs entre les niveaux d'accès.

### Réplication d’Objets Blob
- **Options de réplication** : Choisir la réplication en fonction des besoins de résilience et de disponibilité.
- **Impact sur les coûts** : Comprendre comment la réplication affecte les coûts du stockage Blob.

### Simulation de Labo
- **Objectif** : Pratiquer la création, la gestion des conteneurs et l’assignation des niveaux d’accès via des exercices pratiques.

---

## 3. Configurer la Sécurité du Stockage Azure

### Stratégies de Sécurité du Stockage Azure
- **Signatures d’accès partagé (SAS)** : Permettent de déléguer l'accès aux ressources de stockage avec des permissions spécifiques et des durées limitées.
- **Chiffrement des Données** :
  - **At Rest** : Données chiffrées par défaut dans Azure.
  - **In Transit** : Utilisation de TLS pour sécuriser les données en transit.

### Créer des Clés Gérées par le Client
- **Méthode** : Générer des clés de chiffrement personnalisées et les gérer via Azure Key Vault.

### Simulation de Labo
- **Exercice** : Appliquer les meilleures pratiques de sécurité, créer des signatures SAS, et configurer des clés de chiffrement.

---

## 4. Configurer Azure Files et Azure File Sync

### Comparer le Stockage pour les Partages de Fichiers et les Blobs
- **Azure Files** : Meilleure solution pour les partages de fichiers, surtout pour les scénarios de remplacement de serveurs de fichiers on-premises.
- **Blobs** : Optimisés pour le stockage d'objets, moins efficace pour les partages de fichiers.

### Gestion des Partages de Fichiers Azure
- **Création et Gestion** :
  - Créer des partages de fichiers via le portail Azure.
  - Configurer la suppression réversible pour récupérer des fichiers supprimés accidentellement.

### Déployer Azure File Sync
- **Utilité** : Synchroniser les données entre les partages de fichiers Azure et les serveurs de fichiers on-premises.
- **Étapes** :
  - Installer l'agent Azure File Sync sur les serveurs.
  - Configurer la synchronisation dans le portail Azure.

---

## 5. Créer un Compte de Stockage Azure

### Déterminer les Besoins en Comptes de Stockage
- **Évaluation** :
  - Identifier le nombre de comptes de stockage nécessaires en fonction de la charge de travail.
  - Définir les paramètres tels que le type de stockage, la réplication et la sécurité.

### Choisir un Outil de Création de Compte
- **Options** :
  - Portail Azure : Interface graphique.
  - Azure CLI : Ligne de commande pour les utilisateurs avancés.

### Exercice Pratique
- **Création d’un compte** :
  - Utiliser le portail Azure pour créer un compte de stockage et configurer les options de réplication et de sécurité.

---

## 6. Contrôler l’Accès au Stockage Azure avec des Signatures d’Accès Partagé

### Utiliser des Signatures d’Accès Partagé (SAS)
- **Objectif** : Déléguer l’accès sécurisé aux données dans les comptes de stockage Azure.
- **Paramètres** :
  - Période de validité.
  - Permissions spécifiques (lecture, écriture, suppression, etc.).

### Exercice Pratique
- **Mise en place** : Créer et utiliser des SAS pour permettre un accès contrôlé aux données.

---

## 7. Charger, Télécharger et Gérer des Données avec l’Explorateur de Stockage Azure

### Connecter l’Explorateur Stockage Azure à un Compte de Stockage
- **Objectif** : Utiliser une interface graphique pour gérer facilement les services de stockage Azure.
- **Connexion** : Ajouter des comptes de stockage et naviguer entre les services disponibles.

### Exercice Pratique
- **Manipulation des Données** :
  - Charger et télécharger des données.
  - Connecter l’explorateur au stockage Azure Data Lake pour des cas d’utilisation Big Data.

---

## Conseils de Révision
- **Pratiquez régulièrement** : Faites des exercices pratiques dans un environnement de labo pour bien comprendre les configurations et les commandes.
- **Révisez les concepts clés** : Concentrez-vous sur les options de réplication, les stratégies de sécurité, et la gestion des comptes de stockage.
- **Utilisez l’Explorateur Stockage Azure** : Familiarisez-vous avec cet outil pour gérer les données efficacement.

---

Avec ce guide, vous êtes équipé pour réviser efficacement et réussir l’examen AZ-104. Bonne chance !
