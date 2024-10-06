
# Surveiller et maintenir les ressources Azure (10–15%)

## Surveiller les ressources à l'aide d'Azure Monitor

Azure Monitor vous permet de surveiller les ressources Azure pour identifier les problèmes potentiels et optimiser les performances.

### Configurer et interpréter les métriques

- Azure Monitor collecte des métriques à partir de vos ressources Azure.
- Les métriques fournissent des données en temps quasi-réel pour vous aider à comprendre les performances et la santé de vos ressources.
- Utilisez les métriques pour identifier les tendances, diagnostiquer les problèmes et déclencher des alertes.

### Configurer Azure Monitor Logs

- Azure Monitor Logs collecte et organise les journaux des ressources Azure.
- Les logs sont stockés dans un espace de travail Log Analytics où ils peuvent être analysés.
- Vous pouvez configurer des sources de données pour envoyer des logs vers Azure Monitor Logs, telles que les machines virtuelles, les applications et les services Azure.

### Interroger et analyser les journaux

- Utilisez Kusto Query Language (KQL) pour interroger et analyser les données dans Azure Monitor Logs.
- Créez des requêtes pour extraire des informations précises, générer des rapports et surveiller les événements critiques.
- Les résultats des requêtes peuvent être visualisés sous forme de tableaux, de graphiques ou exportés pour une analyse plus approfondie.

### Configurer des alertes et des actions

- Les alertes Azure Monitor sont configurées pour surveiller des conditions spécifiques dans vos ressources.
- Une alerte se compose de règles d'alerte définissant les conditions, les signaux à surveiller et les ressources à surveiller.
- Lorsqu'une alerte est déclenchée, des actions peuvent être exécutées automatiquement, telles que l'envoi de notifications aux administrateurs.

### Configurer la surveillance des machines virtuelles (VM), des comptes de stockage et des réseaux à l'aide des insights pour VM

- Azure Monitor propose des insights spécifiques pour les VM, les comptes de stockage et les réseaux.
- Les insights pour VM fournissent une visibilité approfondie sur les performances et la santé des machines virtuelles.
- Surveillez les métriques de CPU, de mémoire, de disque et de réseau pour identifier les problèmes et optimiser l'utilisation des ressources.

## Azure Monitor Alerts

Azure Monitor Alerts vous aide à rester informé des problèmes potentiels en capturant les logs et les données télémétriques des métriques.

### Types d'alertes

- **Alertes sur les métriques** : Déclenchées lorsque les métriques surveillées dépassent un seuil spécifié.
- **Alertes sur les journaux** : Basées sur des requêtes de logs spécifiques.
- **Événements du journal d'activités** : Déclenchées par des modifications ou des événements dans Azure.
- **Alertes de détection intelligente** : Utilisent des algorithmes d'apprentissage automatique pour détecter des anomalies dans les métriques.

### États des alertes

- **Nouvelle** : Alarme ouverte et non révisée.
- **Reconnu** : Alarme en cours de révision, le travail est en cours.
- **Fermé** : Problème résolu.

### Alertes sans état

- Déclenchées chaque fois qu'une condition de règle d'alerte correspond aux données analysées, même si la même alerte existe déjà.

### Alertes avec état

- Déclenchées lorsque les conditions de la règle correspondent aux données et qu'il n'existe pas encore d'alerte similaire.

## Implémenter la sauvegarde et la récupération

### Créer un coffre de services de récupération Azure

- Un coffre de services de récupération Azure stocke les données de sauvegarde, y compris les copies de configuration pour les postes de travail, les serveurs, les VM, et plus encore.
- Pour créer un coffre, vous aurez besoin de spécifier l'abonnement, le groupe de ressources, le nom du coffre et la région.

### Créer un coffre de sauvegarde Azure

- Un coffre de sauvegarde Azure est utilisé pour sauvegarder, protéger et restaurer des données dans le cloud.
- Les coffres de sauvegarde sont configurés pour stocker les données de manière sécurisée avec des options de réplication.

### Créer et configurer une stratégie de sauvegarde

- Les stratégies de sauvegarde définissent la fréquence et la durée des sauvegardes.
- Configurez des stratégies pour répondre aux besoins de rétention des données à court et long terme.

### Effectuer des opérations de sauvegarde et de restauration à l'aide d'Azure Backup

- Azure Backup permet de sauvegarder des machines virtuelles, des bases de données SQL, et d'autres services Azure.
- Les opérations de restauration récupèrent les données à partir du coffre de services de récupération en cas de besoin.

### Configurer Azure Site Recovery pour les ressources Azure

- Azure Site Recovery offre des solutions de récupération après sinistre pour les services Azure.
- Configurez la réplication des ressources vers une région secondaire pour garantir une haute disponibilité en cas de panne régionale.

### Effectuer un basculement vers une région secondaire à l'aide d'Azure Site Recovery

- Le basculement vers une région secondaire est un processus crucial pour la continuité des activités en cas de panne majeure.
- Azure Site Recovery permet de basculer les ressources vers une région secondaire configurée.

### Configurer et examiner les rapports de sauvegarde

- Les rapports de sauvegarde vous permettent de suivre l'état des sauvegardes, les succès et les échecs.
- Utilisez Backup Center pour unifier la gestion, la surveillance et la gouvernance des sauvegardes à grande échelle.

## Azure Backup

Azure Backup offre une solution cloud pour sauvegarder, protéger et restaurer des données.

### Avantages d'utiliser Azure Backup

- **Sécurité** : Les données sont sécurisées par chiffrement avec une phrase de passe locale.
- **Transfert de données illimité** : Sans frais supplémentaires pour les transferts de données.
- **Compatibilité applicative** : Les sauvegardes sont cohérentes avec les applications, assurant une restauration complète sans corrections supplémentaires.
- **Gestion automatique du stockage** : Plus besoin de stockage sur site, Azure Backup gère tout.
- **Rétention longue durée** : Les données peuvent être conservées à long terme avec une limite de 9 999 points de récupération par instance protégée.
- **Réplication géoredondante (GRS)** : Réplique les données vers une autre région secondaire pour une haute disponibilité.
- **Réplication localement redondante (LRS)** : Réplique les données 3 fois dans le même centre de données pour une protection contre les pannes matérielles.

## Coffre de services de récupération Azure

- Stocke les données de sauvegarde des services Azure et sur site.
- Permet d'organiser et de gérer les données de sauvegarde de manière centralisée.
- **Services pouvant être sauvegardés** : VM (Windows et Linux), bases de données Azure SQL, serveurs Windows, System Center DPM, et plus encore.

## Backup Center

Backup Center offre une interface unifiée pour gérer et surveiller les sauvegardes dans Azure.

### Avantages de Backup Center

- **Gestion centralisée** : Surveiller et gérer les sauvegardes à travers plusieurs charges de travail, abonnements et régions.
- **Rapports détaillés** : Utilise les Workbooks d'Azure Monitor pour des rapports complets sur les sauvegardes.
- **Gouvernance** : Intègre Azure Policy pour gouverner les sauvegardes et assurer la conformité.

