
# Barb’or Guyane – Système de prise de rendez-vous

Ce projet comprend un **site de réservation complet**, avec un frontend Flutter Web, un backend Node.js sécurisé, et une interface admin. Il est **bilingue (FR/EN)**.

## Fonctionnalités principales

1. **Frontend Flutter Web** :
   - Sélection de service
   - Choix de l'heure
   - Saisie des informations clients
   - Confirmation de RDV

2. **Backend Node.js** :
   - API Express sécurisée
   - Stockage des RDV dans MongoDB
   - Authentification admin via JWT
   - Protection des routes d'administration

3. **Interface Admin** :
   - Gestion des services et horaires
   - Vue calendrier des RDV
   - Authentification admin avec mot de passe sécurisé

4. **Bilingue** :
   - L'application est disponible en français et anglais, selon la préférence de l'utilisateur.

5. **Extras (optionnels)** :
   - Intégration Stripe pour les paiements en ligne
   - Emails de confirmation via EmailJS

---

## Installation et déploiement

1. **Backend (API Node.js)** :
   - Allez dans le dossier `api_barber/`
   - Installez les dépendances : `npm install`
   - Configurez votre MongoDB avec une URL valide dans le fichier `.env`
   - Démarrez le serveur avec : `node index.js`

2. **Frontend (Flutter Web)** :
   - Ouvrez le dossier `flutter_barber_app/`
   - Installez Flutter si ce n’est pas déjà fait
   - Lancez `flutter pub get` puis `flutter run -d chrome`

---

## Déploiement
- Hébergez le backend sur un service comme **Render** ou **Heroku**
- Déployez l'application Flutter sur **Firebase Hosting** ou un autre service compatible

---

### Sécurisation :
Toutes les routes admin sont protégées avec **JSON Web Tokens (JWT)** et toutes les données sont validées avant d’être stockées.

Bon développement !
