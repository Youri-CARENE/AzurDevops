
# Mon guide de Révision pour l'Examen AZ-104

---

## 1. Comprendre Microsoft Entra ID

### Microsoft Entra ID :
- **Définition** : Un service d'identité et d'accès basé sur le cloud, anciennement appelé Azure AD.
- **Fonctionnalités principales** :
  - Gestion des identités : Utilisation pour gérer les identités des utilisateurs dans un environnement cloud.
  - Authentification multifactorielle (MFA) : Sécurise les connexions en demandant plusieurs formes de vérification.
  - Accès conditionnel : Contrôle l'accès aux applications en fonction de conditions spécifiques (emplacement, appareil, etc.).

### Comparaison avec Active Directory Domain Services (AD DS) :
- **AD DS** : Traditionnellement utilisé pour les réseaux d'entreprises on-premises.
- **Entra ID** : Optimisé pour les environnements cloud avec une meilleure gestion des identités décentralisées.

### Plans P1 et P2 de Microsoft Entra ID :
- **Plan P1** : Basique, couvre la plupart des besoins, y compris MFA, l'accès conditionnel et la gestion d'identités.
- **Plan P2** : Inclut tout de P1 + outils avancés pour la détection des menaces et la protection basée sur le risque.

### Microsoft Entra Domain Services :
- **Fonctionnalités** : Simule les services de domaine d'Active Directory dans le cloud. Permet de gérer des appareils joints au domaine sans infrastructure on-premises.

---

## 2. Configurer des Comptes d’Utilisateurs et de Groupes

### Création et Gestion de Comptes Utilisateurs :
- **Individuellement** : Via le portail Azure, navigation vers **Azure Active Directory > Utilisateurs > Nouvel utilisateur**.
- **En bloc** : Utiliser des fichiers CSV pour importer plusieurs utilisateurs simultanément. Commandes PowerShell disponibles pour automatiser la gestion.

### Création de Groupes :
- **Types de groupes** : 
  - Groupes de sécurité : Pour contrôler l'accès aux ressources.
  - Groupes Microsoft 365 : Pour la collaboration (emails, fichiers partagés).
- **Création** : Dans **Azure AD > Groupes > Nouveau groupe**.

### Unités Administratives :
- **Utilité** : Diviser les utilisateurs et ressources pour déléguer la gestion à des administrateurs spécifiques.
- **Création** : Via **Azure AD > Unités administratives > Nouvelle unité administrative**.

### Simulation de Labo :
- **Pratique recommandée** : Effectuez des opérations de création et de gestion dans un environnement de test pour solidifier vos connaissances.

---

## 3. Configurer des Abonnements

### Créer et Gérer des Abonnements :
- **Obtenir un abonnement** : Via le portail Azure sous **Gestion des abonnements**.
- **Régions Azure** : Comprendre les régions pour optimiser la latence et les coûts.

### Gestion des Coûts :
- **Microsoft Cost Management** : 
  - **Suivi des coûts** : Analyser les coûts via des rapports.
  - **Alertes de coûts** : Configurer des alertes pour éviter les dépassements de budget.

### Étiquetage des Ressources :
- **Objectif** : Organiser les ressources pour une gestion efficace.
- **Comment faire** : Dans **Azure Portal > Ressources > Étiquettes**. Ajouter des paires clé/valeur.

---

## 4. Configurer Azure Policy

### Implémentation de Stratégies Azure :
- **Création de Stratégies** : Utiliser **Azure Policy > Définition de stratégie > Créer une définition**.
- **Scénarios d’utilisation** : Conformité aux réglementations, gestion des configurations sécuritaires.

### Définitions de Stratégies et Initiatives :
- **Définitions** : Une politique unique définissant une règle spécifique.
- **Initiatives** : Un regroupement de plusieurs stratégies pour gérer des ensembles de règles complexes.

### Délimitation et Conformité :
- **Étendue** : Appliquer les politiques à des groupes de ressources ou à des abonnements spécifiques.
- **Conformité** : Utiliser les rapports de conformité pour vérifier que toutes les ressources adhèrent aux politiques.

---

## 5. Configurer le Contrôle d’Accès en Fonction du Rôle (RBAC)

### Implémentation de RBAC :
- **Concept** : Contrôle granulé des accès aux ressources, basé sur les rôles attribués aux utilisateurs.
- **Création de Rôles** :
  - **Définition personnalisée** : Dans **Azure AD > Rôles > Créer un rôle personnalisé**.
  - **Attribution de rôles** : Assigner des rôles à des utilisateurs ou groupes sous **Contrôle d’accès (IAM)**.

### Comparaison entre Rôles Azure et Microsoft Entra :
- **Rôles Azure** : Spécifiques aux services Azure (VM, stockage, etc.).
- **Rôles Microsoft Entra** : Concernent la gestion des identités et l'accès à Entra ID.

---

## 6. Créer des Utilisateurs et des Groupes Azure dans Microsoft Entra ID

### Création d’Utilisateurs dans Microsoft Entra ID :
- **Processus** : Suivez la même méthode que pour la création d’utilisateurs dans Azure AD.

### Gestion des Groupes et des Comptes Invités B2B :
- **Groupes** : Utilisez les groupes pour gérer l’accès aux ressources.
- **Comptes Invités B2B** : Permettre à des partenaires externes d’accéder à des ressources spécifiques tout en gardant un contrôle strict.

---

## 7. Sécuriser vos Ressources Azure avec Azure RBAC

### Gestion de l’Accès :
- **Lister et Accorder des Accès** : Utilisez le portail Azure pour voir qui a accès à quelles ressources et ajuster les permissions si nécessaire.
- **Journaux d’Activité** : Consultez ces journaux pour auditer les changements de rôles et accès.

---

## 8. Réinitialisation de Mot de Passe en Libre-Service (SSPR)

### Implémentation SSPR :
- **Objectif** : Permettre aux utilisateurs de réinitialiser leurs mots de passe sans intervention du support.
- **Configurer SSPR** : Sous **Azure AD > Réinitialisation de mot de passe**. Choisir les options de validation (questions de sécurité, MFA, etc.).

### Personnalisation et Test :
- **Personnalisation** : Adapter l’apparence et les notifications pour correspondre à la marque de l'entreprise.
- **Test** : Valider le bon fonctionnement en simulant des scénarios de réinitialisation.

---

## Conseils de Révision
- **Pratique active** : Faites des exercices pratiques dans un environnement de labo.
- **Mémorisation des concepts clés** : Comprenez et mémorisez les différences entre les services similaires comme AD DS et Entra ID.
- **Concentration sur les simulations de labo** : Elles constituent une part importante de l'examen pratique et théorique.
- **Révision des modules** : Relisez les sections importantes et utilisez des fiches de révision pour les notions complexes comme les rôles RBAC et Azure Policy.

---
