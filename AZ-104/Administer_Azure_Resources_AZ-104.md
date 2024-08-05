
## Administer Azure Resources

### Module Introduction

Ce module couvre les outils et les techniques nécessaires pour administrer efficacement les ressources Azure. Vous apprendrez à utiliser divers outils d'administration, à comprendre et à déployer des ressources via Azure Resource Manager (ARM), et à travailler avec des modèles ARM et Azure Bicep.

### Compare Administrator Tools

Azure offre plusieurs outils pour administrer les ressources. Les principaux outils incluent :
- **Portail Azure** : Interface graphique pour gérer et surveiller les services Azure.
- **Azure PowerShell** : Interface en ligne de commande pour automatiser les tâches de gestion Azure.
- **Azure CLI** : Interface en ligne de commande multiplateforme pour gérer les ressources Azure.
- **Azure Cloud Shell** : Environnement shell accessible via le portail Azure, prenant en charge Azure PowerShell et Azure CLI.
- **Azure Resource Manager** : Interface pour déployer, gérer et surveiller les ressources Azure de manière cohérente.

### Azure Resource Manager

Azure Resource Manager (ARM) est la couche de gestion pour toutes les ressources Azure. Les principaux concepts incluent :
- **Groupes de ressources** : Conteneurs qui regroupent les ressources Azure liées pour une gestion commune.
- **Modèles ARM** : Fichiers JSON qui définissent l'infrastructure et les configurations des ressources Azure.
- **Déploiement basé sur des modèles** : Utilisation des modèles ARM pour déployer, mettre à jour et supprimer des ressources de manière déclarative.
- **Contrôle d'accès basé sur les rôles (RBAC)** : Gestion des autorisations pour les ressources Azure via ARM.

### Azure Resource Manager Templates

Les modèles ARM sont utilisés pour définir l'infrastructure Azure de manière déclarative :
- **Structure des modèles** : Fichiers JSON contenant des sections telles que `schema`, `contentVersion`, `parameters`, `variables`, `resources`, et `outputs`.
- **Déploiement de modèles** : Utilisation du portail Azure, Azure PowerShell, ou Azure CLI pour déployer des modèles ARM.
- **Paramètres de modèles** : Variables d'entrée qui permettent de personnaliser les déploiements de modèles ARM.
- **Fonctions de modèles** : Fonctions intégrées pour manipuler les valeurs dans les modèles ARM.

### ARM Template Structure

La structure des modèles ARM est composée de plusieurs sections clés :
- **`$schema`** : URI du schéma de modèle ARM.
- **`contentVersion`** : Version du contenu du modèle.
- **`parameters`** : Paramètres d'entrée pour personnaliser les déploiements.
- **`variables`** : Variables utilisées dans le modèle pour simplifier les définitions.
- **`resources`** : Définition des ressources à déployer ou à mettre à jour.
- **`outputs`** : Valeurs de sortie du déploiement, telles que des informations sur les ressources déployées.

### Azure Bicep

Azure Bicep est un langage de déploiement de l'infrastructure en tant que code (IaC) qui simplifie l'écriture de modèles ARM :
- **Syntaxe simplifiée** : Azure Bicep utilise une syntaxe plus concise et plus facile à lire que les modèles ARM JSON.
- **Transpilation vers ARM** : Les fichiers Bicep sont convertis en modèles ARM JSON pour le déploiement.
- **Modularité** : Azure Bicep permet de créer des modules réutilisables pour des composants d'infrastructure.
- **Déploiement** : Utilisation d'Azure CLI pour déployer des fichiers Bicep.
