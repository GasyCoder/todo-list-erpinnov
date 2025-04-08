# 📋 Liste des Tâches du Projet

## 🖥️ Frontend – Vue.js (avec Vite)

Refonte complète de l’interface utilisateur avec Vue.js :

### Pages et Composants à développer :

- [ ] **Page d’accueil**
  - Récupération des contenus (collaboration avec M. Sylvain)
  - Présentation claire de l’objectif du service
- [ ] **Composant "Plans tarifaires"**
  - Design responsive des cartes de prix
  - Intégration dynamique via API
  - Affichage des avantages par plan
- [ ] **Pages Authentification**
  - Formulaire de **connexion**
  - Formulaire d’**inscription**
  - Confirmation de déconnexion
- [ ] **Pages Légales**
  - Politique de confidentialité
  - Conditions générales d’utilisation
- [ ] **Gestion d’état**
  - Intégration avec Pinia ou autre store pour gérer l’état utilisateur et les plans
- [ ] **Appel API**
  - Connexion sécurisée aux endpoints du backend
- [ ] **UI/UX**
  - Responsive Design
  - Expérience utilisateur fluide

---

## 🧩 Backend – API Laravel

Développement d’une API REST avec Laravel :

### Endpoints Authentification :

- [x] `POST /api/login` – Authentification de l’utilisateur
- [x] `POST /api/register` – Création d’un compte utilisateur
- [x] `POST /api/logout` – Déconnexion
- [x] `GET /api/privacy` – Politique de confidentialité
- [x] `GET /api/terms` – Conditions générales

### Endpoints pour les Plans Tarifaires :

- [ ] `GET /api/plans` – Liste de tous les plans disponibles
- [ ] `GET /api/plans/{id}` – Détails d’un plan spécifique
- [ ] `POST /api/plans` – Création d’un nouveau plan (admin uniquement)
- [ ] `PUT /api/plans/{id}` – Mise à jour d’un plan existant
- [ ] `DELETE /api/plans/{id}` – Suppression d’un plan (admin uniquement)

### Autres tâches backend :

- [ ] Mise en place de la base de données (migrations + seeders)
- [ ] Configuration des règles de validation
- [ ] Protection des routes via Sanctum ou Passport
- [ ] Gestion des rôles (Admin, Utilisateur)
- [ ] Tests unitaires et fonctionnels

---

## ⚙️ Architecture du Projet

- 🔄 **Séparation Frontend / Backend**
  - Frontend : SPA avec Vue.js (consomme l’API via axios ou fetch)
  - Backend : API REST Laravel (serveur indépendant)
- 🔐 Authentification via tokens (Laravel Sanctum)
- 📡 Communication via JSON API

---

> ✨ À venir : Intégration de Stripe ou d’un autre moyen de paiement, Dashboard utilisateur, Interface
