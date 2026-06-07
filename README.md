# 📱 Telegram Chat — Application Android

Application de chat instantané développée avec **Android Studio**, **Java** et **Firebase**, entièrement en français.

---

## 🛠️ Technologies utilisées

- **Android Studio** — IDE de développement Android
- **Java** — Langage de programmation principal
- **Firebase Authentication** — Connexion via code OTP (SMS)
- **Firebase Realtime Database** — Messagerie en temps réel
- **Cloud Firestore** — Stockage des profils et chaînes
- **Firebase Cloud Messaging** — Notifications push

---

## 📸 Captures d'écran

### 1. Écran de démarrage
![Écran de démarrage](screenshots/splash_screen.png)

Écran de chargement animé avec le logo Telegram Chat et la barre de progression.

---

### 2. Connexion par OTP
![Connexion OTP](screenshots/connexion_otp.png)

Saisie du numéro de téléphone avec sélecteur de pays. Un code OTP est envoyé par SMS via Firebase Phone Auth.

---

### 3. Sélection du pays
![Sélection du pays](screenshots/selection_pays.png)

Liste complète des pays avec drapeaux, indicatifs téléphoniques et barre de recherche rapide.

---

### 4. Liste des conversations
![Liste des conversations](screenshots/liste_chats.png)

Vue principale affichant toutes les conversations récentes avec aperçu du dernier message et heure d'envoi.

---

### 5. Messagerie en temps réel
![Messagerie](screenshots/messagerie.png)

Interface de chat avec bulles de messages, horodatage et indicateurs de lecture (✓✓).

---

### 6. Mes chaînes
![Mes chaînes](screenshots/mes_chaines.png)

Gestion des chaînes publiques suivies avec section de découverte et bouton **Suivre**.

---

### 7. Créer une chaîne — Dialogue
![Créer une chaîne](screenshots/creer_chaine_dialogue.png)

Fenêtre modale pour créer une chaîne publique visible et rejoignable par tous les utilisateurs.

---

### 8. Formulaire — Chaîne publique
![Formulaire chaîne](screenshots/creer_chaine_formulaire.png)

Configuration de la chaîne : nom, description, lien public (`t.me/`), visibilité et catégorie.

---

### 9. Paramètres — Notifications
![Notifications](screenshots/notifications.png)

Contrôle des alertes : messages privés, groupes, mentions, chaînes, son, vibration et mode Ne pas déranger.

---

### 10. Paramètres généraux
![Paramètres](screenshots/parametres.png)

Gestion du profil, confidentialité, appareils connectés, thème sombre, langue et taille du texte.

---

## ✨ Fonctionnalités

- 🔐 Authentification par numéro de téléphone (OTP via SMS)
- 💬 Messagerie instantanée avec indicateurs de lecture
- 📡 Création et abonnement à des chaînes publiques
- 🌍 Sélecteur de pays avec tous les indicatifs internationaux
- 🔔 Notifications push personnalisables
- 🌙 Thème sombre intégré
- 🇫🇷 Interface entièrement en français
- ⚙️ Paramètres complets (confidentialité, stockage, appareils)

---

## ⚙️ Installation

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/votre-repo/telegram-chat-fr.git
   ```

2. **Créer un projet Firebase**  
   Rendez-vous sur [console.firebase.google.com](https://console.firebase.google.com) et activez :
   - Authentication (téléphone)
   - Realtime Database
   - Cloud Firestore

3. **Ajouter `google-services.json`**  
   Téléchargez le fichier de configuration et placez-le dans le dossier `app/`.

4. **Synchroniser Gradle**  
   Ouvrez le projet dans Android Studio :
   ```
   File → Sync Project with Gradle Files
   ```

5. **Lancer l'application**  
   Connectez un appareil Android ou lancez un émulateur, puis appuyez sur **Run ▶** (`Shift + F10`).

---

## 📁 Structure du projet

```
app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/telegramchat/
│   │   │       ├── activities/
│   │   │       ├── adapters/
│   │   │       ├── models/
│   │   │       └── utils/
│   │   └── res/
│   │       ├── layout/
│   │       ├── drawable/
│   │       └── values/
│   └── google-services.json
├── build.gradle
└── AndroidManifest.xml
```

---

## 📄 Licence

Ce projet est distribué sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.
