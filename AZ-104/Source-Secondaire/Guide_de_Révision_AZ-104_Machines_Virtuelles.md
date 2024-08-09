
# Guide de Révision pour l'Examen AZ-104

---

## 1. Configurer des Machines Virtuelles

### Responsabilités des Services Cloud
- **Objectif** : Comprendre les différents services cloud et les responsabilités partagées entre le fournisseur de cloud (Azure) et le client.
- **Notions Clés** :
  - Modèles de service : IaaS, PaaS, SaaS.
  - Partage des responsabilités : Sécurité, maintenance, gestion des données.

### Planifier des Machines Virtuelles
- **Éléments à Considérer** :
  - **Dimensionnement** : Choisir les tailles de VM en fonction des besoins en CPU, RAM, et stockage.
  - **Images** : Sélectionner l'image de système d'exploitation appropriée (Windows, Linux).

### Déterminer le Dimensionnement des Machines Virtuelles
- **Considérations** :
  - Charge de travail : Analyser les besoins en performances pour sélectionner la taille adéquate.
  - Évolutivité : Prévoir des options pour augmenter ou réduire la taille des VM en fonction des besoins futurs.

### Déterminer le Stockage des Machines Virtuelles
- **Types de Stockage** :
  - **Disques gérés** : Stockage persistant pour les VM, optimisé pour des performances spécifiques.
  - **Disques non gérés** : Nécessitent une gestion manuelle des comptes de stockage.
  - **Options** : SSD Premium, Standard SSD, HDD.

### Créer et Connecter des Machines Virtuelles
- **Création** : Via le portail Azure, Azure CLI ou PowerShell.
- **Connexion** : Utilisation de RDP (Remote Desktop Protocol) pour les VM Windows, SSH pour les VM Linux.

---

## 2. Configurer la Disponibilité des Machines Virtuelles

### Maintenance et Temps d'Arrêt
- **Stratégies** :
  - Planifier les temps d'arrêt pour les maintenances.
  - Utiliser les Groupes à Haute Disponibilité pour minimiser l'impact des pannes.

### Groupes à Haute Disponibilité
- **Objectif** : Garantir la disponibilité des applications critiques en cas de panne d’un datacenter.
- **Domaines de Mise à Jour et d'Erreur** :
  - Répartir les machines virtuelles sur différents domaines pour éviter une défaillance commune.

### Zones de Disponibilité et Mise à l'Échelle
- **Zones de Disponibilité** : Répartir les machines dans plusieurs datacenters d'une même région.
- **Mise à l'Échelle** :
  - **Verticale** : Augmenter les ressources (CPU, RAM) d'une VM.
  - **Horizontale** : Ajouter plus de VMs pour gérer la charge.

### Azure Virtual Machine Scale Sets
- **Utilité** : Permet de déployer et gérer un ensemble de VMs identiques.
- **Mise à l'Échelle Automatique** : Configurer pour augmenter ou réduire automatiquement le nombre de VMs en fonction de la demande.

---

## 3. Configurer des Plans Azure App Service

### Implémenter des Plans Azure App Service
- **Objectif** : Héberger des applications web sans gérer l'infrastructure sous-jacente.
- **Tarification** :
  - Plans gratuits ou partagés pour les tests.
  - Plans de production avec des ressources dédiées.

### Mise à l'Échelle d'un Plan Azure App Service
- **Scale-Up** : Augmenter les ressources d'un plan (CPU, RAM).
- **Scale-Out** : Ajouter plus d'instances pour répartir la charge.

### Mise à l'Échelle Automatique
- **Objectif** : Ajuster automatiquement les ressources allouées en fonction du trafic.

---

## 4. Configurer Azure App Service

### Implémenter et Configurer Azure App Service
- **Création d'une Application** : Via le portail Azure ou Azure CLI.
- **Déploiement** : Utiliser l'intégration continue (CI/CD) avec des outils comme GitHub Actions ou Azure DevOps.

### Emplacements de Déploiement
- **Utilité** : Faciliter le test des nouvelles versions de l'application avant leur mise en production.
- **Sécurisation** : Utiliser TLS/SSL pour sécuriser les applications.

### Sauvegarde et Restauration
- **Objectif** : Prévenir la perte de données et garantir une récupération rapide en cas de problème.

---

## 5. Configurer Azure Container Instances

### Comparaison des Conteneurs et Machines Virtuelles
- **Conteneurs** : Légers, démarrent rapidement, partagent le noyau du système d'exploitation.
- **VMs** : Isolation complète, chaque VM a son propre système d'exploitation.

### Implémentation d'Azure Container Instances (ACI)
- **Groupes de Conteneurs** : Plusieurs conteneurs peuvent être gérés ensemble comme une unité.

### Azure Container Apps
- **Utilité** : Gérer des applications conteneurisées avec des fonctionnalités de mise à l'échelle automatique.

---

## 6. Gérer des Machines Virtuelles avec Azure CLI

### Création et Gestion de Machines Virtuelles
- **Commandes Principales** :
  - `az vm create` : Créer une nouvelle VM.
  - `az vm start` : Démarrer une VM.
  - `az vm stop` : Arrêter une VM.
- **Exercices** : Pratiquer la création, le démarrage, l'arrêt, et la configuration des VMs via Azure CLI.

### Installer des Logiciels sur les Machines Virtuelles
- **Automatisation** : Utiliser des scripts pour installer des logiciels et configurer des machines après leur création.

---

## 7. Créer une Machine Virtuelle Windows dans Azure

### Création et Connexion
- **Procédure** :
  - Créer une VM Windows via le portail Azure.
  - Se connecter en utilisant RDP (Remote Desktop Protocol).

### Configurer les Paramètres Réseau
- **Sécurité** :
  - Configurer les NSG (Network Security Groups) pour limiter l'accès aux machines.
  - Mettre en place des règles de pare-feu.

---

## 8. Héberger une Application Web avec Azure App Service

### Création et Déploiement
- **Créer une Application Web** : Via le portail Azure.
- **Déployer le Code** : Utiliser des outils de déploiement CI/CD pour automatiser la mise en production.

### Préparation et Déploiement
- **Préparer le Code** : Assurer que le code est optimisé pour l'environnement Azure.
- **Exercices** : Pratiquer la création et le déploiement d'applications sur Azure App Service.

---

## Conseils de Révision
- **Pratique Active** : Faites des exercices pratiques pour bien maîtriser la création et la gestion des VMs, App Services, et conteneurs.
- **Révisez les Concepts Clés** : Concentrez-vous sur les stratégies de haute disponibilité, la mise à l’échelle, et la gestion des ressources via CLI.
- **Utilisez les Simulations de Labo** : Profitez des simulations interactives pour renforcer vos compétences.

---

Avec ce guide, vous êtes bien préparé pour réussir l’examen AZ-104. Bonne chance !
