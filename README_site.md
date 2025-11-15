README o stažené stránce

- Zdroj: https://dev-bobik.github.io/dnd/
- Staženo automaticky do složky `site/` v repozitáři
- Jak zobrazit lokálně: otevřete `/workspaces/dnd/site/dev-bobik.github.io/dnd/index.html` v prohlížeči
- Poznámky: Stránka obsahuje inline base64 obrázky a externí skripty (Firebase). Pokud chcete projekt integrovat, můžu:
  - přesunout soubory do kořenového `public/` a upravit cesty,
  - nebo převést do jednoduchého statického projektu (např. s `package.json`).

Pokud chcete, pokračuji úpravou nebo integrací — dejte vědět.

Jak nasadit na GitHub Pages (váš profil nebo repozitář):

- Umístěte soubory do větve `main` a do složky `docs/` (už jsem to udělal za vás: `docs/` obsahuje staženou stránku).
- Otevřete nastavení repozitáře → `Pages` a vyberte zdroj: `Branch: main` a `Folder: /docs`.
- Po uložení bude stránka dostupná na `https://<váše-uživatelské-jméno>.github.io/<repo>/` (nebo `https://<váše-uživatelské-jméno>.github.io/` pro uživatelské stránky, pokud repozitář pojmenujete `username.github.io`).

Lokální náhled:

1. Otevřete terminál v kořeni repozitáře a spusťte jednoduchý HTTP server:

```bash
python3 -m http.server --directory docs 8000
```

2. Otevřete `http://localhost:8000` v prohlížeči.

Poznámky o konfiguraci:
- Stránka používá externí Firebase skripty; ty budou fungovat, pokud projekt očekává ten samý Firebase projekt (konfigurace je v `index.html`). Pokud nechcete sdílet tyto údaje, můžeme je nahradit nebo odstranit.
- Pokud chcete, mohu:
  - automaticky commitnout a pushnout změny do repozitáře (řekněte, jestli chcete),
  - upravit cesty nebo vyčistit tracking externích zdrojů,
  - převést projekt na menší statický projekt s balíčkem (např. `package.json`) a `serve` skriptem.

