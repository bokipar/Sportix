# Haptics Lab (Capacitor)

Потребно: Mac со Xcode, Node.js, iPhone и USB кабел.

## Првпат

```bash
npm install @capacitor/core @capacitor/cli @capacitor/ios @capacitor/haptics
npx cap add ios
npx cap sync ios
npx cap open ios
```

Во Xcode:
1. Лево кликни на проектот App, па на табот Signing & Capabilities.
2. Кај Team избери го твојот Apple ID (Add Account ако го нема).
3. Ако Bundle Identifier е зафатен, смени го (на пр. mk.boki.hapticslab2).
4. Горе избери го твојот iPhone (не симулатор) и притисни Run.

На iPhone првпат: Settings → General → VPN & Device Management → дозволи го твојот профил.
На iOS 16+ вклучи и Developer Mode (Settings → Privacy & Security).

## Кога ќе го смениш index.html

```bash
npx cap sync ios
```
па повторно Run во Xcode.

## Забелешки

- Симулаторот не вибрира, само вистински iPhone.
- Со бесплатен Apple ID апликацијата истекува по 7 дена, тогаш само пушти ја пак од Xcode.
