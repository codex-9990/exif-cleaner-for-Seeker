# Exif Cleaner for Seeker

Ein leichter Foto-Metadaten-Reiniger, entwickelt für Benutzer, die Wert auf OpSec (Operationssicherheit) und Privatsphäre legen.

[English](README.md) | [日本語](README_JA.md) | [Français](README_FR.md) | [Deutsch](README_DE.md) | [Italiano](README_IT.md) | [Español](README_ES.md) | [繁體中文](README_TW.md) | [简体中文](README_CN.md) | [한국어](README_KO.md) | [العربية](README_AR.md)

Diese App entfernt identifizierende Metadaten von Fotos **lokal auf Ihrem Gerät**, bevor Sie sie auf Plattformen wie X oder Discord teilen.

**Kein Tracking. Kein Upload. Vollständig offline.**

---

## ✨ Funktionen

- **Entfernung von Standortdaten (GPS)**
- **Entfernung von Geräte- und Kamerakennungen**
- **Entfernung von Software-Tags** wie "Taken on Seeker"
- **Offline-Verarbeitung** (keine Netzwerk-Uploads)
- **Keine Analysen, keine Tracker**
- **Mehrsprachige Unterstützung:** Englisch, Japanisch, Französisch, Deutsch, Italienisch, Spanisch, Chinesisch (Traditionell/Vereinfacht), Koreanisch, Arabisch
- **Dunkelmodus:** Vollständig unterstützt

---

## 🔐 Warum gibt es das?

Fotos enthalten oft versteckte Metadaten, die Folgendes preisgeben können:
- wo sie aufgenommen wurden
- wann sie aufgenommen wurden
- welches Gerät oder welche Kamera verwendet wurde

Für Benutzer von **Solana Mobile Seeker** kann dies Metadaten umfassen wie:
- Gerätemodell
- Kamerasoftware
- Zeichenfolgen wie `"Taken on Seeker"`

Diese App hilft, versehentliche Metadatenlecks zu reduzieren, bevor Bilder öffentlich geteilt werden.

---

## 🛡 Privatsphäre & Sicherheit

- Die gesamte Verarbeitung erfolgt **lokal auf dem Gerät**
- Die App lädt Fotos **nirgendwo** hoch
- Keine Konten, keine Wallets, keine Blockchain-Interaktion
- Minimale Android-Berechtigungen, nur das Nötigste für den Medienzugriff

---

## 📱 Berechtigungen

Die App fordert nur Berechtigungen an, die für den Zugriff und die Bereinigung von Foto-Metadaten erforderlich sind:
- **Medienzugriff (Bilder/Videos):** Zum Lesen und Speichern von Fotos.
- **Kein Mikrofon**
- **Keine Kamera**
- **Keine Overlay-Berechtigungen**

---

## ⚠️ Wichtige Hinweise

- Diese App entfernt **Metadaten**, nicht die visuellen Merkmale von Fotos.
- Sie kann keine vollständige Anonymität garantieren oder alle Formen des Geräte-Fingerprinting verhindern.
- Gedacht als **OpSec-Hygienewerkzeug**, nicht als Allheilmittel für den Datenschutz.

---

## 🧪 Gebaut mit

- Expo (React Native)
- Android (APK-Verteilung)

---

## Entwicklung

Dieses Projekt wurde mit [Expo](https://expo.dev) und React Native erstellt.

```bash
# Abhängigkeiten installieren
npm install

# App starten
npx expo start
```

## Build

### Android

```bash
# Preview build (APK zum Testen)
npx eas-cli build -p android --profile preview

# Production build (AAB für Google Play)
npx eas-cli build -p android --profile production
```

> **Hinweis für Windows-Benutzer:**
> Wenn Sie auf einen PowerShell-Sicherheitsfehler stoßen, stellen Sie `cmd /c` vor den Befehl:
> ```powershell
> cmd /c npx eas-cli build -p android --profile preview
> ```

---

## 📄 Lizenz

MIT Lizenz
