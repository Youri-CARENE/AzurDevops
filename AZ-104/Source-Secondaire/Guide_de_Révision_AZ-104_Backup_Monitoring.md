
# Guide de Révision pour l'Examen AZ-104

---

## 1. Présentation d'Azure Backup

### Qu'est-ce qu'Azure Backup ?
- **Fonctionnalité** : Service de sauvegarde basé sur le cloud qui protège les données en créant des copies sécurisées des fichiers, dossiers, machines virtuelles et applications.
- **Utilisations** :
  - Sauvegarde des machines virtuelles, bases de données SQL, et autres ressources Azure.
  - Récupération des données en cas de perte ou de corruption.

### Fonctionnement de la Sauvegarde Azure
- **Processus** :
  - Créer un coffre de sauvegarde (Recovery Services Vault).
  - Configurer les stratégies de sauvegarde pour automatiser les sauvegardes.
  - Restaurer les données à partir des points de récupération.

### Quand utiliser Azure Backup ?
- **Cas d'usage** :
  - Protection des données critiques.
  - Conformité réglementaire et besoins en récupération d’urgence.

---

## 2. Configurer des Sauvegardes de Machines Virtuelles

### Options de Protection des Données des Machines Virtuelles
- **Stratégies** :
  - Sauvegardes régulières.
  - Snapshots pour des copies rapides.
  - Réplication des données pour la résilience.

### Configurer les Sauvegardes dans un Coffre Recovery Services
- **Création d’un Coffre** : Utilisez le portail Azure pour configurer un coffre Recovery Services.
- **Options de Sauvegarde** : Choisir la fréquence et la rétention des sauvegardes.
- **Restaurer des Machines Virtuelles** : Récupérer des VMs à partir des points de restauration.

### Implémenter la Suppression Réversible et Azure Site Recovery
- **Suppression Réversible** : Protège contre les suppressions accidentelles.
- **Azure Site Recovery** : Utilisé pour la continuité des opérations en cas de panne majeure.

### Simulation de Labo
- **Exercice Pratique** : Configurer des sauvegardes et tester la restauration des machines virtuelles.

---

## 3. Configurer Azure Monitor

### Fonctionnalités Clés d'Azure Monitor
- **Surveillance** : Collecte des données en temps réel sur les performances, l'intégrité et les journaux des ressources Azure.
- **Composants** :
  - **Métriques** : Données numériques sur l'état des ressources.
  - **Journaux** : Informations détaillées sur les événements du système.

### Configuration d'Azure Monitor
- **Définir les Métriques et Journaux** : Choisir les données à surveiller pour optimiser les performances.
- **Interroger le Journal d'Activité** : Analyser les événements enregistrés pour diagnostiquer les problèmes.

---

## 4. Configurer Log Analytics

### Utilisation de Log Analytics
- **Objectif** : Centraliser les données des journaux pour les analyser avec des requêtes spécifiques.
- **Création d'un Espace de Travail** : Configurer un espace de travail Log Analytics pour regrouper les données.

### Structurer des Requêtes Kusto (KQL)
- **Kusto Query Language (KQL)** : Langage utilisé pour interroger les données de Log Analytics.
- **Exercice Pratique** : Rédiger des requêtes KQL pour extraire des informations pertinentes des journaux.

---

## 5. Configurer Network Watcher

### Fonctionnalités de Network Watcher
- **Diagnostic Réseau** : Outil pour surveiller et diagnostiquer les problèmes de connectivité réseau dans Azure.
- **Visualisation de la Topologie Réseau** : Afficher la structure de votre réseau pour comprendre la connectivité et les flux de données.

### Diagnostic des Flux IP et Tronçons Suivants
- **Flux IP** : Vérifier le chemin des paquets à travers le réseau.
- **Tronçons Suivants** : Déterminer le prochain saut pour les paquets envoyés depuis une ressource Azure.

---

## 6. Améliorer la Réponse aux Incidents avec les Alertes Azure Monitor

### Types d'Alerte dans Azure Monitor
- **Métriques** : Signaler des anomalies dans les performances.
- **Journaux** : Identifier des événements spécifiques à surveiller.
- **Groupes d'Actions** : Définir les actions à entreprendre lorsqu'une alerte est déclenchée.

### Utiliser les Alertes pour Répondre aux Incidents
- **Exercice Pratique** : Configurer des alertes basées sur les métriques et journaux pour surveiller et réagir aux incidents.

---

## 7. Analyser l'Infrastructure Azure avec les Journaux Azure Monitor

### Extraction d'Informations à Partir des Journaux
- **Création de Requêtes** : Utiliser Azure Monitor pour rédiger des requêtes qui extraient des informations clés des journaux.
- **Exercice Pratique** : Créer et tester des requêtes pour surveiller l'infrastructure.

---

## 8. Surveiller les Machines Virtuelles Azure avec Azure Monitor

### Surveillance des Machines Virtuelles
- **Données Collectées** :
  - **Métriques d'Hôte** : Suivi des performances de l'hyperviseur.
  - **Journaux Client** : Suivi des événements spécifiques à la machine virtuelle.

### Utilisation de Metrics Explorer
- **Metrics Explorer** : Outil pour visualiser et analyser les métriques collectées.
- **Collecte des Compteurs de Performances** : Surveiller l'utilisation des ressources des machines virtuelles pour optimiser les performances.

---

## Conseils de Révision
- **Pratique Active** : Faites des exercices pratiques pour bien maîtriser la configuration des sauvegardes, la surveillance avec Azure Monitor, et l'analyse des journaux.
- **Révisez les Concepts Clés** : Concentrez-vous sur la récupération d’urgence avec Azure Backup, l'optimisation des performances avec Azure Monitor, et la gestion des journaux avec Log Analytics.
- **Utilisez les Simulations de Labo** : Profitez des simulations interactives pour renforcer vos compétences avant l'examen.

-
