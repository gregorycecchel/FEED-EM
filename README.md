# FEED'EM 🍔

Application mobile de swipe pour découvrir des restaurants et leurs plats, inspirée de Tinder.

## Fonctionnalités

### 🎯 Fonctionnalités principales
- ✨ Swipe sur des photos de plats
- ❤️ Like pour voir l'adresse du restaurant
- ❌ Pass pour passer au plat suivant
- 📍 Affichage de l'adresse complète lors d'un like
- ⭐ Système de notation et avis pour chaque restaurant

### 👤 Profil & Social
- 🔐 Authentification utilisateur
- 👥 Système de followers/following
- 💬 Messagerie entre utilisateurs
- 🔔 Notifications en temps réel
- 📸 Partage de photos
- 🔍 Recherche d'utilisateurs

### 🌍 Localisation
- 📍 Géolocalisation automatique
- 🏙️ Sélection de ville
- 🗺️ Restaurants de Nice intégrés

### 💎 Premium
- 👑 Fonctionnalités premium
- 💳 Système de paiement intégré
- ❤️ Likes illimités (vs limite gratuite)

### 🌐 Internationalisation
- 🇫🇷 Français
- 🇬🇧 Anglais
- 🌙 Mode sombre/clair

## Technologies

- **Framework :** React Native avec Expo SDK 54
- **Langage :** TypeScript
- **Navigation :** React Native Screens
- **Animations :** React Native Reanimated
- **Gestes :** React Native Gesture Handler
- **Stockage :** AsyncStorage
- **Images :** Expo Image & Image Picker
- **Localisation :** Expo Location
- **Icônes :** Expo Vector Icons

## Structure du projet

```
├── App.tsx                      # Point d'entrée
├── eas.json                     # Configuration EAS Build
├── src/
│   ├── components/
│   │   ├── FoodCard.tsx         # Carte de plat avec swipe
│   │   ├── FoodSwiper.tsx       # Gestionnaire de swipe
│   │   ├── Logo.tsx             # Logo FEED'EM
│   │   ├── ReviewModal.tsx      # Modal d'avis
│   │   └── UsernameText.tsx     # Affichage nom utilisateur
│   ├── context/
│   │   ├── LanguageContext.tsx  # Gestion multilingue
│   │   └── ThemeContext.tsx     # Thème sombre/clair
│   ├── data/
│   │   ├── foodData.ts          # Données de test
│   │   ├── foodTags.ts          # Tags des plats
│   │   └── real-restaurants-nice.json  # Restaurants de Nice
│   ├── screens/
│   │   ├── AuthScreen.tsx       # Connexion/Inscription
│   │   ├── FeedScreen.tsx       # Feed principal (swipe)
│   │   ├── FollowListScreen.tsx # Liste followers/following
│   │   ├── HomeScreen.tsx       # Accueil
│   │   ├── LikedRestaurantsScreen.tsx  # Favoris
│   │   ├── LocationSelectScreen.tsx    # Sélection ville
│   │   ├── MessagesScreen.tsx   # Messagerie
│   │   ├── NotificationsScreen.tsx     # Notifications
│   │   ├── ProfileScreen.tsx    # Profil utilisateur
│   │   ├── PublicProfileScreen.tsx     # Profil public
│   │   ├── SharedPhotosScreen.tsx      # Photos partagées
│   │   └── UserSearchScreen.tsx # Recherche utilisateurs
│   ├── services/
│   │   ├── activityService.ts   # Activité utilisateur
│   │   ├── authService.ts       # Authentification
│   │   ├── cityService.ts       # Gestion des villes
│   │   ├── followService.ts     # Système follow
│   │   ├── geocodingService.ts  # Géocodage
│   │   ├── likeLimitService.ts  # Limite de likes
│   │   ├── locationService.ts   # Localisation
│   │   ├── messageService.ts    # Messagerie
│   │   ├── notificationService.ts      # Notifications
│   │   ├── paymentService.ts    # Paiements
│   │   ├── postService.ts       # Publications
│   │   ├── premiumService.ts    # Abonnement premium
│   │   ├── restaurantProposalService.ts  # Propositions
│   │   ├── reviewService.ts     # Avis/Notes
│   │   └── suggestionService.ts # Suggestions
│   └── types/
│       ├── message.ts           # Types messagerie
│       ├── notification.ts      # Types notifications
│       ├── post.ts              # Types publications
│       ├── review.ts            # Types avis
│       └── user.ts              # Types utilisateur
├── assets/
│   └── feedem_logo.svg          # Logo vectoriel
```

## Prochaines étapes

- [ ] Intégration API Google Places
- [ ] Notifications push
- [ ] Mode hors-ligne
- [ ] Partage sur les réseaux sociaux
- [ ] Filtres avancés (cuisine, prix, distance)
- [ ] Réservation de table

## Licence

Projet privé - Tous droits réservés.
