# Claude PWA – Osobní asistent

Minimalistická PWA aplikace pro přímou komunikaci s Claude AI.

## Soubory
- `index.html` – hlavní aplikace
- `manifest.json` – PWA manifest
- `sw.js` – service worker (offline podpora)
- `icon-192.svg` – ikona aplikace

## Spuštění

### Varianta A – GitHub Pages (zdarma, nejjednodušší)
1. Vytvoř nový repozitář na GitHubu
2. Nahraj všechny soubory
3. Jdi do Settings → Pages → Source: main / root
4. Aplikace běží na `https://tvoje-uzivatelske-jmeno.github.io/nazev-repo`

### Varianta B – Netlify (drag & drop)
1. Jdi na netlify.com → přetáhni složku
2. Dostaneš URL za 30 sekund

### Varianta C – lokálně
```bash
npx serve .
# nebo
python3 -m http.server 8080
```
Otevři http://localhost:8080

## Bezpečnost
- API klíč je uložen **pouze** v localStorage tvého prohlížeče
- Aplikace nemá žádný backend – vše jde přímo na api.anthropic.com
- API klíč nikdy neopustí tvůj prohlížeč jinak než při volání Anthropic API

## Instalace jako app (PWA)
- **Desktop Chrome/Edge**: klikni na ikonu instalace v adresním řádku
- **Android**: "Přidat na plochu" v menu prohlížeče
- **iOS Safari**: Sdílet → Přidat na plochu
