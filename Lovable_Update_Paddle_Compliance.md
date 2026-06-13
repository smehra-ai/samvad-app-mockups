# SAMVAD — Lovable Update Prompt: Paddle Compliance
*Direkt in den Lovable-Chat einfügen*

---

Please apply the following Paddle compliance changes across the entire codebase. These are label and text changes only — no logic changes.

## 1. i18n.tsx — Update these keys in BOTH `de` and `en` dictionaries

### English (`en`) — change these values:

| Key | Current value | New value |
|---|---|---|
| `"drama.title"` | `"Drama Triangle"` | `"Communication Patterns"` |
| `"drama.subtitle"` | `"The three roles in the Drama Triangle"` | `"Recurring interaction patterns that block productive dialogue"` |
| `"drama.persecutor"` | `"Persecutor"` | `"Critic"` |
| `"drama.victim"` | `"Victim"` | `"Passive Role"` |
| `"drama.rescuer"` | `"Rescuer"` | `"Enabler"` |
| `"drama.games"` | `"Common games"` | `"Common patterns"` |
| `"drama.reflect"` | `"Self-reflection"` | `"Leadership reflection"` |
| `"basics.ego"` | `"Ego states"` | `"Communication styles"` |
| `"basics.ego.desc"` | `"Transactional Analysis"` | `"Parent / Adult / Child modes"` |
| `"gen.type.help.desc"` | `"Diagnose: Will, Can, May, Must"` | `"Leadership self-check: responsibility reflection"` |
| `"gen.diagnose.title"` | `"Which responsibility is missing?"` | `"Leadership responsibility check"` |
| `"gen.diagnose.subtitle"` | `"Answer each dimension honestly."` | `"Reflect on your own leadership actions before the conversation."` |
| `"gen.diagnose.badge"` | `"Diagnose"` | `"Self-check"` |
| `"gen.diagnose.evaluate"` | `"Evaluate diagnosis"` | `"Find my conversation framework"` |
| `"dim.wollen.q"` | `"Is the motivation there?"` | `"Is the person showing willingness and engagement?"` |
| `"dim.koennen.q"` | `"Does the person have the skill?"` | `"Have I ensured the person has the necessary skills and training?"` |
| `"dim.duerfen.q"` | `"Do they have resources & permission?"` | `"Have I granted the necessary authority and resources?"` |
| `"dim.muessen.q"` | `"Are they actually responsible?"` | `"Have I clearly communicated what is expected?"` |

### German (`de`) — change these values:

| Key | Current value | New value |
|---|---|---|
| `"drama.title"` | `"Drama-Dreieck"` | `"Kommunikationsmuster"` |
| `"drama.subtitle"` | `"Die drei Rollen im Drama-Dreieck"` | `"Wiederkehrende Gesprächsmuster, die produktiven Dialog blockieren"` |
| `"drama.persecutor"` | `"Verfolger"` | `"Kritiker"` |
| `"drama.victim"` | `"Opfer"` | `"Passive Rolle"` |
| `"drama.rescuer"` | `"Retter"` | `"Ermöglicher"` |
| `"drama.games"` | `"Häufige Spiele"` | `"Häufige Muster"` |
| `"drama.reflect"` | `"Selbstreflexion"` | `"Führungsreflexion"` |
| `"basics.ego"` | `"Ich-Zustände"` | `"Kommunikationsstile"` |
| `"basics.ego.desc"` | `"Transaktionsanalyse"` | `"Eltern / Erwachsener / Kind"` |
| `"gen.type.help.desc"` | `"Diagnose: Wollen, Können, Dürfen, Müssen"` | `"Führungs-Selbstcheck: Verantwortungsreflexion"` |
| `"gen.diagnose.title"` | `"Welche Verantwortung fehlt?"` | `"Führungsverantwortung prüfen"` |
| `"gen.diagnose.subtitle"` | `"Beantworte jede Dimension ehrlich."` | `"Reflektiere deine eigenen Führungshandlungen vor dem Gespräch."` |
| `"gen.diagnose.badge"` | `"Diagnose"` | `"Selbstcheck"` |
| `"gen.diagnose.evaluate"` | `"Diagnose auswerten"` | `"Meinen Gesprächsrahmen ermitteln"` |
| `"dim.wollen.q"` | `"Ist die Motivation vorhanden?"` | `"Zeigt die Person Bereitschaft und Engagement?"` |
| `"dim.koennen.q"` | `"Kann die Person das?"` | `"Habe ich sichergestellt, dass die Person die nötigen Fähigkeiten hat?"` |
| `"dim.duerfen.q"` | `"Hat sie Ressourcen & Befugnis?"` | `"Habe ich die nötige Befugnis und Ressourcen bereitgestellt?"` |
| `"dim.muessen.q"` | `"Ist sie überhaupt zuständig?"` | `"Habe ich klar kommuniziert, was erwartet wird?"` |

---

## 2. _shell.module.drama.tsx — Update meta tags and page content

Change the `head()` meta tags:
- `title`: `"Drama-Dreieck — SAMVAD Modul"` → `"Kommunikationsmuster — SAMVAD Modul"`
- `description`: `"Opfer, Retter, Verfolger: die drei Rollen..."` → `"Wiederkehrende Kommunikationsmuster erkennen und produktiven Dialog fördern — ein Führungs-Tool für Executives."`
- `og:title`: same as title above

Change the `games` array (DE):
- `"Ja, aber …"` → stays (fine)
- `"Schau mal, was du angerichtet hast"` → `"Schuldzuweisung"`
- `"Wäre da nicht …"` → stays (fine)
- `"Ich versuch's ja nur"` → `"Überverantwortung übernehmen"`

Change the `exits` array (DE):
- `"Rolle benennen, nicht spielen."` → `"Muster benennen, nicht mitspielen."`
- All others stay the same.

Change the `reflect` array (DE):
- `"In welcher Rolle finde ich mich gerade?"` → `"Welches Kommunikationsmuster zeige ich gerade?"`
- `"Was würde Erwachsenenkommunikation jetzt brauchen?"` → `"Was würde sachliche Führungskommunikation jetzt brauchen?"`
- `"Wessen Problem löse ich gerade?"` → stays (fine)

Same changes in the `en` arrays:
- `"Look what you made me do"` → `"Blame shifting"`
- `"I'm only trying to help"` → `"Taking over responsibility"`
- `"In which role am I right now?"` → `"Which communication pattern am I showing right now?"`
- `"What would adult communication need now?"` → `"What would factual leadership communication need now?"`

---

## 3. _shell.module.basics.tsx — Update "Ego states" section

Find any visible label that says "Transaktionsanalyse", "Transactional Analysis", "Ego states", or "Ich-Zustände" and replace with "Kommunikationsstile" / "Communication Styles". The description should read "Eltern / Erwachsener / Kind Kommunikationsmodi" / "Parent / Adult / Child communication modes".

Do NOT change the underlying logic — only the visible labels.

---

## 4. subscribe.tsx — Update the BENEFITS array

Replace the current BENEFITS array with:

```typescript
const BENEFITS = [
  lang === "de"
    ? "KI-gestützte Gesprächsleitfäden, zugeschnitten auf deine Situation"
    : "AI-powered conversation guides tailored to your situation",
  lang === "de"
    ? "Members-only Insights für Leaders — Essays zu achtsamer Führung"
    : "Members-only Insights for Leaders — essays on mindful leadership",
  lang === "de"
    ? "Führungsverantwortung reflektieren, bevor du das Gespräch führst"
    : "Reflect on your leadership responsibility before every conversation",
  lang === "de"
    ? "PDF-Export — nimm deinen Leitfaden mit ins Gespräch"
    : "PDF export — take your guide into the meeting",
  lang === "de"
    ? "Jederzeit kündbar — 14-Tage-Rückgabegarantie"
    : "Cancel anytime — 14-day refund guarantee",
];
```

If the subscribe page does not use i18n/lang, just use the English version as static strings (already Paddle-compliant):
```typescript
const BENEFITS = [
  "AI-powered conversation guides tailored to your situation",
  "Members-only Insights for Leaders — essays on mindful leadership",
  "Reflect on your leadership responsibility before every conversation",
  "PDF export — take your guide into the meeting",
  "Cancel anytime — 14-day refund guarantee",
];
```

---

## 5. Meta tags — global SEO/description check

Search for any occurrence of the following words in ALL meta description tags, og:description tags, and page titles, and replace as follows:

| Find | Replace with |
|---|---|
| `"Drama-Dreieck"` | `"Kommunikationsmuster"` |
| `"Drama Triangle"` | `"Communication Patterns"` |
| `"Transaktionsanalyse"` | `"Kommunikationsstile"` |
| `"Transactional Analysis"` | `"Communication Styles"` |
| `"psychologisch"` | `"kommunikativ"` |
| `"psychological"` | `"communication-based"` |
| `"Diagnose"` (when referring to people) | `"Führungs-Selbstcheck"` |
| `"diagnose"` (when referring to people) | `"leadership self-check"` |

---

## 6. insights route — check one file

In `_shell.insights.drama-dreieck.tsx`: update the page title and any visible heading from "Drama-Dreieck" to "Kommunikationsmuster erkennen" / "Recognizing Communication Patterns". Keep all content — just rename the module label.

---

## Summary

These are label and text changes only. No logic, no routing, no database schema changes. The goal is that no visible UI text uses the words "Drama-Dreieck", "Transaktionsanalyse", "Ego states", "psychologisch", or "Diagnose des Mitarbeiters" — replacing them with business communication and leadership development terminology that is Paddle-compliant.
