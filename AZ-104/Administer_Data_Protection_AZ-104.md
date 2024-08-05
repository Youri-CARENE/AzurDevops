
## Administer Data Protection

### Module Introduction

L'administration de la protection des données dans Azure comprend l'utilisation de services de sauvegarde et de récupération pour garantir la disponibilité et la durabilité des données. Ce module couvre les outils et les meilleures pratiques pour protéger les données et assurer la continuité des activités.

### Azure Backup

Azure Backup est un service de sauvegarde basé sur le cloud qui protège les données contre les pertes et les corruptions :
- **Fonctionnalités** : Sauvegarde des machines virtuelles, des bases de données, des fichiers et des dossiers.
- **Configuration** : Mise en place de sauvegardes via le portail Azure, Azure CLI ou PowerShell.
- **Restauration** : Procédures pour restaurer les données sauvegardées.

### Azure Backup Center

Azure Backup Center offre une vue unifiée pour gérer les sauvegardes à grande échelle :
- **Tableau de bord centralisé** : Surveillance et gestion des sauvegardes à partir d'un emplacement unique.
- **Gestion des politiques** : Définir et appliquer des politiques de sauvegarde cohérentes.
- **Alertes et notifications** : Configurer des alertes pour les échecs et les succès des sauvegardes.

### File and Folder Backup

La sauvegarde des fichiers et dossiers permet de protéger les données critiques sur les serveurs et les ordinateurs :
- **Configuration des sauvegardes** : Utiliser Azure Backup pour configurer des sauvegardes de fichiers et dossiers.
- **Restauration** : Procédures pour restaurer des fichiers et dossiers spécifiques à partir des sauvegardes.

### Configuring Backup – Azure VM

La configuration des sauvegardes pour les machines virtuelles Azure est essentielle pour protéger les charges de travail critiques :
- **Création de sauvegardes** : Utiliser le service Azure Backup pour configurer des sauvegardes automatiques des VM Azure.
- **Restauration des VM** : Procédures pour restaurer des machines virtuelles à partir des sauvegardes.

### Configuring Backup – Non-Azure VM

Azure Backup peut également être utilisé pour protéger les machines virtuelles non-Azure :
- **Configuration des agents** : Installer et configurer des agents de sauvegarde sur des VM locales ou dans d'autres clouds.
- **Restauration des VM** : Procédures pour restaurer des VM non-Azure à partir des sauvegardes.

### Compare Backup Options

Il existe plusieurs options de sauvegarde dans Azure, chacune adaptée à des scénarios spécifiques :
- **Sauvegarde de fichiers et dossiers** : Pour les données critiques de petite taille.
- **Sauvegarde de machines virtuelles** : Pour protéger les charges de travail complètes.
- **Sauvegarde de bases de données** : Pour les bases de données SQL et autres systèmes de gestion de bases de données.

### Manage Soft Delete

La gestion de la suppression douce protège les données contre les suppressions accidentelles :
- **Activation de la suppression douce** : Configurer Azure Backup pour conserver les données supprimées pendant une période spécifiée.
- **Restauration de données supprimées** : Récupérer les données supprimées pendant la période de rétention.

### Azure Site Recovery

Azure Site Recovery (ASR) assure la continuité des activités en cas de sinistre :
- **Réplication** : Configurer la réplication des machines virtuelles et des applications vers une région secondaire.
- **Basculement** : Procédures pour effectuer un basculement vers le site secondaire en cas de sinistre.
- **Retour arrière** : Procédures pour revenir au site principal après la résolution du sinistre.
