# T.Sikkema Engineering website

Statische website voor `t.sikkema-engineering.nl`, geschikt voor GitHub Pages.

## Bestanden

- `index.html` - Homepagina
- `diensten.html` - Dienstenpagina
- `blog.html` - Blogoverzicht
- `contact.html` - Contactpagina met statische mailto-formulierflow
- `assets/styles.css` - Styling
- `assets/script.js` - Mobiel menu, formulier en subtiele reveal-animatie
- `assets/logo-site.png` - Aangeleverd logo, alleen gebruikt in de bovenregel
- `assets/hero-engineering.jpg` - Geoptimaliseerde hero-afbeelding
- `CNAME` - Custom domain voor GitHub Pages
- `robots.txt` en `sitemap.xml` - SEO-bestanden

## Publiceren via GitHub Pages

1. Maak een nieuwe GitHub-repository aan, bijvoorbeeld `tsikkema-engineering-website`.
2. Plaats alle bestanden uit deze map in de root van de repository.
3. Ga in GitHub naar `Settings` > `Pages`.
4. Kies bij `Build and deployment` voor `Deploy from a branch`.
5. Kies branch `main` en folder `/root`.
6. Sla op en wacht tot GitHub Pages klaar is met publiceren.
7. Controleer bij `Custom domain` dat `t.sikkema-engineering.nl` ingevuld staat. Dit hoort ook in het meegeleverde `CNAME` bestand.

## DNS

Voor een subdomein zoals `t.sikkema-engineering.nl` is meestal een DNS-record nodig:

```text
Type: CNAME
Naam/Host: t
Waarde/Target: <github-gebruikersnaam>.github.io
```

Vervang `<github-gebruikersnaam>` door de GitHub-accountnaam waaronder de Pages-site draait.

## Contactformulier

GitHub Pages heeft geen server-side formulierverwerking. Het formulier opent daarom het e-mailprogramma van de bezoeker met een voorbereid bericht aan `terrysikkema@outlook.com`.
