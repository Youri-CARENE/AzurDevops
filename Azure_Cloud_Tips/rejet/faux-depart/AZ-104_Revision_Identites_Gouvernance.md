
# Révision pour la certification AZ-104 : Gérer les identités Azure et la gouvernance

## Gérer les objets Azure AD

### Créer des utilisateurs et des groupes
- Créer des utilisateurs et des groupes dans Azure AD via le portail ou via des scripts PowerShell/CLI.
- Les utilisateurs peuvent être créés en tant qu'utilisateurs natifs Azure AD ou invités.
- Les groupes peuvent être statiques ou dynamiques, selon les besoins de l'organisation.

### Gérer les licences dans Azure AD
- Gérer les licences via le portail Azure AD.
- Comprendre les états des licences : **Total**, **Attribué**, **Disponible**, **Expirant bientôt**.
- Assigner des licences aux utilisateurs ou groupes en fonction de leur localisation.
- Modifier ou supprimer des plans de licence ; noter que les licences héritées ne peuvent être supprimées directement.

### Créer des unités administratives
- Les unités administratives permettent de déléguer la gestion d'Azure AD à différents administrateurs selon des critères organisationnels spécifiques.
- Ajouter des utilisateurs ou groupes à ces unités et configurer des permissions spécifiques.

### Gérer les propriétés des utilisateurs et des groupes
- Modifier les propriétés des utilisateurs et des groupes via le portail ou des scripts.
- Gérer les attributs tels que les informations de contact, les rôles assignés, et les unités administratives.

### Gérer les paramètres des appareils et l'identité des appareils
- Configurer et gérer les types d'appareils connectés à Azure AD :
  - Appareils **enregistrés** dans Azure AD.
  - Appareils **rejoints** à Azure AD.
  - Appareils **rejoints en mode hybride** à Azure AD.
- Configurer des politiques pour gérer l'accès des appareils en fonction de leur statut dans Azure AD.

### Effectuer des mises à jour en masse
- Utiliser des fichiers CSV ou des scripts pour la gestion en masse des utilisateurs et groupes.
- Les tâches en masse nécessitent des privilèges d'administrateur global ou d'administrateur utilisateur.

### Gérer les comptes invités
- Gérer l'ajout, la suppression, et les permissions des comptes invités dans Azure AD.
- Les comptes invités permettent la collaboration avec des utilisateurs externes tout en contrôlant leur accès aux ressources.

### Configurer la réinitialisation de mot de passe en libre-service (SSPR)
- Activer la réinitialisation de mot de passe en libre-service (SSPR) pour permettre aux utilisateurs de réinitialiser leurs mots de passe sans intervention administrative.
- Configurer les méthodes d'authentification pour SSPR : **SMS**, **E-mail**, **Code de sécurité**, **Questions de sécurité**.

## Azure Active Directory (Azure AD)

Azure AD est le service d'annuaire et de gestion des identités (IAM) basé sur le cloud de Microsoft, supportant l'accès aux ressources internes, cloud, et externes.

### Fonctionnalités d'Azure AD
- **Authentification unique (SSO)** : Permet aux utilisateurs d'accéder à plusieurs applications avec une seule authentification.
- **Réinitialisation de mot de passe en libre-service (SSPR)** : Réinitialisation de mot de passe sans contact avec le service d'assistance.
- **Authentification multifacteur (MFA)**, **politiques d'accès conditionnel**, et **gestion des accès basée sur les groupes**.
- **Extensibilité cloud** : Prend en charge les environnements multi-locataires.
- **Support universel des appareils** : Fonctionne avec iOS, macOS, Windows, Android.

### Termes Azure AD
- **Identité** : Un objet pouvant être authentifié, comme un utilisateur, une application, ou un service.
- **Compte** : Une identité avec des données associées, stockée dans Azure AD.
- **Locataire Azure** : Instance unique d'Azure AD, représentant une organisation.
- **Abonnement Azure** : Lié à un locataire, utilisé pour payer les services Azure.
- **Identité cloud** : Compte utilisateur défini uniquement dans Azure AD.
- **Identité synchronisée** : Comptes utilisateurs définis dans un AD local et synchronisés avec Azure AD.
- **Utilisateur invité** : Comptes utilisateurs définis en dehors d'Azure, permettant la collaboration externe.

### Active Directory Domain Services (AD DS) comparé à Azure AD
- **AD DS** : Active Directory traditionnel déployé sur des serveurs physiques ou virtuels. Utilise des services tels que **AD CS**, **AD LDS**, **AD FS**, et **AD RMS**.
- **Azure AD** : Solution d'identité pour les applications cloud, offrant une gestion simplifiée des identités avec des fonctionnalités avancées.

### Plans Azure AD
- **Azure AD Free** : Gestion de l'identité de base, SSO illimité, collaboration B2B.
- **M365 Apps** : Inclut IAM de base pour les applications M365.
- **Premium P1** : Gestion avancée des groupes, accès conditionnel, SSPR pour utilisateurs locaux.
- **Premium P2** : Protection et gouvernance des identités avec **PIM** et **JIT**.

## Gérer les abonnements Azure et la gouvernance

### Gérer les rôles d'accès basés sur les rôles (RBAC)
- Créer et gérer des rôles RBAC personnalisés et interpréter les affectations d'accès.
- **Niveaux de scope RBAC** : 
  - **Groupe de gestion**
  - **Abonnement**
  - **Groupe de ressources**
  - **Ressource**

### Gérer les politiques Azure
- Configurer des politiques pour s'assurer que les ressources respectent les exigences de conformité.
- Gérer la conformité et les non-conformités via des tableaux de bord dédiés.

### Gérer les groupes de ressources et de gestion
- Utiliser des groupes de ressources pour organiser logiquement les ressources Azure.
- Utiliser des groupes de gestion pour regrouper des abonnements et appliquer des politiques globales.

### Verrous de ressources
- **Supprimer** : Empêche la suppression des ressources.
- **Lecture seule** : Empêche la modification ou la suppression des ressources.

### Tags sur les ressources
- Utiliser des tags pour organiser et suivre les ressources Azure. Limite de 50 paires nom-valeur par ressource.

