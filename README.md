# WinOpt

Optimizator de Windows pentru **gaming**, **privacy** și **debloat**, cu interfață în română. Un singur exe, fără instalare.

## Descărcare

**Link direct (ultima versiune):**

```
https://github.com/raull292/WinOpt/releases/latest/download/WinOpt.exe
```

1. Pune linkul de mai sus în browser — descarcă direct `WinOpt.exe` (sau mergi la [Releases](https://github.com/raull292/WinOpt/releases)).
2. Rulează-l **ca administrator** (aplicația cere singură drepturi de admin).

**Nota SmartScreen:** la prima rulare, Windows poate afișa „Windows protected your PC". Apasă **More info → Run anyway**. Mesajul apare doar pentru că exe-ul nu e semnat digital. Fiecare release include `SHA256SUMS.txt` pentru verificarea integrității.

## Ce face

- **Gaming & Performanță** — plan de alimentare Ultimate Performance, Game Mode, Game DVR OFF, prioritate multimedia pentru jocuri, accelerare mouse OFF, dezactivare servicii inutile și altele.
- **Privacy** — telemetrie la minim, Advertising ID / Activity History / sugestii și reclame OFF, căutare Bing în Start OFF, Copilot / Widgets / Recall OFF (Windows 11) și altele.
- **Debloat** — elimină aplicațiile preinstalate (Bing, Solitaire, Teams, aplicații sponsorizate gen Spotify/TikTok/Netflix); aplicațiile esențiale sunt protejate și nu apar niciodată în listă.
- **CMD (administrator)** — comenzile de reparare Windows (`sfc /scannow`, DISM) gata de copiat, plus deschidere CMD elevat dintr-un click.

## Siguranță

- **Backup + Revert**: fiecare tweak salvează starea originală înainte de modificare; totul se poate reveni din aplicație („Revert tot").
- **Servicii protejate**: `PcaSvc`, `CDPSvc`, `DPS`, `SSDPSRV`, `DiagTrack`, `SysMain`, `EventLog`, `CDPUserSvc_*`, `Appinfo`, `WSearch` nu sunt dezactivate niciodată (sunt necesare pentru Windows și pentru anticheat-uri gen FACEIT/Vanguard) — iar la fiecare pornire aplicația le verifică și le **repară automat** dacă altă unealtă le-a stricat.
- **Punct de restaurare** de sistem dintr-un click (și ofertat automat înainte de prima aplicare).
- **Mod preview**: pornește cu `WinOpt.exe --dry-run` și nimic nu se modifică — acțiunile doar se loghează.
- Log complet în `%ProgramData%\WinOpt\winopt.log`.

## ⚠️ Avertisment

Folosește pe propria răspundere. Aplicația modifică setări de sistem (registry, servicii, task-uri programate). Orice tweak se poate reveni din aplicație, în afară de aplicațiile eliminate din Debloat (acelea se reinstalează din Microsoft Store).

---

*Acest repo conține doar release-urile (exe-ul). Codul sursă este privat.*
