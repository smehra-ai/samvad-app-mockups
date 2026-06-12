# SAMVAD — Mockup-Zusammenfassung & Strukturbewertung

**Datum:** 12. Juni 2026  
**Projekt:** SAMVAD (samvad.purebeing.eu)  
**Zweck:** Mockups als Vorlage für den Bau in Lovable (via GitHub)

---

## 1. Design-Entscheidungen

### Farbpalette (final für Lovable)

| Token | Hex | Verwendung |
|---|---|---|
| Background | `#0A0A0F` | Haupt-Hintergrund (fast Schwarz) |
| Surface | `#1A1A3E` | Karten, Cards, Nav-Elemente (Dunkelblau/Navy) |
| Accent | `#D4B26A` | Gold — Icons, Borders, aktive Elemente, CTAs |
| Text Primary | `#FDF8F4` | Cream — Fließtext, Headlines |
| Text Muted | `#A89F94` | Gedämpftes Cream für Subtitles |

### Typografie

| Element | Font | Gewicht |
|---|---|---|
| Headlines | Cormorant Garamond | Light (300) |
| Fließtext | Crimson Pro | Regular (400) |
| Labels/Badges | Crimson Pro | SemiBold (600) |

### Design-Prinzipien

- **Eine Hauptaktion pro Screen** — keine Reizüberflutung
- **Viel Schwarzraum** — edel, ruhig, hochwertig
- **Gold-Kontur auf Navy** — Karten-Stil durchgängig
- **Konsistent mit purebeing.eu** — Schwarz-Gold-Ästhetik
- **Gut lesbar** — Cream auf dunklem Grund, ausreichend Kontrast

---

## 2. Bewertung der von Claude vorgeschlagenen Struktur

Die im Konzept-Brief definierte Struktur (10 Screens) ist **solide und gut durchdacht**. Meine Einschätzung:

### Stärken der Struktur

- **Klare Diagnose-Logik:** Die 4 Dimensionen (Wollen/Können/Dürfen/Müssen) als Routing-Mechanismus ist ein echtes Alleinstellungsmerkmal. Das unterscheidet SAMVAD von generischen KI-Gesprächshilfen.
- **Einheitliche Leitfaden-Anatomie:** Dass jeder Output die gleiche Struktur hat (Vorbereitung → Einstieg → Formulierungen → Worauf achten → Abschluss), schafft Wiedererkennbarkeit und Vertrauen.
- **Sinnvolle v1/v2-Trennung:** v1 fokussiert auf den Generator-Kern + die wichtigsten Referenz-Module. v2 ergänzt Tiefe (Beurteilungsfehler, Kommunikations-Basics, Videos).
- **Zweisprachigkeit von Anfang an:** Die FKT-Karten liegen bereits bilingual vor — das ist ein großer Vorteil.

### Empfehlungen zur Optimierung

| Punkt | Empfehlung |
|---|---|
| **Navigation** | 3-Punkt-Bottom-Nav (Start/Bibliothek/Profil) ist richtig. Die Referenz-Module (Verantwortung, Drama-Dreieck etc.) sind über Home erreichbar — das reicht für v1. |
| **Generator-Flow** | 3 Schritte (Thema → Diagnose → Ergebnis) sind ideal. Nicht mehr. Der „Unsicher"-Button bei der Diagnose ist klug — er erlaubt dem System, bei Unklarheit einen allgemeineren Leitfaden zu generieren. |
| **Onboarding** | Für v1 kein separates Onboarding nötig. Der Home-Screen ist selbsterklärend. Für v2 ggf. ein kurzes Tutorial beim ersten Öffnen. |
| **PDF-Export** | Ja, in v1 aufnehmen. Führungskräfte wollen den Leitfaden ausdrucken oder ins Meeting mitnehmen. |
| **Offline-Fähigkeit** | Als PWA sollte die Bibliothek offline verfügbar sein. Der Generator braucht Internet (KI-Call). |
| **UMIT-Inhalte** | Platzhalter „BALD" im Kommunikations-Basics-Modul ist korrekt. Sobald neue Transkripte vorliegen, können diese als Micro-Learning-Einheiten eingepflegt werden. |

### Technische Architektur für Lovable

| Komponente | Umsetzung |
|---|---|
| Frontend | React + Tailwind (Lovable-Standard) |
| KI-Backend | Ein einzelner AI-Call pro Leitfaden-Generierung |
| Datenbank | Gespeicherte Leitfäden (Bibliothek) |
| Auth | Wie ZENDO (Abo-Modell) |
| PWA | Installierbar, Offline-Bibliothek |
| Hosting | samvad.purebeing.eu (Subdomain) |

---

## 3. Screen-Übersicht der Mockups

| # | Screen | Datei | Sprache |
|---|---|---|---|
| 1 | Home / Start | `01_home_de.png` | DE |
| 1 | Home / Start | `01_home_en.png` | EN |
| 2 | Generator — Thema | `02_generator_thema_de.png` | DE |
| 3 | Generator — Diagnose | `03_diagnose_de.png` | DE |
| 4 | Ergebnis — Leitfaden | `04_leitfaden_ergebnis_de.png` | DE |
| 4 | Ergebnis — Leitfaden | `04_leitfaden_ergebnis_en.png` | EN |
| 5 | Welche Verantwortung fehlt? | `05_verantwortung_de.png` | DE |
| 6 | Drama-Dreieck | `06_drama_dreieck_de.png` | DE |
| 7 | Vor dem Beurteilen | `07_beurteilungsfehler_de.png` | DE |
| 8 | Kommunikations-Basics | `08_kommunikation_basics_de.png` | DE |
| 9 | Bibliothek | `09_bibliothek_de.png` | DE |
| 10 | Profil | `10_profil_de.png` | DE |

---

## 4. Nächste Schritte

1. **Mockups reviewen** — Feedback zu Design, Farben, Layout
2. **Lovable-Projekt aufsetzen** — GitHub-Repo erstellen, Grundstruktur
3. **Generator-Prompt-Spec** — Detaillierte KI-Prompt-Logik je Gesprächstyp
4. **Content einspeisen** — FKT-Karten-Texte als Datenbasis
5. **UMIT-Transkripte** — Dieses Jahr neue erstellen, dann in Kommunikations-Basics integrieren

---

## 5. Fireflies-Status

Die Fireflies-Integration hat beim Abruf der UMIT-Transkripte (Juni 2025) nicht reagiert (Timeout). Shalini wird dieses Jahr neue Transkripte erstellen. Der Platzhalter „BALD" im Kommunikations-Basics-Modul ist entsprechend gesetzt.

---

*Erstellt von Manus als Grundlage für den Lovable-Bau der SAMVAD-App.*
