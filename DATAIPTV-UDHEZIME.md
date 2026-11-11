# DataIPTV – përgatitja e projektit

Kjo kopje bazohet në Extreme InfiniTV dhe ruan licencën GPL-3.0-or-later dhe kreditet origjinale. Identifikuesi është pro.datapos.dataiptv; përditësimet automatike janë të fikura derisa të konfigurohet një çelës nënshkrimi i DataIPTV. Publikimet kërkohen te ffk-futsall/DataIPTV. Automatizimet origjinale janë në upstream-workflows/ dhe nuk janë aktive.

Testimi i ndërtimit web dhe i testeve JavaScript ka kaluar. Windows dhe Android nuk janë ndërtuar apo testuar ende në këtë përgatitje; migrimi i Android duhet verifikuar në pajisje. Ikonat origjinale dhe disa materiale historike mbeten. Bin/ përmban paketa Microsoft të projektit origjinal; .gitignore i përjashton nga GitHub derisa të kontrollohen kushtet e rishpërndarjes.

Për Windows duhen Node.js, pnpm dhe Rust plus ndërtuesit Visual Studio C++ dhe WebView2. Për Android nevojiten gjithashtu Java 21, Android Studio, SDK, NDK dhe objektivat Rust për Android. APK për shpërndarje duhet të nënshkruhet; mos i vendos çelësat e nënshkrimit ose fjalëkalimet në GitHub.

Kodit për zhvillim:

```powershell
pnpm install --frozen-lockfile
pnpm build
pnpm test
pnpm tauri build
```

Hapat e Android varen nga konfigurimi lokal dhe duhen testuar. Lexo README-UPSTREAM.md për burimin origjinal. Këto udhëzime nuk autorizojnë automatikisht përdorimin ose rishpërndarjen e përmbajtjes dhe binarëve të palëve të treta.
