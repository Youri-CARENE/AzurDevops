
# Préparation certification AZ-104

## 1. Tags sur les ressources Azure
- **Tags** sont des paires clé-valeur appliquées aux ressources Azure pour les organiser logiquement.
- **Utilisations des Tags** : Suivi des coûts par département, environnement (prod, dev), propriétaire, etc.
- **Implémentation** : Via le portail Azure, PowerShell (`New-AzTag`), ou Azure CLI.

## 2. Azure AD Conditional Access et MFA
- **Conditional Access** : Politiques qui définissent des conditions pour l'accès aux applications cloud.
- **Multi-Factor Authentication (MFA)** : Exiger une authentification à deux facteurs pour accéder à Azure AD, en particulier pour les Global Administrators.
- **Configuration** : Accès via Azure AD -> Security -> Conditional Access -> New Policy. Exemples : Exiger MFA + appareil joint à Azure AD pour les connexions depuis des emplacements non approuvés.

## 3. Création de machines virtuelles Azure avec des configurations personnalisées
- **Commandes PowerShell** : `New-AzVM` pour créer des VMs avec des configurations spécifiques.
- **Incorporation de certificats** : Utiliser des extensions ou des scripts pour ajouter des autorités de certification lors du provisionnement.

## 4. Options de redondance du stockage Azure
- **Local Redundant Storage (LRS)** : Réplication des données dans un seul datacenter.
- **Geo-Redundant Storage (GRS)** : Réplication dans un datacenter secondaire, en lecture uniquement (RA-GRS).
- **Read-Access Geo-Redundant Storage (RA-GRS)** : Permet de lire les données à partir du secondaire.

## 5. Azure Resource Manager (ARM) Templates
- **ARM Templates** : Fichiers JSON décrivant l'infrastructure nécessaire.
- **Récupération des templates** : Portail Azure -> Resource Group -> Deployments -> Voir et télécharger le template.
- **Exécution** : Déploiement via Azure CLI, PowerShell, ou le portail Azure.

## 6. Availability Sets et Allocation Failure
- **Availability Sets** : Groupes qui répartissent les VMs sur plusieurs fault domains et update domains pour éviter les interruptions simultanées.
- **Fault Domains** : Groupes de ressources qui partagent un même risque de panne matérielle.
- **Update Domains** : Groupes de VMs qui peuvent être mis à jour ou redémarrés en même temps.
- **Allocation Failure** : Résolu en arrêtant toutes les VMs de l’Availability Set avant de les redimensionner.

## 7. Gestion des disques dans Azure
- **Détachement des disques** : Portail Azure -> Disks -> Detach, ou via PowerShell (`Dismount-AzDisk`).
- **Attachement** : Ajouter le disque à une autre VM via le portail ou PowerShell (`Add-AzVMDataDisk`).

## 8. Configuration de Fault Domain et Update Domain
- **PlatformFaultDomainCount** : Définit le nombre de fault domains dans un Availability Set, maximum 3 pour la plupart des régions.
- **PlatformUpdateDomainCount** : Définit le nombre d'update domains, maximum 20.
- **Résilience** : Plus ces nombres sont élevés, meilleure est la tolérance aux pannes et aux mises à jour.

## 9. Automatisation avec PowerShell sur les VMs
- **SetupComplete.cmd** : Fichier batch exécuté à la fin du processus de configuration de Windows.
- **Scripts PowerShell** : Utiliser pour automatiser les configurations post-déploiement. Ex : installation d'applications, configuration réseau.

## 10. Capturer et télécharger des images VMs
- **Generalizing** : Utiliser `sysprep` sur Windows ou dépersonnaliser Linux pour capturer une image.
- **Cmdlet `Add-AzVhd`** : Permet de télécharger un disque dur virtuel (VHD) personnalisé sur un compte de stockage Azure.

## 11. VPN et Virtual Network Peering
- **Virtual Network Peering** : Permet la communication entre deux réseaux virtuels dans la même région ou régions différentes.
- **Site-to-Site VPN** : Connexion VPN permanente entre un réseau local et un réseau Azure.
- **Point-to-Site VPN** : Connexion VPN individuelle d'un poste de travail à un réseau Azure.

## 12. Azure Internal Load Balancer et SQL Server Always On
- **Floating IP** : Active la redirection de l'IP du load balancer vers l'instance SQL Server active dans un groupe Always On.
- **Load Balancer interne** : Utilisé pour distribuer le trafic au sein d'un réseau virtuel, souvent pour des bases de données ou d'autres services backend.

## 13. Configuration d'IP statiques
- **IP statiques** : Doivent être définies manuellement lors de la création ou modifiées via PowerShell (`Set-AzNetworkInterface`).
- **Set-AzureStaticVNetIP** : Cmdlet utilisé pour définir une IP statique sur une VM avant la dépréciation de cette commande au profit de `Set-AzNetworkInterface`.

## 14. Network Security Groups (NSG) et interfaces réseau
- **NSG** : Contrôlent le trafic entrant et sortant des interfaces réseau associées.
- **Configuration** : Créer une NSG, définir des règles, puis l'appliquer à une ou plusieurs interfaces réseau ou sous-réseaux.
- **Interfaces réseau (NIC)** : Gérer les interfaces réseau pour chaque VM, s’assurer que chaque interface possède des règles NSG appropriées.

## 15. Azure Backup et restauration
- **Azure Backup** : Service de sauvegarde et de restauration des VMs. Configure des sauvegardes fréquentes et automatiques.
- **Instant Restore** : Permet de restaurer rapidement des fichiers individuels ou la VM entière à un état antérieur.
- **Scénarios de restauration** : Restauration à partir de la sauvegarde, restauration complète ou partielle.

## 16. Diagnostic de performance avec Azure Monitor
- **Azure Monitor** : Service pour collecter et analyser les métriques des ressources Azure.
- **Utilisation** : Configurer des alertes, visualiser les logs et les métriques pour diagnostiquer les problèmes de performance.

## 17. Gestion des utilisateurs externes dans Azure AD
- **Azure AD B2B** : Permet d'inviter des utilisateurs externes dans Azure AD.
- **New-AzureADMSInvitation** : Cmdlet pour envoyer des invitations B2B à des utilisateurs externes.
- **Importation en masse** : Utiliser des scripts PowerShell pour créer plusieurs utilisateurs à partir de fichiers CSV.
