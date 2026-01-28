# Exif Cleaner for Seeker

OpSec(운영 보안)과 개인 정보를 중요하게 생각하는 사용자를 위해 설계된 경량 사진 메타데이터 클리너입니다.

[English](README.md) | [日本語](README_JA.md) | [Français](README_FR.md) | [Deutsch](README_DE.md) | [Italiano](README_IT.md) | [Español](README_ES.md) | [繁體中文](README_TW.md) | [简体中文](README_CN.md) | [한국어](README_KO.md) | [العربية](README_AR.md)

이 앱은 X나 Discord와 같은 플랫폼에 공유하기 전에 사진에서 식별 가능한 메타데이터를 **기기에서 로컬로** 제거합니다.

**추적 없음. 업로드 없음. 완전 오프라인.**

---

## ✨ 기능

- **위치 데이터(GPS) 제거**
- **기기 및 카메라 식별자 제거**
- **소프트웨어 태그 제거** (예: "Taken on Seeker")
- **오프라인 처리** (네트워크 업로드 없음)
- **분석 없음, 추적기 없음**
- **다국어 지원:** 영어, 일본어, 프랑스어, 독일어, 이탈리아어, 스페인어, 중국어(번체/간체), 한국어, 아랍어
- **다크 모드:** 완벽 지원

---

## 🔐 왜 이 앱이 필요한가요?

사진에는 종종 다음과 같은 정보를 드러낼 수 있는 숨겨진 메타데이터가 포함되어 있습니다:
- 촬영 장소
- 촬영 시점
- 사용된 기기 또는 카메라

**Solana Mobile Seeker** 사용자의 경우 여기에는 다음과 같은 메타데이터가 포함될 수 있습니다:
- 기기 모델
- 카메라 소프트웨어
- `"Taken on Seeker"`와 같은 문자열

이 앱은 이미지를 공개적으로 공유하기 전에 우발적인 메타데이터 유출을 줄이는 데 도움이 됩니다.

---

## 🛡 개인 정보 및 보안

- 모든 처리는 **기기에서 로컬로** 수행됩니다.
- 앱은 사진을 어디에도 업로드 **하지 않습니다**.
- 계정 없음, 지갑 없음, 블록체인 상호 작용 없음
- 최소한의 Android 권한, 미디어 액세스에 필요한 것만 요청

---

## 📱 권한

이 앱은 사진 메타데이터에 액세스하고 정리하는 데 필요한 권한만 요청합니다:
- **미디어 액세스(이미지/동영상):** 사진을 읽고 저장하기 위해.
- **마이크 없음**
- **카메라 없음**
- **오버레이 권한 없음**

---

## ⚠️ 중요 참고 사항

- 이 앱은 사진의 시각적 특성이 아니라 **메타데이터**를 제거합니다.
- 완전한 익명성을 보장하거나 모든 형태의 기기 지문 생성을 방지할 수는 없습니다.
- **OpSec 위생 도구**로 의도되었으며, 개인 정보 보호의 만병통치약은 아닙니다.

---

## 🧪 제작 도구

- Expo (React Native)
- Android (APK 배포)

---

## 개발

이 프로젝트는 [Expo](https://expo.dev) 및 React Native로 구축되었습니다.

```bash
# 의존성 설치
npm install

# 앱 시작
npx expo start
```

## 빌드

### Android

```bash
# Preview build (테스트용 APK)
npx eas-cli build -p android --profile preview

# Production build (Google Play용 AAB)
npx eas-cli build -p android --profile production
```

> **Windows 사용자 주의사항:**
> PowerShell 보안 오류가 발생하면 명령어 앞에 `cmd /c`를 붙이세요:
> ```powershell
> cmd /c npx eas-cli build -p android --profile preview
> ```

---

## 📄 라이선스

MIT License
