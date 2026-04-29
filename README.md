# Lab Active Directory

## 📌 Contexte

Projet de lab réalisé dans un environnement virtualisé afin de simuler une infrastructure Active Directory en entreprise.

## 🎯 Objectifs

- Déployer un domaine Active Directory
- Gérer utilisateurs et groupes
- Mettre en place des stratégies de sécurité (GPO)
- Tester l’environnement depuis un poste client

## 🏗️ Architecture

- 1 contrôleur de domaine (Windows Server)
- 1 poste client (Windows 10)
- Domaine : lab.local

## ⚙️ Mise en place

### Active Directory

- Installation et configuration du rôle AD DS
- Création du domaine `lab.local`
- Mise en place des OU (Users, Admins)
- Création et gestion des comptes utilisateurs et groupes

### Stratégies de sécurité (GPO)

- Restriction de l’invite de commande pour limiter l’exécution de scripts et commandes non autorisées  
- Restriction du panneau de configuration pour empêcher les modifications système critiques  
- Politique de mot de passe renforcée (longueur, complexité, expiration)

## 🧪 Tests réalisés

- Connexion avec un utilisateur standard
- Vérification de l’application des GPO
- Accès aux ressources réseau partagées
- Tests de restrictions sur poste client Windows 10

## 🔐 Analyse sécurité

### Vulnérabilités observées

- Utilisation possible de mots de passe faibles sans politique adaptée
- Risques liés à l’élévation de privilèges
- Absence de supervision des événements de sécurité

### Mesures mises en place

- Application de GPO de restriction
- Renforcement de la politique de mots de passe
- Structuration des utilisateurs et groupes par OU

### Améliorations possibles

- Mise en place d’un SIEM pour la centralisation des logs
- Détection des attaques (brute force, comportements anormaux)
- Durcissement avancé de l’infrastructure

## 🚀 Conclusion

Ce projet m’a permis de mettre en pratique la gestion d’un environnement Active Directory complet et d’appliquer les bases de la sécurisation d’un domaine Windows en entreprise.

## ⏭️ Suite logique

Prochaine étape : mettre en place un SIEM dans le lab pour aller vers la détection et la réponse aux incidents.
