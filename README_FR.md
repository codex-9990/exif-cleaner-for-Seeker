# Exif Cleaner for Seeker

Un nettoyeur de métadonnées photo léger conçu pour les utilisateurs soucieux de l'OpSec (sécurité opérationnelle) et de la confidentialité.

[English](README.md) | [日本語](README_JA.md) | [Français](README_FR.md) | [Deutsch](README_DE.md) | [Italiano](README_IT.md) | [Español](README_ES.md) | [繁體中文](README_TW.md) | [简体中文](README_CN.md) | [한국어](README_KO.md) | [العربية](README_AR.md)

Cette application supprime les métadonnées identifiantes de vos photos **localement sur votre appareil**, avant de les partager sur des plateformes comme X ou Discord.

**Pas de suivi. Pas de téléchargement. Entièrement hors ligne.**

---

## ✨ Fonctionnalités

- **Suppression des données de localisation (GPS)**
- **Suppression des identifiants de l'appareil et de la caméra**
- **Suppression des balises logicielles** telles que "Taken on Seeker"
- **Traitement hors ligne** (aucun téléchargement réseau)
- **Pas d'analyses, pas de traceurs**
- **Support multilingue :** Anglais, Japonais, Français, Allemand, Italien, Espagnol, Chinois (Traditionnel/Simplifié), Coréen, Arabe
- **Mode sombre :** Entièrement pris en charge

---

## 🔐 Pourquoi cela existe-t-il ?

Les photos contiennent souvent des métadonnées cachées qui peuvent révéler :
- où elles ont été prises
- quand elles ont été prises
- quel appareil ou caméra a été utilisé

Pour les utilisateurs de **Solana Mobile Seeker**, cela peut inclure des métadonnées comme :
- le modèle de l'appareil
- le logiciel de la caméra
- des chaînes de caractères telles que `"Taken on Seeker"`

Cette application aide à réduire les fuites accidentelles de métadonnées avant de partager des images publiquement.

---

## 🛡 Privacité et Sécurité

- Tout le traitement est effectué **localement sur l'appareil**
- L'application ne télécharge **pas** de photos où que ce soit
- Pas de comptes, pas de portefeuilles, pas d'interaction blockchain
- Permissions Android minimales, uniquement ce qui est nécessaire pour l'accès aux médias

---

## 📱 Permissions

L'application demande uniquement les permissions nécessaires pour accéder et nettoyer les métadonnées des photos :
- **Accès aux médias (images/vidéos) :** Pour lire et enregistrer des photos.
- **Pas de microphone**
- **Pas de caméra**
- **Pas de permissions de superposition**

---

## ⚠️ Notes Importantes

- Cette application supprime les **métadonnées**, pas les caractéristiques visuelles des photos.
- Elle ne peut pas garantir un anonymat complet ni empêcher toutes les formes d'empreinte digitale de l'appareil.
- Conçue comme un **outil d'hygiène OpSec**, pas comme une solution miracle pour la confidentialité.

---

## 🧪 Construit avec

- Expo (React Native)
- Android (Distribution APK)

---

## Développement

Ce projet est construit avec [Expo](https://expo.dev) et React Native.

```bash
# Installer les dépendances
npm install

# Démarrer l'application
npx expo start
```

## Build

### Android

```bash
# Preview build (APK pour tester)
npx eas-cli build -p android --profile preview

# Production build (AAB pour Google Play)
npx eas-cli build -p android --profile production
```

> **Note pour les utilisateurs de Windows :**
> Si vous rencontrez une erreur de sécurité PowerShell, ajoutez `cmd /c` au début de la commande :
> ```powershell
> cmd /c npx eas-cli build -p android --profile preview
> ```

---

## 📄 Licence

Licence MIT
