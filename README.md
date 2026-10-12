# TA Signals – Android app

Tadawul ke shares (default: 1820 BAAN aur 3008 Al Kathiri) ke liye buy zone, targets, stop-loss, signals aur chances dikhane wali app.
Yeh app prices khud phone par laati hai. Claude ki zaroorat nahi.

## APK kaise banayein (ek baar, ~20 minute, computer par)

1. **GitHub account banayein:** https://github.com/signup (free).
2. **Nayi repository banayein:** upar right mein **+** → **New repository** → naam `mere-2-shares` → **Public** → **Create repository**.
3. **Files upload karein:** zip ko computer par unzip karein. Repository page par **"uploading an existing file"** link par click karein.
   `mere-2-shares` folder ke **andar ki saari cheezein** (`.github`, `app`, `build.gradle`, `settings.gradle`, `gradle.properties`, `README.md`) drag karke daalein → neeche **Commit changes**.
4. **Check karein:** repository mein `.github` folder dikhna chahiye. Agar nahi dikha, to neeche "Agar .github upload na ho" wala step karein.
5. **Build dekhein:** upar **Actions** tab kholiye. "Build APK" chal raha hoga (peela gol). 4–6 minute mein hara ✓ ho jayega.
   (Agar Actions enable karne ko pooche to hara button daba dein.)

## Phone par install

1. Phone ke Chrome mein kholiye: `https://github.com/<aapka-username>/mere-2-shares/releases`
2. **TASignals.apk** par tap karke download karein.
3. Download khol kar **Install** dabaiye. Phone "Unknown apps" ki permission maange to Chrome ko allow karein.
4. Play Protect warning aaye to **"Install anyway"** dabaiye. (Yeh aapki apni banayi app hai, Play Store se nahi, isliye warning aati hai.)

## Agar .github upload na ho

Repository mein **Add file → Create new file** → naam mein likhein `.github/workflows/build.yml` → is zip ki `.github/workflows/build.yml` file ka poora text paste karein → **Commit changes**.

## Agar build fail ho (laal ✕)

Actions mein fail hua run kholiye, laal step par click karke error ka text copy karein aur Claude ko bhejein.

## App mein kya hai

- Prices: Yahoo Finance se (~15 minute delayed), har baar app kholne par aur market hours (Sun–Thu, 10:00–15:00 Riyadh) mein har minute refresh.
- Internet na ho to aakhri saved data dikhata hai (upar naarangi rang mein likha aata hai).
- "Mere shares" mein koi bhi 4-ankon ka Tadawul code jod ya hata sakte hain.
- Yeh probability batati hai, guarantee nahi. Financial advice nahi hai.
