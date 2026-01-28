# Exif Cleaner for Seeker

Un pulitore di metadati fotografici leggero progettato per utenti attenti all'OpSec (sicurezza operativa) e alla privacy.

[English](README.md) | [日本語](README_JA.md) | [Français](README_FR.md) | [Deutsch](README_DE.md) | [Italiano](README_IT.md) | [Español](README_ES.md) | [繁體中文](README_TW.md) | [简体中文](README_CN.md) | [한국어](README_KO.md) | [العربية](README_AR.md)

Questa app rimuove i metadati identificativi dalle foto **localmente sul tuo dispositivo**, prima di condividerle su piattaforme come X o Discord.

**Nessun tracciamento. Nessun caricamento. Completamente offline.**

---

## ✨ Caratteristiche

- **Rimozione dati posizione (GPS)**
- **Rimozione identificatori dispositivo e fotocamera**
- **Rimozione tag software** come "Taken on Seeker"
- **Elaborazione offline** (nessun caricamento in rete)
- **Nessuna analisi, nessun tracker**
- **Supporto multilingue:** Inglese, Giapponese, Francese, Tedesco, Italiano, Spagnolo, Cinese (Tradizionale/Semplificato), Coreano, Arabo
- **Modalità scura:** Completamente supportata

---

## 🔐 Perché esiste?

Le foto contengono spesso metadati nascosti che possono rivelare:
- dove sono state scattate
- quando sono state scattate
- quale dispositivo o fotocamera è stato utilizzato

Per gli utenti di **Solana Mobile Seeker**, questo può includere metadati come:
- modello del dispositivo
- software della fotocamera
- stringhe come `"Taken on Seeker"`

Questa app aiuta a ridurre le perdite accidentali di metadati prima di condividere immagini pubblicamente.

---

## 🛡 Privacy e Sicurezza

- Tutta l'elaborazione avviene **localmente sul dispositivo**
- L'app **non** carica foto da nessuna parte
- Nessun account, nessun portafoglio, nessuna interazione blockchain
- Permessi Android minimi, solo quanto necessario per l'accesso ai media

---

## 📱 Permessi

L'app richiede solo i permessi necessari per accedere e pulire i metadati delle foto:
- **Accesso ai media (immagini/video):** Per leggere e salvare foto.
- **Nessun microfono**
- **Nessuna fotocamera**
- **Nessun permesso di sovrapposizione**

---

## ⚠️ Note Importanti

- Questa app rimuove i **metadati**, non le caratteristiche visive delle foto.
- Non può garantire il completo anonimato o prevenire tutte le forme di fingerprinting del dispositivo.
- Inteso come **strumento di igiene OpSec**, non come una soluzione miracolosa per la privacy.

---

## 🧪 Costruito con

- Expo (React Native)
- Android (Distribuzione APK)

---

## Sviluppo

Questo progetto è costruito con [Expo](https://expo.dev) e React Native.

```bash
# Installare le dipendenze
npm install

# Avviare l'app
npx expo start
```

## Build

### Android

```bash
# Preview build (APK per test)
npx eas-cli build -p android --profile preview

# Production build (AAB per Google Play)
npx eas-cli build -p android --profile production
```

> **Nota per utenti Windows:**
> Se riscontri un errore di sicurezza PowerShell, aggiungi `cmd /c` all'inizio del comando:
> ```powershell
> cmd /c npx eas-cli build -p android --profile preview
> ```

---

## 📄 Licenza

Licenza MIT
