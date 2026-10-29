# Korištenje logo-design skilla u ChatGPT-u i Codexu

Originalni skill nalazi se u `skills/logo-design/`. Ovaj repozitorij ga već sadrži; **ne treba ga kopirati drugi put**. Metapodaci za ChatGPT nalaze se u `skills/logo-design/agents/openai.yaml`.

## ChatGPT: instalacija

1. Preuzmi ili kloniraj ovaj repozitorij na svoje računalo.
2. U korijenu repozitorija pokreni `python tools/package_skill.py` (ili `python3 tools/package_skill.py`).
3. Skripta izrađuje `dist/logo-design.zip` i manji `dist/logo-design-lite.zip`.
4. U ChatGPT-u otvori **/skills** i učitaj ZIP datoteku skilla. Ako puna verzija prelazi dopuštenu veličinu, koristi lite verziju.
5. Započni novi razgovor i zatraži dizajn, analizu ili doradu logotipa.

**Važno:** GitHub repozitorij nije isto što i instalirani ChatGPT skill. Samo dodavanje datoteka na GitHub ne aktivira skill u tvom ChatGPT računu. Potrebna je instalacija putem sučelja za Skills.

## Codex CLI: instalacija

Kopiraj cijeli direktorij `skills/logo-design` u korisničku mapu `~/.codex/skills/logo-design`, odnosno u projektni `.codex/skills/logo-design` ako agent podržava projektne skillove. Restartaj sesiju nakon instalacije.

## Tipični zadaci

- Osmisliti tri različita koncepta logotipa i prikazati ih za odabir prije izrade završnog paketa.
- Provjeriti postojeći SVG: geometriju, kontrast, čitljivost na 16 px i jednobojnu izvedbu.
- Izraditi varijante za web, favicon, ikonu aplikacije, tamnu pozadinu i smjernice korištenja.
- Kritički usporediti prijedloge bez kopiranja postojećih robnih marki iz referentne biblioteke.

Ako korisnik traži očuvanje originalnog logotipa, **nemoj ga redizajnirati**: radi samo prikaz, izvoz i primjenu dostavljene originalne datoteke.

## Ograničenja i autorska prava

Skill je izvorno djelo [kaankiziltug](https://github.com/kaankiziltug/logo-design-skill) i zadržava njegovu MIT licencu. Referentni logotipovi u biblioteci pripadaju njihovim vlasnicima te nisu licencirani za kopiranje ili uporabu u novim vizualima. Pogledaj `LICENSE` i `TRADEMARKS.md`.

Python 3 je potreban za skripte. Pojedini SVG/PNG prikazi dodatno zahtijevaju instaliran renderer, kako je opisano u `SKILL.md`.
