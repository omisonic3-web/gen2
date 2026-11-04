# Cimitir Parohial – aplicație Android

Proiect Capacitor: `www/` conține aplicația (index.html, style.css, app.js, vendor/xlsx).
Folderul `android/` este proiectul Android gata de compilat.

## Varianta A – Android Studio
1. Instalați Android Studio și Node.js 18+.
2. În acest folder: `npm install` apoi `npx cap sync android`
3. `npx cap open android` → Build → Build Bundle(s)/APK(s) → Build APK(s)
4. APK: `android/app/build/outputs/apk/debug/app-debug.apk`

## Varianta B – fără instalare (GitHub)
1. Creați un depozit gratuit pe github.com și încărcați tot conținutul acestui folder.
2. Fila Actions → „Build APK” → Run workflow.
3. După ~5 minute descărcați „Cimitir-Parohial-APK” (conține app-debug.apk).

## Instalare pe telefon
Copiați APK-ul pe telefon, deschideți-l și permiteți „Instalare din surse necunoscute”.

## Modificări ulterioare
Editați fișierele din `www/`, apoi `npx cap sync android` și recompilați.
Datele sunt păstrate local pe telefon: faceți periodic backup JSON (Backup → Export JSON).
Pe Android, exporturile și „Tipărește” deschid meniul de partajare (Salvează în Fișiere, WhatsApp, e-mail);
extrasul/adeverința se salvează ca fișier HTML, care se deschide în Chrome → Tipărește → Salvează ca PDF.
