# Exif Cleaner for Seeker

Un limpiador de metadatos de fotos ligero diseñado para usuarios que se preocupan por la OpSec (seguridad operativa) y la privacidad.

[English](README.md) | [日本語](README_JA.md) | [Français](README_FR.md) | [Deutsch](README_DE.md) | [Italiano](README_IT.md) | [Español](README_ES.md) | [繁體中文](README_TW.md) | [简体中文](README_CN.md) | [한국어](README_KO.md) | [العربية](README_AR.md)

Esta aplicación elimina los metadatos de identificación de las fotos **localmente en su dispositivo**, antes de compartirlas en plataformas como X o Discord.

**Sin rastreo. Sin subidas. Totalmente sin conexión.**

---

## ✨ Características

- **Eliminación de datos de ubicación (GPS)**
- **Eliminación de identificadores de dispositivo y cámara**
- **Eliminación de etiquetas de software** como "Taken on Seeker"
- **Procesamiento sin conexión** (sin subidas a la red)
- **Sin análisis, sin rastreadores**
- **Soporte multilingüe:** Inglés, Japonés, Francés, Alemán, Italiano, Español, Chino (Tradicional/Simplificado), Coreano, Árabe
- **Modo oscuro:** Totalmente compatible

---

## 🔐 ¿Por qué existe esto?

Las fotos a menudo contienen metadatos ocultos que pueden revelar:
- dónde fueron tomadas
- cuándo fueron tomadas
- qué dispositivo o cámara se utilizó

Para los usuarios de **Solana Mobile Seeker**, esto puede incluir metadatos como:
- modelo del dispositivo
- software de la cámara
- cadenas como `"Taken on Seeker"`

Esta aplicación ayuda a reducir las fugas accidentales de metadatos antes de compartir imágenes públicamente.

---

## 🛡 Privacidad y Seguridad

- Todo el procesamiento se realiza **localmente en el dispositivo**
- La aplicación **no** sube fotos a ninguna parte
- Sin cuentas, sin billeteras, sin interacción con blockchain
- Permisos de Android mínimos, solo lo necesario para el acceso a medios

---

## 📱 Permisos

La aplicación solo solicita los permisos necesarios para acceder y limpiar los metadatos de las fotos:
- **Acceso a medios (imágenes/videos):** Para leer y guardar fotos.
- **Sin micrófono**
- **Sin cámara**
- **Sin permisos de superposición**

---

## ⚠️ Notas Importantes

- Esta aplicación elimina **metadatos**, no características visuales de las fotos.
- No puede garantizar el anonimato completo ni evitar todas las formas de huella digital del dispositivo.
- Diseñado como una **herramienta de higiene OpSec**, no como una solución mágica para la privacidad.

---

## 🧪 Construido con

- Expo (React Native)
- Android (Distribución APK)

---

## Desarrollo

Este proyecto está construido con [Expo](https://expo.dev) y React Native.

```bash
# Instalar dependencias
npm install

# Iniciar la aplicación
npx expo start
```

## Build

### Android

```bash
# Preview build (APK para pruebas)
npx eas-cli build -p android --profile preview

# Production build (AAB para Google Play)
npx eas-cli build -p android --profile production
```

> **Nota para usuarios de Windows:**
> Si encuentra un error de seguridad de PowerShell, agregue `cmd /c` al principio del comando:
> ```powershell
> cmd /c npx eas-cli build -p android --profile preview
> ```

---

## 📄 Licencia

Licencia MIT
