---
title: 'SOTA Web Crawler, 1-Click WordPress i Dinamički Follow-Up'
date: '2026-11-10'
versionNumber: 'v0.8-beta'
description: 'Predstavljamo novi SOTA web crawler sa podrškom za headless rendering, WordPress 1-Click povezivanje, sažete AI odgovore i klikabilne opcije za nastavak razgovora.'
---

## SOTA Web Crawler, 1-Click WordPress i Dinamički Follow-Up

Izdanje **v0.8-beta** donosi temeljitu nadogradnju web crawler sistema, potpuno redizajniran WordPress dodatak i prirodnije vođenje razgovora uz pametne prijedloge narednih pitanja.

### 🕷️ SOTA Web Scraper & Headless Rendering (Faze 1–5)
- **Headless rendering podrška:** Integrisan Puppeteer / Playwright headless preglednik koji omogućava indeksiranje modernih SPA (Single Page Application) sajtova koji renderuju sadržaj putem JavaScripta.
- **Ekstrakcija strukturiranih podataka:** Automatsko preuzimanje Schema.org JSON-LD entiteta za proizvode, cijene, organizacije, radno vrijeme i često postavljana pitanja (FAQ).
- **Čišćenje navigacije i bannera:** Automatsko uklanjanje cookie traka, menija i ponavljajućih podnožja uz očuvanje semantičkih navigacijskih mrvica (breadcrumbs).
- **Varijabilni proizvodi:** Pametno prepoznavanje varijacija proizvoda i opcija direktno iz HTML-a.

### 🔌 Pitaj.io WordPress Plugin v1.5 / v1.6
- **1-Click Auto Connect:** Povezivanje WordPress sajta sa vašim Pitaj.io agentom u samo jednom kliku bez komplikovanog kopiranja API ključeva.
- **Monohromatski admin redizajn:** Minimalistički interfejs unutar WordPress administracije usklađen s izgledom Pitaj.io dashboarda.
- **Pouzdaniji embed:** Učitavanje widgeta direktno s `cdn.pitaj.io` uz sprječavanje keš konflikata sa WP Rocket i Cloudflare servisima.

### 💬 Sažeti odgovori i dinamičke opcije (`<<<OPCIJE>>>`)
- **Prirodniji stil odgovaranja:** AI asistent više ne ispisuje predugačke zidove teksta, već nudi kratak, direktan i jasan odgovor od 1–3 rečenice.
- **Klikabilni balončići za nastavak:** Na dnu svakog odgovora asistent nudi do 3 logična naredna pitanja koje posjetitelj može jednim klikom odabrati za nastavak razgovora.

### 🔄 Dvosmjerna sinhronizacija agenata
- Povezano interno ime agenta i javno ime bota (`bot_name`) kako bi postavke uvijek bile dosljedne.
