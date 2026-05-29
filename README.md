DT Detailing - Production-ready site

Co jsem upravil:

- `index.html` - kompletní refaktorace na čistý, validní HTML dokument.
  - Odstraněny všechny stopy po Lovable (badge, metadata, fonty, skripty).
  - Přidáno: `title`, `meta description`, Open Graph, Twitter card.
  - Přidáno: JSON-LD (`LocalBusiness`).
  - Opraveny cesty k lokálním obrázkům a CSS.
  - Jednoduchý kontaktní formulář s klientskou validací a potvrzením.
  - Paticka s aktuálním rokem.

- `styles/custom.css` - nové přepsání pro layout, hlavičku, hero, galerii a responzivitu.
  - Přidáno pro rychlou opravu rozložení a vizuální sjednocení.

- Upraven `index.html` tak, aby načítal `styles/custom.css` po hlavním CSS.

Doporučené další kroky:

- Prohlédnout a upravit `styles/styles-CA-1LR1X.css` pokud potřebuješ větší vizuální změny; `custom.css` nyní přebíjí základní pravidla.
- Odstranit nepotřebné binární fonty, pokud nejsou použity (ve složce `images/` je soubor `mcp-widgets_v1_fonts_CameraPlainVariable.woff2.bin`).
- Zkontrolovat soubor `scripts/flock.js` — pokud je to analytický/monitorovací skript, případně ho odpojit nebo nahradit reálným řešením.
- Otestovat stránku lokálně a na cílovém hostingu (GitHub Pages nebo vaše hostingové řešení).

Nasazení na GitHub Pages (rychlý návod):

1. Inicializuj repo a přidej soubory (pokud ještě nemáš git):

```bash
git init
git add .
git commit -m "Refactor: remove Lovable, prepare for production"
```

2. Vytvoř repo na GitHubu a pusheuj (nahraď URL):

```bash
git remote add origin git@github.com:USERNAME/REPO.git
git branch -M main
git push -u origin main
```

3. Zapni GitHub Pages v nastavení repo: Source -> `main` branch (root). Po chvíli bude stránka dostupná.

Seznam souborů upravených nebo přidaných:

- Upraveno: `index.html`
- Přidáno: `styles/custom.css`
- Přidáno: `README.md`

Poznámka: Pokud chceš, můžu automaticky odstranit soubor `images/mcp-widgets_v1_fonts_CameraPlainVariable.woff2.bin` a vytvořit `CNAME` nebo další soubory pro nasazení. Dej vědět, zda pokračovat.