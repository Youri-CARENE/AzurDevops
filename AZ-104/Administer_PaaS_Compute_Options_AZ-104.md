
## Administer PaaS Compute Options

### Module Introduction

L'administration des options de calcul PaaS dans Azure comprend la gestion des services d'application, des conteneurs et des déploiements continus. Ce module couvre les concepts clés et les meilleures pratiques pour administrer efficacement les services PaaS dans Azure.

### App Service Plans

Les plans de service d'application définissent les ressources et les coûts associés aux applications hébergées dans Azure App Service :
- **Niveaux de plan de service** : Free, Shared, Basic, Standard, Premium, et Isolated.
- **Scalabilité** : Options de mise à l'échelle verticale et horizontale pour ajuster les ressources en fonction des besoins.
- **Performance** : Choisir le plan approprié en fonction des exigences de performance et de coût.

### Deploying App Service

Le déploiement des services d'application implique plusieurs étapes :
- **Création d'une App Service** : Utiliser le portail Azure, Azure CLI, ou Azure PowerShell pour créer une nouvelle instance de service d'application.
- **Déploiement de l'application** : Utiliser FTP, Git, ou des outils de déploiement intégrés pour publier l'application.
- **Configuration des paramètres** : Ajuster les configurations de l'application telles que les chaînes de connexion et les paramètres d'application.

### Securing App Service

La sécurisation des services d'application est cruciale pour protéger les données et les applications :
- **Authentification et autorisation** : Utiliser Azure AD pour authentifier et autoriser les utilisateurs.
- **Certificats SSL/TLS** : Configurer les certificats pour sécuriser les communications.
- **Règles de pare-feu** : Définir des règles de pare-feu pour restreindre l'accès à l'application.

### Custom Domains

Les domaines personnalisés permettent de mapper un domaine spécifique à une application Azure App Service :
- **Ajout d'un domaine personnalisé** : Configurer le DNS pour mapper le domaine au service d'application.
- **Configuration SSL** : Associer des certificats SSL pour sécuriser le domaine personnalisé.

### Backup App Service

La sauvegarde des services d'application assure la récupération en cas de perte de données ou de défaillance :
- **Configuration des sauvegardes** : Planifier et configurer des sauvegardes automatiques de l'application et de la base de données.
- **Restauration** : Utiliser les sauvegardes pour restaurer les applications et les données en cas de besoin.

### CI/CD and Deployment Slots

L'intégration continue et le déploiement continu (CI/CD) automatisent le processus de déploiement des applications :
- **Configuration CI/CD** : Utiliser Azure DevOps, GitHub Actions, ou d'autres outils pour configurer les pipelines CI/CD.
- **Slots de déploiement** : Utiliser des slots de déploiement pour tester les nouvelles versions avant de les mettre en production.

### Azure Container Instances

Azure Container Instances (ACI) permet de déployer des conteneurs directement sur Azure sans gestion d'infrastructure sous-jacente :
- **Déploiement de conteneurs** : Utiliser le portail Azure, Azure CLI, ou des modèles ARM pour déployer des conteneurs.
- **Scalabilité** : Ajuster les ressources des instances de conteneurs en fonction des besoins de l'application.

### Container Groups

Les groupes de conteneurs permettent de déployer plusieurs conteneurs ensemble sur une même hôte logique :
- **Configuration des groupes** : Définir les groupes de conteneurs avec des configurations de réseau et de stockage partagées.
- **Cas d'utilisation** : Scénarios où les conteneurs doivent fonctionner ensemble en étroite collaboration.

### Manage Containers with Azure Container Apps

Azure Container Apps facilite la gestion et le déploiement des conteneurs dans un environnement entièrement géré :
- **Déploiement des applications** : Utiliser le portail Azure ou la CLI pour gérer les applications conteneurisées.
- **Mise à l'échelle automatique** : Configurer des règles pour la mise à l'échelle automatique basée sur la demande.
- **Surveillance et journalisation** : Utiliser les outils intégrés pour surveiller les performances et capturer les journaux.
