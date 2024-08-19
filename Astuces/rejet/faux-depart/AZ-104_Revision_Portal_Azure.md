
# Révision pour la certification AZ-104 : Portail Azure et Notes Diverses

## Portail Azure

- Accédez au portail à l'adresse [portal.azure.com](https://portal.azure.com).

## Azure Cloud Shell

- Permet aux utilisateurs de choisir entre **Bash** et **PowerShell** pour gérer les ressources Azure.
- **Temporaire** : nécessite le montage d'un partage de fichiers Azure existant ou nouveau.
- Offre un éditeur de texte graphique intégré (**Monaco Editor**, open-source).
- **Authentification automatique** : accès facile aux ressources Azure.
- **Déconnexion** après 20 minutes d'inactivité.
- Fonctionne sur un **hôte temporaire** fourni par session et par utilisateur.
- Nécessite un groupe de ressources, un compte de stockage et un partage de fichiers Azure.
- Utilise le **même partage de fichiers** Azure pour Bash et PowerShell.
- Attribué à une machine par compte utilisateur.
- **Persistance** de $HOME via une image de 5 Go stockée dans votre partage de fichiers.
- Permissions définies comme un **utilisateur Linux standard** dans Bash.

## Azure PowerShell

- Disponible dans le cloud via **Azure Cloud Shell** ou localement via **PowerShell** pour Windows, Linux ou macOS.
- Deux modes d'utilisation :
  - **Mode interactif** : entrez manuellement chaque commande.
  - **Mode script** : exécutez un script contenant plusieurs commandes.
- **PowerShell 7.x** : installation possible sur Windows, macOS, et Linux.
  - Sur **macOS** : installation via HomeBrew.
  - Sur **Linux** : installation via les gestionnaires de paquets selon la distribution :
    - Ubuntu & Debian : `apt-get`
    - Red Hat & CentOS : `yum`
    - OpenSUSE : `zypper`
    - Fedora : `dnf`

### Module Az

- Permet de travailler avec diverses fonctionnalités Azure :
  - Conteneurs
  - DNS
  - Event Hub
  - Machine Learning
  - Groupes de ressources
  - Stockage
  - Machines virtuelles (VMs)
  - Et plus encore
- Remplace le module **AzureRM** depuis décembre 2018, mais il est **rétrocompatible**.

## Azure CLI

- Utilisation locale (terminal, invite de commande) ou dans le cloud.
- Deux modes d'utilisation :
  - **Mode interactif** : entrez manuellement chaque commande.
  - **Mode script** : exécutez un script contenant plusieurs commandes.
- Commandes structurées en **groupes** et **sous-groupes** :
  - Les groupes représentent les **services Azure**.
  - Les sous-groupes divisent les commandes en regroupements logiques.
- Recherche de commandes :
  - Exemple : `az find blob`
  - Détails supplémentaires : `az storage blob --help`
  - Redémarrer une VM : `az vm restart -g MyResourceGroup -n MyVm`

## Régions Azure

- Une région est une zone géographique comprenant au moins un centre de données.
- Les centres de données sont **isolés** mais connectés par des réseaux à faible latence.
- Régions offrent :
  - Options de **conformité** et de **résilience**.
  - Flexibilité pour déployer des ressources proches des clients.
  - **Résidence des données**.
- Certains services sont spécifiques à une région ou limités à certaines régions.
- **Paires régionales** : régions jumelées dans la même géographie.
- **Géographie Azure** : zone composée de plusieurs régions Azure.
  - Exemples :
    - États-Unis : East US, Central US, West US, etc.
    - Inde
    - Royaume-Uni

## Terminologie

### Ressource Azure

- Un élément gérable disponible via Azure.
- Exemples de ressources :
  - Machines virtuelles (VMs)
  - Comptes de stockage
  - Bases de données
  - Réseaux virtuels (VNets)
  - Applications web

### Groupe de ressources

- Un conteneur qui contient des ressources liées pour les solutions Azure.
- Permet de gérer les ressources de manière logique pour l'organisation.

### Fournisseur de ressources

- Service qui fournit des ressources à déployer et à gérer via Azure Resource Manager (ARM).
- Exemples :
  - **Microsoft.Compute** : fournit les ressources de machine virtuelle (VM).
  - **Microsoft.Storage** : fournit les ressources de compte de stockage.
  - **Microsoft.Web** : fournit les ressources d'application web.
  - **Microsoft.KeyVault** : stockage des clés et secrets.

### Modèle (Template)

- Fichier JSON définissant une ou plusieurs ressources à déployer dans un groupe de ressources.
- Définit également les **dépendances** entre les ressources.
- Avantages :
  - Déploiement cohérent et répétable.
  - **Syntaxe déclarative** : permet de créer des ressources sans scripts complexes.
  - **Modèles ARM** : exemple de syntaxe déclarative pour déployer l'infrastructure Azure.

