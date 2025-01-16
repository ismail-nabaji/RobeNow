# **RobeNow - React Native App** 👗📱

Bienvenue sur **RobeNow**, une application de gestion de location de robes développée avec **React Native**.

## 🛠️ Installation et Configuration de l'Environnement

Avant de commencer, assure-toi d'avoir un environnement de développement **React Native** configuré correctement. Suis le guide officiel jusqu'à l'étape ["Creating a new application"](https://reactnative.dev/docs/environment-setup).

### 1️⃣ **Prérequis**
- **Node.js** (LTS recommandé) → [Télécharger ici](https://nodejs.org/)
- **Yarn** (optionnel mais recommandé)  
  ```bash
  npm install --global yarn
  ```
- **Android Studio** (avec SDK Android installé) → [Télécharger ici](https://developer.android.com/studio)
- **Xcode** (pour iOS) → Installable depuis l'App Store
- **Ruby 3.x** (pour CocoaPods sur iOS)
  ```bash
  brew install rbenv
  rbenv install 3.2.2
  rbenv global 3.2.2
  ```

### 2️⃣ **Cloner le projet**
```bash
git clone https://github.com/VOTRE_REPO/robeNow.git
cd robeNow
```

### 3️⃣ **Installer les dépendances**
```bash
yarn install  # ou npm install
```

### 4️⃣ **Installer les Pods pour iOS**
```bash
cd ios
pod install
cd ..
```

---

## 🚀 Démarrer l'Application

### 1️⃣ **Lancer le serveur Metro**
Metro est le bundler JavaScript qui accompagne React Native.

```bash
yarn start  # ou npm start
```

Laisse **Metro** tourner dans une fenêtre de terminal et ouvre un autre terminal pour exécuter l'application.

### 2️⃣ **Démarrer sur Android**
```bash
yarn android  # ou npm run android
```
📌 **Assure-toi d'avoir un émulateur Android actif** (ou un téléphone branché en USB avec le mode développeur activé).

### 3️⃣ **Démarrer sur iOS** (macOS uniquement)
```bash
yarn ios  # ou npm run ios
```
📌 **Assure-toi que Xcode est installé et qu'un simulateur est ouvert.** Tu peux aussi ouvrir `ios/robeNow.xcworkspace` et lancer l’application depuis Xcode.

---

## 🛠️ **Développement et Modification**

### Modifier le code
1. Ouvre **`App.tsx`** dans ton éditeur de code.
2. Modifie le fichier et **sauvegarde**.
3. L’application se mettra à jour automatiquement via **Fast Refresh**.

### Recharger l’application
- **Android** : Appuie deux fois sur `R` ou utilise `Cmd + M` sur macOS (`Ctrl + M` sur Windows/Linux) pour ouvrir le menu développeur.
- **iOS** : Appuie sur `Cmd + R` dans le simulateur.

---

## 🏗️ **Structure du Projet**
```bash
robeNow/
 ├── android/          # Configuration Android
 ├── ios/              # Configuration iOS
 ├── src/              
 │   ├── components/   # Composants réutilisables
 │   ├── screens/      # Écrans principaux
 │   ├── services/     # Logique métier (API, stockage, etc.)
 │   ├── assets/       # Images, icônes, etc.
 │   ├── App.tsx       # Point d'entrée de l'application
 ├── package.json      
 ├── README.md
 ├── .gitignore
 ├── babel.config.js
 ├── metro.config.js
 └── tsconfig.json
```

---

## 🛠️ **Dépannage**
### ❌ Erreur "Unable to open base configuration reference file"
➡️ **Solution** :
```bash
cd ios
rm -rf Pods Podfile.lock
pod install
cd ..
```

### ❌ Erreur CocoaPods sur Mac M1/M2
➡️ Essaye :
```bash
arch -x86_64 pod install
```

### ❌ Erreur lors de l’installation des dépendances ?
```bash
rm -rf node_modules
yarn install
```

### ❌ Autres problèmes ?
Utilise :
```bash
npx react-native doctor
```
Et consulte la documentation officielle :  
[https://reactnative.dev/docs/troubleshooting](https://reactnative.dev/docs/troubleshooting)

---

## 📚 **Ressources**
- [React Native Docs](https://reactnative.dev/docs/getting-started)
- [CocoaPods](https://cocoapods.org/)
- [rbenv](https://github.com/rbenv/rbenv)
- [Android Developer](https://developer.android.com/studio)

---

## 📜 **Licence**
Ce projet est sous licence **MIT**. Libre à toi de l'utiliser et de l'améliorer ! 🎉

---

## 🎉 **Félicitations !**
Tu as maintenant un environnement React Native prêt à l’emploi pour **RobeNow**. 🚀 Bon développement ! 🎨✨
