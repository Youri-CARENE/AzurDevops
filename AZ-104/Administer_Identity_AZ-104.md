
## Administer Identity

### Introduction to Microsoft Entra ID

Microsoft Entra ID, anciennement connu sous le nom d'Azure Active Directory (AAD), est un service de gestion des identités et des accès basé sur le cloud. Il permet de gérer les utilisateurs et les groupes, d'assurer la sécurité des identités et d'intégrer les applications pour un accès sécurisé et unifié. Entra ID offre des fonctionnalités d'authentification, de gestion des utilisateurs et de contrôle d'accès qui aident les organisations à sécuriser leurs ressources.

### Microsoft Entra ID concepts

Les concepts clés de Microsoft Entra ID incluent :
- **Identités** : Les objets qui représentent les utilisateurs, les groupes et les appareils.
- **Annuaire** : La structure qui stocke les informations d'identité.
- **Applications** : Les services et les applications qui s'intègrent avec Entra ID pour l'authentification et l'autorisation.
- **Rôles et permissions** : Les mécanismes permettant de contrôler l'accès aux ressources en fonction des rôles attribués.

### Microsoft Entra ID vs Active Directory Domain Services

Microsoft Entra ID et Active Directory Domain Services (AD DS) sont deux solutions de gestion des identités :
- **Entra ID** est basé sur le cloud, conçu pour les applications modernes et les services SaaS. Il offre une gestion des identités pour les utilisateurs internes et externes.
- **AD DS** est basé sur site, adapté pour les environnements d'entreprise traditionnels. Il fournit des services d'authentification et d'autorisation pour les réseaux locaux.

### Microsoft Entra ID Editions

Microsoft Entra ID est disponible en plusieurs éditions :
- **Free** : Offre des fonctionnalités de base pour les petites organisations.
- **Office 365 Apps** : Inclus avec les abonnements Office 365, offrant des fonctionnalités additionnelles pour la gestion des identités Office 365.
- **Premium P1** : Ajoute des fonctionnalités avancées telles que la gestion des identités hybrides et l'accès conditionnel.
- **Premium P2** : Inclut toutes les fonctionnalités de P1, avec des capacités supplémentaires pour la gouvernance des identités et la protection avancée.

### Configure device identities

La configuration des identités des appareils implique l'inscription des appareils dans Entra ID pour une gestion sécurisée. Cela permet de contrôler l'accès aux ressources en fonction de l'état de conformité des appareils. Les étapes incluent :
- **Inscription des appareils** : Enregistrer les appareils dans Entra ID.
- **Configuration des stratégies de conformité** : Définir les règles de conformité pour les appareils.
- **Gestion des appareils** : Superviser et gérer les appareils inscrits pour assurer leur conformité et sécurité.

### User Accounts

La gestion des comptes utilisateurs dans Microsoft Entra ID comprend :
- **Création et gestion des utilisateurs** : Ajouter, modifier et supprimer des utilisateurs.
- **Attribution des licences** : Assigner des licences d'utilisation des services Microsoft.
- **Gestion des groupes** : Organiser les utilisateurs en groupes pour simplifier la gestion des accès.
- **Autorisations et rôles** : Définir les rôles et permissions des utilisateurs pour sécuriser l'accès aux ressources.

### Bulk Operations

Les opérations en masse permettent de gérer un grand nombre d'utilisateurs de manière efficace :
- **Importation CSV** : Utiliser des fichiers CSV pour ajouter ou modifier plusieurs utilisateurs à la fois.
- **Scripts PowerShell** : Automatiser la gestion des utilisateurs avec des scripts PowerShell.
- **Portail Azure** : Utiliser le portail Azure pour effectuer des modifications en masse via l'interface utilisateur.

### Group Accounts

La gestion des comptes de groupe comprend :
- **Création et gestion des groupes** : Ajouter, modifier et supprimer des groupes.
- **Groupes dynamiques** : Créer des groupes dont la composition est déterminée par des règles dynamiques.
- **Attribution des permissions** : Gérer les permissions et accès en fonction des groupes.
- **Stratégies de groupe** : Définir et appliquer des stratégies pour les groupes pour une gestion centralisée des accès.

### Self Service Password Reset (SSPR)

Le Self Service Password Reset permet aux utilisateurs de réinitialiser leur mot de passe de manière autonome :
- **Configuration SSPR** : Activer et configurer SSPR pour les utilisateurs.
- **Méthodes d'authentification** : Définir les méthodes d'authentification (email, SMS, questions de sécurité) pour la réinitialisation de mot de passe.
- **Audit et reporting** : Superviser les activités de réinitialisation de mot de passe et générer des rapports pour la conformité.

### Multi Tenant Environments

La gestion des environnements multi-locataires implique :
- **Gestion des locataires** : Gérer plusieurs locataires Entra ID pour différentes organisations ou départements.
- **Accès inter-locataires** : Configurer l'accès et la collaboration entre les locataires.
- **Sécurité et isolation** : Assurer la sécurité et l'isolation des données entre les locataires pour prévenir les accès non autorisés.
