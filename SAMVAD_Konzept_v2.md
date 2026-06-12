# SAMVAD — Konzept & Mockup-Dokumentation
**The Art of Mindful Conversations**
*samvad.purebeing.eu · PURE BEING by Shalini Mehra*

---

## 1. Design-Entscheidungen

### Markenfamilie PURE BEING

| Element | purebeing.eu | ZENDO | SAMVAD |
|---|---|---|---|
| Wortmarke | PURE BEING Gold | PURE BEING Gold | PURE BEING Gold |
| Typografie | Cormorant Garamond | Cormorant Garamond | Cormorant Garamond |
| Akzentfarbe | Gold #D4B26A | Gold #D4B26A | Gold #D4B26A |
| Hintergrund | Schwarz | Creme #F5F0E8 | Creme #F5F0E8 |
| Hero-Stil | Drachen, Buddha | Zen-Garten | Zen-Garten + Menschen |
| Stimmung | Edel, repräsentativ | Ruhig, heilend | Klar, weise, menschlich |

**Begründung:** SAMVAD folgt der ZENDO-Innenstruktur (heller Creme-Hintergrund für alle Innen-Screens, volle Lesbarkeit) und teilt die DNA der Hauptmarke über Gold, Typografie und Bildsprache. Der Home-Screen hat ein atmosphärisches Zen-Garten-Bild mit der asiatischen Meisterin — das differenziert SAMVAD von ZENDO durch den menschlichen, gesprächsorientierten Fokus.

### Bildsprache
- **Divers und international:** Europäische, afrikanische, asiatische und gemischte Führungskräfte
- **Settings:** Zen-Boardroom, Garten, modernes Executive Office, Outdoor
- **Elemente:** Sumi-e-Malerei, Drachen-Artwork, Bonsai, Kirschblüten, Feng-Shui-Wasserfeature, Stadtpanorama
- **Zielgruppe sichtbar:** Sensitive Leaders & Entrepreneurs auf Executive Level, auch aufstrebende Führungskräfte

---

## 2. App-Struktur

### Navigation (Bottom Bar)
- **Home** — Einstieg, Generator-CTA, Gesprächstyp-Pills, 4 Module
- **Bibliothek** — Gespeicherte Leitfäden + Insights für Leaders
- **Favoriten** — Gemerkte Leitfäden und Artikel
- **Profil** — Account, Abo, Einstellungen, Sprache

### Generator-Flow (3 Schritte)

**Schritt 1 — Gesprächstyp wählen**
- Option A: Direkt auswählen (9 Typen: Motivieren, Ziele vereinbaren, Loben, Tadeln, Fördern, Konflikte, Verantwortungsdialog, Fehler eingestehen, Kontrollieren)
- Option B: Diagnose nutzen → führt zu Schritt 1b

**Schritt 1b — Diagnose (optional)**
- Vier Dimensionen: WOLLEN / KÖNNEN / DÜRFEN / MÜSSEN
- Je Dimension: JA / NEIN / UNSICHER
- Auswertung → empfiehlt Gesprächstyp automatisch

**Schritt 2 — Kontext eingeben**
- Was ist das Thema? *(Freitext)*
- Warum kommt es zu diesem Gespräch? *(Freitext)*
- Was soll das Ziel sein? *(Freitext)*

**Schritt 3 — Dein Leitfaden**
Personalisiertes Gesprächsskript mit:
- Vorbereitung (Fakten, Einstellung, Stimmung)
- Einstieg (konkreter Formulierungsvorschlag)
- Formulierungsbeispiele (3–5 Sätze)
- Worauf achten (Drama-Dreieck, Beurteilungsfehler, Wahrnehmung)
- Abschluss (Vereinbarung, Kontrolltermin)

**Aktionen nach dem Leitfaden:**
- Speichern (in Bibliothek)
- Teilen (Link oder Text)
- Als PDF (Download oder per E-Mail)

### 4 Wissens-Module (Home-Kacheln)

| Modul | Inhalt |
|---|---|
| Welche Verantwortung fehlt? | Wollen/Können/Dürfen/Müssen-Modell, Selbstcheck, Verantwortungsdialog |
| Welches Spiel läuft hier? | Drama-Dreieck, häufige Spiele, Ausstiegsstrategien |
| Vor dem Beurteilen | 8 Beurteilungsfehler als Checkliste, Pre-Flight-Reminder |
| Kommunikations-Basics | Ich-Zustände (TA), Wahrnehmungsregeln, Quittungen, Fragetechnik |

### Insights für Leaders
- Kuratierte Artikel unter der Bibliothek (kein "Blog")
- Beispielthemen: Das Drama-Dreieck erkennen, Führen ohne Angst, Psychologische Sicherheit
- Exklusiv für Mitglieder (Paddle-Abo)

---

## 3. Monetarisierung & KI-Kosten

### Empfohlenes Modell: Flat-Rate Abo mit monatlichem Generator-Limit

| Plan | Preis | Generator-Leitfäden/Monat | Module | Insights |
|---|---|---|---|---|
| Free | 0 € | 2 Leitfäden | Vollzugang | Nein |
| Essential | 9,99 €/Mo | 10 Leitfäden | Vollzugang | Ja |
| Professional | 19,99 €/Mo | Unbegrenzt | Vollzugang | Ja + Früher Zugang |
| Jahresabo (Pro) | 149 €/Jahr | Unbegrenzt | Vollzugang | Ja |

**Begründung:** Die KI-Generierung (OpenAI GPT-4o oder ähnlich) kostet ca. 0,01–0,05 € pro Leitfaden. Bei 10 Leitfäden/Monat und 9,99 € Abo ist die Marge sehr gesund. Unbegrenzte Nutzung ist nur im Pro-Plan — das schützt vor Missbrauch.

**PDF-Export:** Serverseitige PDF-Generierung (z.B. via Puppeteer oder WeasyPrint) — einmalige Kosten minimal, kein laufender KI-Aufwand. Empfehlung: im Essential und Pro Plan inklusive.

**Billing:** Paddle (wie bei ZENDO) — VAT-compliant für EU.

---

## 4. Übersicht der Mockup-Screens (v2, ZENDO-Stil)

| Screen | Datei |
|---|---|
| Home | v2_01_home.png |
| Gesprächstyp wählen | v2_02_gespraechstyp.png |
| Kontext eingeben | v2_03_kontext.png |
| Dein Leitfaden (Ergebnis) | v2_04_leitfaden.png |
| Diagnose (Wollen/Können/Dürfen/Müssen) | v2_06_diagnose.png |
| Drama-Dreieck | v2_07_drama.png |
| Vor dem Beurteilen | v2_08_beurteilung.png |
| Kommunikations-Basics + Insights | v2_09_kommunikation.png |
| Bibliothek + Insights für Leaders | v2_10_bibliothek.png |

### Bibliotheks-Bilder (diverse Leadership-Settings)

| Bild | Setting | Personen |
|---|---|---|
| lib_tadel.png | Zen-Boardroom, Sumi-e-Drachen-Gemälde | Europäische Frau (Executive) + asiatischer Mann |
| lib_motivation.png | Executive Office, Stadtpanorama, Golden Hour | Schwarzer Mann (Leader) + diverses Team |
| lib_foerdern.png | Zen-Garten, Kirschblüten, Outdoor | Europäische Mentorin + asiatische Frau |
| lib_konflikt.png | Boardroom, goldenes Drachen-Artwork | Europäischer Mann + südasiatischer Mann |
| lib_ziele.png | Skandinavisch-Feng-Shui, Bergblick, Wasserfeature | Europäische Frau + asiatischer Mann |

---

## 5. Nächste Schritte

1. **Freigabe Mockups** — Shalini bestätigt Design-Richtung
2. **GitHub-Repo anlegen** — privates Repo für SAMVAD
3. **Lovable-Build starten** — mit diesen Mockups als Referenz
4. **KI-Integration** — OpenAI API für Leitfaden-Generierung
5. **Paddle-Integration** — Abo-Modell wie bei ZENDO
6. **UMIT-Transkripte** — nach dem nächsten Training als Insights-Artikel einpflegen

---

*Erstellt: Juni 2026 · PURE BEING · samvad.purebeing.eu*
