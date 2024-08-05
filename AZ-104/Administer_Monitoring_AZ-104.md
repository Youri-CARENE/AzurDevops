
## Administer Monitoring

### Module Introduction

L'administration de la surveillance dans Azure couvre les outils et les techniques pour surveiller les ressources et les activités. Ce module vous guide à travers les concepts et les meilleures pratiques pour configurer et utiliser Azure Monitor, les journaux d'activité, les espaces de travail Log Analytics, et les alertes Azure.

### Azure Monitor

Azure Monitor offre des fonctionnalités de surveillance et de gestion pour collecter, analyser et agir sur les données des ressources Azure :
- **Fonctionnalités** : Surveillance des performances, collecte des journaux, création de tableaux de bord personnalisés.
- **Sources de données** : Collecte de données à partir de VM, d'applications, de conteneurs et d'autres ressources Azure.
- **Insights** : Utiliser les insights d'Azure Monitor pour obtenir des analyses approfondies des applications et des infrastructures.

### Azure Activity Logs

Les journaux d'activité Azure enregistrent toutes les opérations effectuées sur les ressources Azure :
- **Types d'événements** : Opérations de gestion, alertes de service, mises à jour de service.
- **Consultation des journaux** : Utiliser le portail Azure, Azure CLI ou PowerShell pour accéder aux journaux d'activité.
- **Analyse** : Analyser les journaux pour identifier les actions et résoudre les problèmes.

### Enable Log Analytics Workspace

L'espace de travail Log Analytics est utilisé pour collecter et analyser les données de journalisation à partir de diverses sources :
- **Création de l'espace de travail** : Configurer un espace de travail Log Analytics via le portail Azure.
- **Connexion des sources de données** : Ajouter des VM, des applications et d'autres sources à l'espace de travail.
- **Configuration des paramètres** : Définir des politiques de rétention et de collecte des données.

### Querying Log Analytics Workspace

La requête dans Log Analytics Workspace permet d'extraire et d'analyser les données collectées :
- **Kusto Query Language (KQL)** : Utiliser KQL pour écrire des requêtes et analyser les données.
- **Exemples de requêtes** : Requêtes courantes pour surveiller les performances des VM, des applications et des réseaux.
- **Visualisation** : Créer des visualisations et des tableaux de bord basés sur les résultats des requêtes.

### Azure Alerts

Les alertes Azure notifient les administrateurs des conditions spécifiques ou des anomalies détectées dans les ressources surveillées :
- **Types d'alertes** : Alertes basées sur les métriques, les journaux et les journaux d'activité.
- **Configuration des alertes** : Définir des critères d'alerte, configurer les actions et les notifications.
- **Gestion des alertes** : Surveiller et gérer les alertes via le portail Azure, Azure CLI ou PowerShell.
