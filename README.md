# Artikkel 8 — En interaktiv guide

En interaktiv guide til statens menneskerettslige plikt etter EMK artikkel 8: hva Strasbourg krever av staten, og hva som faktisk skjer når en norsk forelder ikke får se barnet sitt.

Bygd for **MannsForum** med utgangspunkt i:

- *Statens menneskerettslige plikt til å beskytte familierelasjoner* — Bjørn Joachimsen, [pasg.no](https://www.pasg.no/artikler/statens-menneskerettslige-plikt-til-beskytte-familierelasjoner)
- *Norsk praksis er i konflikt med EMDs krav til beskyttelse av retten til familieliv* — Øivind Østberg, Geir Kjell Andersland og Bjørn Joachimsen, *Advokatbladet*

## Lokalt

Guiden er én enkelt `index.html`-fil. Åpne den i nettleseren, eller server lokalt:

```bash
python3 -m http.server 8765
```

Gå til `http://localhost:8765`.

## Innhold

- **Start her** — kort introduksjon, aktørene i historien
- **01 · Rettigheten** — EMK artikkel 8, norsk gjennomføring
- **02 · Standarden** — fire ufravikelige prinsipper fra Strasbourg
- **Mellomspill** — scrollytelling som viser hvordan båndet brytes over år
- **03 · Dommene** — ni EMD-saker, filtrérbare etter prinsipp
- **04 · Tallene** — tre statistikker som viser hva passivitet koster
- **05 · Sammenligning** — Strasbourg-standarden vs. norsk praksis
- **06 · Norge** — EMDs dommer mot Norge, NIM-analyse, SSB-tall
- **07 · Kildene** — direkte lenker til alt

## Interaktivitet

- `⌘K` / `Ctrl+K` for søk på tvers av alt
- Trykk hamburgermenyen øverst til høyre for innholdsfortegnelse og ordliste
- Trykk på et prinsipp i Del 02 for å filtrere de ni dommene
- Trykk på en dom for å se utdrag fra avgjørelsen og åpne HUDOC
- Trykk en rad i Del 05 for å fokusere det paret av standard og praksis
- Bla gjennom Mellomspillet for å se forholdet forvitre over 14 år

## Publisere til GitHub Pages

1. Opprett et tomt repo på GitHub (f.eks. `mannsforum-artikkel-8`).
2. Lokalt:
   ```bash
   cd "Mannsforum poc - interactive guides"
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<bruker>/<repo>.git
   git push -u origin main
   ```
3. På GitHub: **Settings → Pages → Build and deployment**. Velg `Deploy from a branch`, `main`, og `/ (root)`. Lagre.
4. Etter ett til to minutter er guiden tilgjengelig på `https://<bruker>.github.io/<repo>/`.

`.nojekyll`-filen som ligger i repoet gjør at GitHub Pages ikke kjører Jekyll-prosessering, slik at alle filer serveres som de er.

## Filer

- `index.html` — hele guiden, én fil. Inneholder all CSS, JavaScript, ikoner og innhold.
- `mannsforum-logo.png` — MannsForum-logo, brukt i header og footer.
- `.nojekyll` — slår av Jekyll-prosessering på GitHub Pages.
- `.gitignore` — utelukker `.DS_Store`, `.claude/` og andre lokale filer.

## Lisens

Innhold © forfatterne. Kildehenvisninger er gitt direkte i guiden. Spør PASG.no / Advokatbladet før viderebruk av tekst. Logoen tilhører MannsForum.
