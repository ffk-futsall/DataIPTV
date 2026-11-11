# DataIPTV

DataIPTV është një përshtatje e Extreme InfiniTV, me pamje të frymëzuar nga DataPOS.

Kodi origjinal: https://github.com/infinitel8p/Extreme-InfiniTV. Ruhet licenca GPL-3.0-or-later; shih LICENSE dhe README-UPSTREAM.md.

## Gjendja

Përditësimet automatike janë të çaktivizuara derisa DataIPTV të ketë çelësin e vet të nënshkrimit. Shënimet e publikimeve dhe kërkimi manual lidhen me ffk-futsall/DataIPTV. Identifikuesi Android/Tauri është pro.datapos.dataiptv.

Skriptet origjinale të automatizimit gjenden te upstream-workflows/ dhe janë joaktive. Ato nuk duhen aktivizuar pa rishikim dhe përshtatje.

## Zhvillimi

Kërkohen Node.js, pnpm dhe Rust; për Android edhe Java 21, Android Studio, SDK dhe NDK.

```powershell
pnpm install --frozen-lockfile
pnpm build
pnpm test
pnpm tauri build
```

Për Android shiko dokumentacionin e Tauri dhe konfigurimin ekzistues të projektit. APK release kërkon nënshkrim privat; mos ngarko kurrë çelësat në GitHub. Ndërtimet native kërkojnë testim në Windows dhe Android.
