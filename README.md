# 🐺 La Malédiction du Village (LMDV) 

**Un village, des secrets... et une malédiction.**

![Logo de LMDV](https://maledictionvillage.netlify.app/icons/android-chrome-192x192.png)

![Statut du déploiement](https://img.shields.io/badge/statut-en%20développement-4a637d?style=for-the-badge)
![Plateformes](https://img.shields.io/badge/plateformes-Android%20%7C%20iOS%20%7C%20Web-1b3b2f?style=for-the-badge)

---

## 📚 Sommaire

- [🎮 Présentation](#-présentation)
- [✨ Fonctionnalités](#-fonctionnalités)
- [📝 Liste des rôles](#-liste-des-rôles)
- [🃏 Images déjà créées](#-images-déjà-créées)
- [💰 Rétributions de fin de partie](#-Rétributions-de-fin-de-partie)
- [🎨 Charte graphique](#-Charte-graphique)
- [🚀 Installation](#-installation)
- [🛠️ Technologies utilisées](#-technologies-utilisées)
- [🧪 Développement Flutter](#-développement-flutter)
<!-- - [🤝 Contribution](#-contribution) -->
- [📄 Licence](#-licence)
- [📬 Contact](#-contact)

---

## 📖 Présentation

**La Malédiction du Village** est un jeu de rôle multijoueur dans lequel chaque joueur incarne secrètement un personnage dans un village mystérieux victime d'une malédiction. Bluff, stratégie, alliances, trahisons… Survivrez-vous jusqu'à la fin ?

[Liste des choses à faire](PROJECT.md)

---

## ✨ Fonctionnalités

- 🔄 Rôles secrets attribués aléatoirement à chaque partie
- 🎮 Application Android (et bientôt Web)
- 📡 Synchronisation en temps réel via Firebase Realtime Database
- 🧠 Intelligence artificielle pour remplacer les joueurs manquants
- 🗨️ Chat intégré avec modération automatique
- 🪙 Système de monnaie virtuelle : **Lunaris**
- 📺 Affichage possible sur écran secondaire (TV, projecteur...)

---

## 📝 Liste des rôles

### Voici la liste officielle des rôles dans **La Malédiction du Village** :

| Rôle           | Description brève                                               |
|----------------|----------------------------------------------------------------|
| **Créature de l'ombre** | Prédateur de la nuit, élimine un joueur chaque nuit|
| **Devin**    | Peut découvrir le rôle d’un joueur chaque nuit                 |
| **Protecteur** | Protège un joueur contre une attaque la nuit                   |
| **Ancien**    | Survit à une premiere attaque nocturne. (Ce bouclier peut durer toute la partie) |
| **Messager**  | Crée un chat privé entre deux joueurs pour discuter en secret toute la partie   |
| **La veuve noire**   | Écoute des messages choisis aléatoirement du chat privé du Messager, sans savoir qui parle  |
| **Le Marionnettiste** | Contrôle un joueur chaque nuit, qui sait qu’il est manipulé et qui est obligé de voté le vote du marionnettiste. Ce pouvoir est limité à 2x par partie.|
| **Le Mercenaire** | Peut acheter et utiliser, contre des Lunaris, les pouvoirs des autres rôles pendant la partie. Voir la tarification ci-dessous |
| **Simple Villageois** | Pas de pouvoir partuculier |

(Liste sujette à évolution selon les mises à jour du jeu)

### Tarification du mercenaire :

| Pouvoir / Rôle      | Coût en Lunaris | Commentaire                      |
| ------------------- | ------------ | ----------------------------------- |
| Créature des Ombres | 7500         | Très puissant, influence majeure    |
| Protecteur          | 4000         | Pouvoir défensif, protège un joueur |
| Devin               | 5000         | Découverte d’un rôle, bon impact    |
| Veuve noire         | 3000         | Espionne quelques messages secrets  |
| Marionnettiste      | 7000         | Contrôle temporaire d’un joueur     |

> Rappel : la mercenaire ne peut acheter que 2 pouvoirs dans une partie. Chacun est utilisable une seule fois.

### Fonctions optionnelle votée par le village en début de partie :

| Fonction | Description brève |
| -------- | ----------------- |
| **Régent** | Une seule fois dans la partie, il peut annuler l'exécution du joueur voté par le village. |

---

## 🃏 Images déjà créées

Pour voir les cartes ou graphismes déjà créés, veuillez voir [ce dossier](lib/assets/images).

---

## 💰 Rétributions de fin de partie

À la fin de chaque partie, les joueurs reçoivent des Lunaris selon leurs performances pour encourager la progression et la stratégie :

- 🎁 Cadeau de bienvenue : chaque nouveau joueur reçoit 5000 Lunaris dès la création de son compte.
- 🏆 Récompense à la victoire : les joueurs faisant partie de l’équipe gagnante obtiennent 2500 Lunaris supplémentaires.
- ⏳ Bonus de survie : chaque joueur reçoit 250 Lunaris multipliés par le nombre de manches durant lesquelles il est resté en vie, même s’il a perdu.
  Exemple : un joueur éliminé après 12 manches reçoit 12 × 250 = 3000 Lunaris.

---

## 🎨 Charte graphique

Les couleurs sont les suivantes :
- Arrière plan : `#4a637d`
- Seconde couleur (cardview, bouttons...) : `#1b3d2f`
- Accent : `#a68a00`

Les polices utilisées sont les suivantes :
- Uncial Antiqua pour les titres ([Voir ici](https://fonts.google.com/specimen/Uncial+Antiqua))
- Lora pour le reste ([Voir ici](https://fonts.google.com/specimen/Lora))

Caractéristiques des cardview :
- 7px de rayon
- 5px de marge et de padding
- La couleur d'arrière plan est définie par hiérarchie :
  - Blanc (`#ffffff`) pour celles qui n'ont rien entre elle et l'arrière plan **ou** si elles sont dans des vertes
  - Vert forêt (`#1b3d2f`) pour celles dans des blanches
  - Et ça continue commme ça en boucle

Les icônes utilisées sont celles de la bibliothèque [Material Icons](https://fonts.google.com/icons).

---

## 🚀 Installation

### 📱 Android

1. Télécharger l'APK (à venir)
2. Activer les **sources inconnues** dans les paramètres de votre appareil
3. Installer et lancer l'application

### 🌐 Web

Lancement prévu ici :  
➡️ [https://maledictionvillage.netlify.app](https://maledictionvillage.netlify.app)

---

## 🛠️ Technologies utilisées

- **Flutter** (Android & Web)
- **Firebase Firestore** (sauvegarde & synchro)
- **Firebase Authentication** (email, Discord, Google)
- **Node.js + WebSocket** pour le backend temps réel
- **Netlify** pour l’hébergement de la version Web
- **OAuth 2.0** (connexion sécurisée)
- **Gooogle Gemini** pour les différents systèmes d'intelligence artificielle (faux joueurs, modération du chat, transformation des images de profil)

---



## 🧪 Développement Flutter

L’application Android est développée avec Flutter. Ce système permet de coder une seul fois l'app en dart avant de la compiler dans les languages natifs des plate-formes disponibles (android, IOS, Web, macOS, Windows, Linux, etc...) ce qui est un gain de temps considérable.

---

<!--
## 🤝 Contribution

Tu veux aider ? Bienvenue !
Voici comment contribuer :

- Fork le dépôt
- Crée une branche avec une fonctionnalité (```git checkout -b nouvelle-fonction``` (ou autre chose que "nouvelle-fonction" !))
- Commit (```git commit -am 'Ajout : nouvelle fonctionnalité'```)
- Push (```git push origin nouvelle-fonction```)
- Ouvre une Pull Request

---
-->

## 📄 Licence

Ce projet est protégé par la licence Creative Commons BY-NC-ND 4.0.
Tu es autorisé à consulter, utiliser et partager ce projet, à condition :
- de créditer l’auteur original (Nico)
- de ne pas en faire un usage commercial
- de ne pas modifier ou redistribuer une version modifiée

Voir les détails : [https://creativecommons.org/licenses/by-nc-nd/4.0/](https://creativecommons.org/licenses/by-nc-nd/4.0/)

---

## 📬 Contact

Pour toute question ou suggestion :

- 🌐 Site : [https://maledictionvillage.netlify.app](https://maledictionvillage.netlify.app)
- 📧 Email : [malediction.village@gmail.com](mailto:malediction.village@gmail.com?subject=Contacter%20la%20Malédiction%20du%20Village%20depuis%20le%20README%20Github.com)
- 💬 Serveur Discord (à venir)

---
