# 🎨 Captain Jack Branding Guide

Basierend auf: https://obm-captain-jack.netlify.app/

---

## 1. FARBSYSTEM (Tailwind CSS)

### Primärfarben (Slate/Dark)
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-slate-900` | `#0f172a` | Header, Footer Background |
| `bg-slate-800` | `#1e293b` | Hero Gradient, dunkle Sections |
| `bg-slate-950` | `#020617` | Footer (dunkelster) |
| `text-slate-300` | `#cbd5e1` | Hero Subtext, sekundärer Text |
| `text-slate-400` | `#94a3b8` | Muted Text, Platzhalter |

### Primärfarben (Blue/Primary)
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-blue-600` | `#2563eb` | Primary Buttons, Icons, CTA |
| `bg-blue-100` | `#dbeafe` | Light Icon Backgrounds |
| `text-blue-600` | `#2563eb` | Links, "Mehr erfahren" |
| `text-blue-200` | `#bfdbfe` | Hero Badges Text |
| `bg-blue-800` | `#1e40af` | Darker accents |

### Akzentfarben (Gold/Orange)
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-amber-500` | `#f59e0b` | Highlights, Key USPs |
| `text-amber-500` | `#f59e0b` | "Exklusiv" Text, Gold-Highlights |
| `bg-amber-100` | `#fef3c7` | Light backgrounds |
| `border-amber-500/30` | rgba(245,158,11,0.3) | Badge borders |
| `text-amber-600` | `#d97706` | Secondary gold text |

### Success/Check (Green)
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-emerald-500` | `#10b981` | Checkmarks, Success Icons |
| `bg-emerald-100` | `#d1fae5` | Light Icon Backgrounds |
| `text-emerald-600` | `#059669` | Success text |

### Neutrale Farben (Gray)
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-gray-50` | `#f9fafb` | Section Backgrounds |
| `bg-gray-100` | `#f3f4f6` | Problem Cards Background |
| `bg-white` | `#ffffff` | Cards, Content Background |
| `text-gray-900` | `#111827` | Headlines, Haupttext |
| `text-gray-600` | `#4b5563` | Body Text, Beschreibungen |
| `text-gray-500` | `#6b7280` | FAQ Icons, Muted |
| `border-gray-100` | `#f3f4f6` | Header border |

### Feature Icon Farben
| Tailwind | Hex | Verwendung |
|----------|-----|------------|
| `bg-amber-100` | `#fef3c7` | Service/Time Icons |
| `text-amber-600` | `#d97706` | Service Icons |
| `bg-purple-100` | `#f3e8ff` | Visibility/Sichtbarkeit |
| `text-purple-600` | `#9333ea` | Visibility Icons |
| `bg-cyan-100` | `#cffafe` | Location/Coast Icons |
| `text-cyan-600` | `#0891b2` | Location Icons |
| `bg-red-100` | `#fee2e2` | Problem Icons (Warning) |
| `text-red-600` | `#dc2626` | Problem Icons |

### Overlay & Effekte
| Tailwind | Verwendung |
|----------|------------|
| `bg-white/10` | Badge backgrounds |
| `backdrop-blur-sm` | Glassmorphism Effekt |
| `border-white/10` | Subtle borders auf dunklem |
| `bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900` | Hero Hintergrund |

---

## 2. TYPOGRAFIE

### Primärschrift
**Font Family:** Inter
**Fallback:** `font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;`

### Schriftgrößen (Tailwind)

| Element | Tailwind | Gewicht | Zeilenhöhe |
|---------|----------|---------|------------|
| **H1 (Hero)** | `text-4xl md:text-5xl lg:text-6xl` | `font-bold` (700) | `leading-tight` |
| **H2 (Sections)** | `text-3xl md:text-4xl` | `font-bold` (700) | `leading-tight` |
| **H3 (Cards)** | `text-xl` | `font-bold` (700) | `leading-tight` |
| **H4 (Features)** | Standard | `font-semibold` (600) | Normal |
| **Body Large** | `text-lg` | `font-normal` (400) | Normal |
| **Body** | Standard | `font-normal` (400) | Normal |
| **Small/Caption** | `text-sm` | `font-medium` (500) | Normal |
| **Label/Badge** | `text-sm` | `font-medium` (500) | Normal |

### Schriftstile
- **Überschriften:** Sentence case für Content
- **Labels:** Title case oder Sentence case
- **Tracking:** Standard (kein extra letter-spacing)

---

## 3. LAYOUT & SPACING

### Container
- **Max-Width:** `max-w-7xl` (1280px)
- **Padding:** `px-4 sm:px-6 lg:px-8` (16px / 24px / 32px)
- **Section Padding:** `py-20` (80px vertikal)

### Grid System
- **Service Cards:** `grid-cols-1 md:grid-cols-2 lg:grid-cols-4`
- **Problem Cards:** `grid-cols-1 md:grid-cols-3`
- **Feature Icons:** `grid-cols-2 lg:grid-cols-4`
- **Steps:** `grid-cols-1 md:grid-cols-3`

### Spacing Scale (Tailwind)
```
4px   - 1 (Icon-Gaps)
8px   - 2 (Badge-Padding)
16px  - 4 (Card-Padding)
24px  - 6 (Content-Gaps)
32px  - 8 (Section-Gaps)
48px  - 12 (Between major elements)
64px  - 16 (Section-Abstände)
80px  - 20 (py-20 Sections)
```

---

## 4. KOMPONENTEN

### Buttons

**Primary Button**
- Background: `bg-blue-600`
- Text: White
- Padding: `px-8 py-4`
- Border-radius: `rounded-lg`
- Font: `font-semibold`
- Hover: `hover:bg-blue-700`

**Secondary Button (Ghost/Outline)**
- Background: `bg-white/10`
- Border: `border border-white/10`
- Text: White
- Backdrop blur: `backdrop-blur-sm`

**Text-Link**
- Text: `text-blue-600`
- Hover: `hover:text-blue-700`
- Icon: Pfeil rechts

### Cards

**Service Card**
- Background: `bg-white`
- Border-radius: `rounded-2xl`
- Padding: `p-8`
- Shadow: `shadow-sm` → `hover:shadow-lg`

**Problem Card**
- Background: `bg-gray-50`
- Border-radius: `rounded-2xl`
- Padding: `p-8`
- Icon: Colored circle background

**Feature Card (Icon + Text)**
- Icon: `w-14 h-14` mit colored background
- Centered text

### Badges

**Stat Badge**
- Background: `bg-white/10 backdrop-blur-sm`
- Border-radius: `rounded-full`
- Text: `text-blue-200`

**Label Badge**
- Background: `bg-blue-100`
- Border-radius: `rounded-full`
- Text: `text-blue-700`

**"Exklusiv" Badge**
- Background: `bg-emerald-500/20 border border-emerald-500/30`
- Text: `text-emerald-300`

---

## 5. VISUELLE ELEMENTE

### Icons
- **Quelle:** Lucide Icons (Heroicons-style)
- **Größe:** `w-6 h-6` standard, `w-8 h-8` für größere
- **Container:** `w-12 h-12` oder `w-14 h-14` mit rounded-xl background

### Bilder
- **Hero:** Full-width mit `bg-cover bg-center` + opacity overlay
- **Cards:** Keine Bilder (nur Icons)
- **Aspect Ratio:** Keine spezifischen Vorgaben

### SVG Icons (Häufig verwendet)
- Boot/Yacht: `<path d="M2.5 8.5l2.5 3.5L9 9l4 6 3.5-2.5L22 19"/>`
- Check: Checkmark in emerald circle
- Phone: Telephone receiver
- Location: Map pin
- Calendar: Termin

---

## 6. SEKTIONEN-STRUKTUR (Tailwind Classes)

### 1. Navigation
```html
<header class="bg-white border-b border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-20">
```

### 2. Hero Section
```html
<section class="relative bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 text-white">
  <div class="absolute inset-0 bg-[url('/images/hero-bg.jpg')] bg-cover bg-center opacity-10">
```

### 3. Service Cards (4er Grid)
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
  <div class="bg-white rounded-2xl p-8 shadow-sm hover:shadow-lg transition-shadow">
```

### 4. Problem-Solution (3er Grid)
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
  <div class="bg-gray-50 rounded-2xl p-8 text-center">
```

### 5. USP Section (Keelcrab)
```html
<section class="py-20 bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 text-white">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
```

### 6. Feature Icons (4er Grid)
```html
<div class="grid grid-cols-2 lg:grid-cols-4 gap-8">
  <div class="text-center">
    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mx-auto mb-4">
```

### 7. Partner Section
- Badge: `bg-blue-100 rounded-full text-blue-700`
- Cards: `bg-white rounded-xl p-6 text-center shadow-sm`

### 8. 3-Step Process
```html
<div class="relative">
  <div class="text-8xl font-bold text-gray-100 absolute -top-6 left-0">01</div>
```

### 9. FAQ Accordion
```html
<div class="bg-white rounded-xl shadow-sm overflow-hidden">
  <button class="faq-toggle w-full flex justify-between items-center p-6 text-left">
```

### 10. CTA Footer
```html
<section class="py-20 bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 text-white">
```

### 11. Footer
```html
<footer class="bg-slate-950 text-slate-400 py-12">
```

---

## 7. RESPONSIVE BREAKPOINTS (Tailwind)

| Breakpoint | Min-Width | Tailwind |
|------------|-----------|----------|
| **Mobile** | 0 | Standard (kein Prefix) |
| **Tablet** | 640px | `sm:` |
| **Desktop** | 768px | `md:` |
| **Large** | 1024px | `lg:` |
| **XL** | 1280px | `xl:` |

### Mobile-First Pattern
```html
class="grid-cols-1 md:grid-cols-2 lg:grid-cols-4"
class="text-4xl md:text-5xl lg:text-6xl"
class="px-4 sm:px-6 lg:px-8"
```

---

## 8. JAVASCRIPT FUNKTIONEN

### FAQ Accordion
```javascript
document.querySelectorAll(".faq-toggle").forEach(e=>{
  e.addEventListener("click",()=>{
    const n=e.nextElementSibling,
    t=e.querySelector(".faq-icon"),
    a=e.getAttribute("aria-expanded")==="true";
    e.setAttribute("aria-expanded",!a),
    n?.classList.toggle("hidden"),
    t?.classList.toggle("rotate-180")
  })
});
```

### Solution Reveal
```javascript
document.querySelectorAll(".solution-btn").forEach(e=>{
  e.addEventListener("click",()=>{
    const n=e.getAttribute("data-target"),
    t=document.getElementById(n);
    t&&(t.classList.toggle("hidden"),
    e.textContent=t.classList.contains("hidden")?"Lösung anzeigen":"Lösung ausblenden")
  })
});
```

---

*Erstellt am: 17.04.2026*
*Quelle: Analyse von obm-captain-jack.netlify.app*
*Tailwind CSS 4.x*
