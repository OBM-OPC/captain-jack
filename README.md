# Captain Jack Website

## Projektübersicht

Multi-Page Website für Captain Jack - Bootslagerung, Parking und Keelcrab Service in Preveza, Griechenland.

## Tech Stack

- **Framework:** Astro 5.x
- **Styling:** Tailwind CSS 4.x
- **Deployment:** Netlify

## Seiten

- **Startseite** (`/`) - Hero, Services Overview, Keelcrab Highlight, FAQ
- **Storage** (`/storage`) - Trockenlagerung, Preise (38€/m³, 225€/Auto)
- **Parking** (`/parking`) - Freie Stellplätze (125€/Boot), überdacht ab Winter 2026
- **Service** (`/service`) - Serviceleistungen (Details folgen)
- **Keelcrab** (`/keelcrab`) - Exklusiver Partner, 5 Key Points, Preise
- **Kontakt** (`/kontakt`) - Gosia Kontaktdaten, Standort
- **Impressum** (`/impressum`) - Rechtliche Angaben
- **Datenschutz** (`/datenschutz`) - Datenschutzerklärung

## Features

- ✅ Mobile-first responsive Design
- ✅ SEO-optimierte Struktur
- ✅ FAQ-Bereich mit Accordion
- ✅ Kontaktdaten für Gosia (DE + GR)
- ✅ Kein Festnetz, WhatsApp verfügbar
- ✅ Standort: Preveza Stadthafen (nicht Marina)
- ✅ Google Business ready
- ✅ Placeholder-Bilder für Kundenfotos

## Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build
```

## Deployment

Für Netlify-Deployment:

```bash
# Option 1: Netlify CLI (mit Login)
netlify login
netlify deploy --prod --dir=dist

# Option 2: Netlify Git Integration
# Connect GitHub/GitLab repository in Netlify dashboard
```

## To-Do (nach Kundenfeedback)

- [ ] Echte Bilder einbauen (Gebäude, Team, Keelcrab Maschine)
- [ ] Google Maps einbinden
- [ ] Firmendaten für Impressum vervollständigen
- [ ] Google Business Reviews integrieren
- [ ] Kundenbewertungen mit Bootsdetails
- [ ] Terminbuchungssystem (falls gewünscht)
- [ ] Service-Details mit Sascha klären

## Struktur

```
src/
├── components/
│   ├── Navigation.astro    # Mobile + Desktop Navigation
│   └── Footer.astro          # Footer mit Kontaktdaten
├── layouts/
│   └── Layout.astro          # Basis-Layout mit SEO
├── pages/
│   ├── index.astro           # Startseite
│   ├── storage.astro         # Storage Seite
│   ├── parking.astro         # Parking Seite
│   ├── service.astro         # Service Seite
│   ├── keelcrab.astro        # Keelcrab Seite
│   ├── kontakt.astro         # Kontakt Seite
│   ├── impressum.astro       # Impressum
│   └── datenschutz.astro     # Datenschutz
└── styles/
    └── global.css            # Tailwind Import
```

## Lizenz

© 2026 Captain Jack - Alle Rechte vorbehalten
