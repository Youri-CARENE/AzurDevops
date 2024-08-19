
# Révision pour la certification AZ-104 : Déployer et gérer les ressources de calcul Azure

## Automatiser le déploiement de ressources à l'aide de modèles ARM ou de fichiers Bicep

### Azure Resource Manager (ARM)
Azure Resource Manager (ARM) vous permet de gérer les ressources de votre solution en tant que groupe, plutôt que de les traiter comme des composants individuels. ARM fournit des outils pour déployer, mettre à jour ou supprimer des ressources de manière cohérente.

- **Déployer, mettre à jour ou supprimer** toutes les ressources d'une solution en une seule opération.
- **Utiliser des modèles** pour déployer des environnements de test, de staging et de production.
- Fournit des fonctionnalités de **sécurité**, **audit** et **balisage** pour gérer les ressources après leur déploiement.
- Permet de **surveiller** toutes les ressources de votre solution.
- **Répétabilité** : déployer des solutions de manière répétée tout au long du cycle de développement en garantissant une cohérence.
- **RBAC** : les rôles peuvent être appliqués à tous les services au sein d'un groupe de ressources.
- **Balisage** : organiser logiquement les ressources et suivre les coûts par balise.

### Modèles ARM
Les modèles ARM sont des documents JSON écrits en syntaxe déclarative.

- **Consistance** : les modèles ARM garantissent que la structure et les expressions sont cohérentes, quel que soit l'outil utilisé.
- **Modularité** : les modèles peuvent être liés pour créer des solutions complexes.
- **Réutilisation** : les modèles peuvent utiliser des paramètres pour personnaliser les déploiements.
- **Orchestration** : déployer plusieurs ressources dans le bon ordre.

#### Schéma des modèles ARM
Les modèles ARM utilisent des paires clé-valeur pour définir les paramètres suivants :

- **$schema** : localisation du fichier de schéma JSON (obligatoire).
- **contentVersion** : version du modèle (obligatoire).
- **parameters** : valeurs pour personnaliser le déploiement (facultatif, max 256).
- **variables** : fragments JSON pour simplifier les expressions (facultatif).
- **functions** : fonctions définies par l'utilisateur (facultatif).
- **resources** : types de ressources déployées ou mises à jour (obligatoire).
- **outputs** : valeurs retournées après le déploiement (facultatif).

### Modèles Bicep
Bicep est un langage spécifique au domaine (DSL) qui simplifie la création de modèles ARM.

- **Syntaxe simple** : plus facile à lire et écrire que JSON.
- **Référence directe** : les paramètres et variables peuvent être référencés directement.
- **Dépendances automatiques** : Bicep détecte automatiquement les dépendances entre ressources.
- **Validation des types et IntelliSense** : fourni par l'extension Bicep dans Visual Studio Code.
- **Modules** : possibilité de décomposer les modèles en modules plus petits et réutilisables.

## Créer et configurer des machines virtuelles

### Machines virtuelles Azure
Les machines virtuelles (VM) fournissent une infrastructure en tant que service (IaaS), permettant de contrôler le système d'exploitation, le stockage, et les configurations réseau.

- **IaaS** : infrastructure informatique instantanée provisionnée et gérée via le web.
- **Scalabilité** : les VM peuvent être mises à l'échelle en fonction des besoins.
- **Responsabilité partagée** : la configuration et la maintenance des VM sont partagées entre Microsoft et le client.

#### Checklist pour la configuration d'une VM
1. **Configuration réseau** : utiliser des VNets pour une connectivité privée.
2. **Nom de la VM** : choisir une convention de nommage standardisée.
3. **Emplacement de la VM** : choisir la région en fonction des utilisateurs et des exigences de conformité.
4. **Taille de la VM** : déterminer la taille en fonction de la charge de travail.
5. **Modèle de tarification** : évaluer les coûts basés sur le calcul et le stockage.
6. **Système d'exploitation** : choisir entre Windows et Linux.
7. **Stockage Azure** : utiliser des disques gérés Azure pour le stockage.
8. **Disques de la VM** : comprendre les types de disques (OS, temporaire, données).

#### Considérations supplémentaires pour le stockage
- **Stockage Premium** : recommandé pour les charges de travail intensives en IOPS.
- **Disques gérés** : abstraction des blobs de pages, des conteneurs de blobs et des comptes de stockage Azure.

## Ensembles de disponibilité et zones de disponibilité

### Ensembles de disponibilité
- **Regroupement logique** : les VM dans un ensemble de disponibilité sont protégées contre les pannes matérielles et logicielles.
- **Domaines de mise à jour (UD)** : groupes de VM pouvant être redémarrés en même temps.
- **Domaines de défaillance (FD)** : groupes de VM partageant le même matériel et point de défaillance.

### Zones de disponibilité
- **Protection contre les pannes de centre de données** : déploiement de VM dans différentes zones pour améliorer la disponibilité.
- **Services zonaux** : ressources associées à une zone spécifique.
- **Services redondants par zone** : répliquent les applications et données à travers les zones.

## Mise à l'échelle des machines virtuelles

### Mise à l'échelle verticale
- **Augmenter/diminuer la taille de la VM** : ajuster les ressources matérielles en réponse à la charge de travail.

### Mise à l'échelle horizontale
- **Augmenter/diminuer le nombre de VM** : ajuster le nombre de VM pour répondre aux besoins changeants.

### Ensembles de machines virtuelles à échelle automatique (VMSS)
- **Déploiement et gestion d'un ensemble de VM identiques** : permet une scalabilité automatique.
- **Supporte jusqu'à 1 000 instances de VM** : idéal pour les charges de travail intensives.
- **Autoscaling** : ajustement automatique du nombre d'instances en fonction de la demande.

## Provisionner et gérer des conteneurs dans le portail Azure

### Registre de conteneurs Azure
- **Créer et gérer** un registre pour stocker et gérer des images de conteneurs.

### Azure Container Instances (ACI) et Azure Container Apps
- **Déploiement et gestion des conteneurs** : utiliser ACI pour déployer des conteneurs de manière simple et rapide.
- **Mise à l'échelle des conteneurs** : ajuster la taille et le nombre de conteneurs pour répondre aux besoins de l'application.

## Créer et configurer un service d'application Azure

### Plans de service d'application Azure
- **Ressources de calcul dédiées** : définir les ressources pour exécuter des applications web.
- **Mise à l'échelle** : options pour la mise à l'échelle verticale et horizontale.

### Azure App Services
- **Création de backends mobiles, sites web, et API web** : s'exécute facilement sur des environnements Linux et Windows.
- **Intégration DevOps** : support pour GitHub, Azure DevOps, Docker Hub, etc.

### Déploiement d'applications avec App Service
- **Configuration** : paramètres de déploiement, mappage de chemin, Always On, affinité ARR.
- **Sécurité** : support intégré pour l'authentification et l'autorisation.

### Noms de domaines personnalisés
- **Mapping de domaines personnalisés** : possibilité de réserver et mapper des domaines à des applications web pour les environnements de production.

