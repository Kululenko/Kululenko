# Aleks Paramonov

AI Developer aus Hamburg. Ich baue Software-Produkte mit Coding-Agenten (Claude Code, Codex). Ich plane, Agenten bauen, ich reviewe.

Ich suche eine Festanstellung in Hamburg, vor Ort, hybrid oder remote.

Portfolio mit Fallstudien zu allen Projekten: **[aleksparamonov.de](https://aleksparamonov.de)**

> In English: I build software products with coding agents. I plan, agents build, I review. Based in Hamburg, looking for a permanent role on site, hybrid or remote.

## Öffentlich einsehbar

**[zodiacally-ephemeris](https://github.com/Kululenko/zodiacally-ephemeris)** ist eine Ephemeride für Astrologie-Software in reinem JavaScript, gebaut auf den NASA/JPL-Daten DE440. Das Repository enthält einen Benchmark gegen die Swiss Ephemeris, den jeder selbst nachrechnen kann:

- Im Messlauf vom 08.11.2026 wich die berechnete Sonnenposition um höchstens 3,0 Millibogensekunden von der Swiss Ephemeris ab, die Mondposition um höchstens 8,7.
- Ist alles geladen, berechnet die Engine ein vollständiges Horoskop rund 14-mal schneller als die Swiss Ephemeris (Node.js, Apple M1).
- Wo die Engine schwächer ist, steht es dabei: langsamerer Kaltstart, weniger Himmelskörper, kürzerer Zeitraum.

Die Engine läuft seit Oktober 2026 auf [zodiacally.com](https://www.zodiacally.com/de/ephemeris/).

**[ai-gift-advisor](https://github.com/Kululenko/ai-gift-advisor)** ist ein eigenständiger Auszug aus dem Geschenkideengenerator: Ein Suchprofil aus Freitext, dessen Prüfung und die Auswahl aus einem Katalog. Die lokale Demo simuliert die Modellantwort, braucht keinen API-Schlüssel und hat eigene Tests.

## Live

| Produkt | Was es ist | Technik |
| --- | --- | --- |
| [zodiacally.com](https://www.zodiacally.com/de/ephemeris/) | Astrologie-Plattform mit eigener Rechenengine und KI-Deutungen, dazu eine Flutter-App | Astro, React, Node.js, Supabase, Flutter, Stripe |
| [geschenkideengenerator.com](https://geschenkideengenerator.com) | Geschenkideen-Website mit KI-Suche. Das Sprachmodell füllt aus dem Freitext nur ein festes Suchprofil aus, die Vorschläge wählt Code aus dem eigenen Katalog. | JavaScript, Netlify Functions, OpenAI API |
| [proteinvergleich.com](https://www.proteinvergleich.com) | Preisvergleich für 439 Proteinpulver. Ein Lauf prüft jeden Morgen die Preise in den Shops, die das zulassen. | Next.js, TypeScript, GitHub Actions |

Dazu ein Hörbuch-Shop mit Stripe-Bezahlung und befristeten Download-Links, live seit 10/2026.

## YouTube

Zwei deutschsprachige Kanäle, deren Folgen KI-Agenten produzieren. Die Stimmen sind KI-Stimmen (ElevenLabs), das steht in den Beschreibungen.

- **[True Crime Mystery Horror Hörbücher](https://www.youtube.com/@truecrimemysteryDE)**: lange Hörgeschichten, meist knapp eine Stunde. Skript, Stimme, Bilder, Schnitt in DaVinci Resolve über einen MCP-Server (Community-Projekt, von mir eingerichtet und unter Windows repariert) und die Prüfung der fertigen Datei übernehmen Agenten. Ich nehme Geschichte und Titelbild ab und gebe den Upload frei.
- **[Zodiacally – Astrologie verstehen](https://www.youtube.com/@ZodiacallyDE)**: Erklärvideos zur Astrologie. Ein geplanter Lauf arbeitet jeden Tag ohne Rückfragen: Recherche mit Quellen, Skript, Stimme, Animation als Code (HyperFrames), Prüfung, Titelbild und Upload. Veröffentlicht wird nie sofort, nur zu einem festen Termin.

## Weitere Projekte

- **Outava** ist eine Event-App für Hamburg (Flutter, Supabase), gemeinsam mit einem Geschäftspartner. Mein Teil ist die gesamte Technik. Der Import verarbeitet rund 50.000 Termine je Lauf und überspringt unveränderte Termine (altes Verfahren 97 Minuten, neues im Folgelauf 29 Minuten). Die Suche umfasste im September 2026 rund 59.000 Veranstaltungen, mehr als ein einzelner Import, weil der vorhandene Bestand dazugehört. Dazu kommen über 2.500 automatisierte Tests (Stand 22.10.2026). Stand: Testversion, noch nicht im Store, letzter Stand 10/2026.
- **Afuku** ist ein Actionspiel für den PC in Unreal Engine 5, das ich mit einem zweiten Entwickler baue. Agenten arbeiten dort über MCP-Server direkt in Blender und Unreal.
- **Agenten-Orchestrierung** (in Arbeit): Mein Ziel ist eine Zentrale, mit der ich spreche und die alle Aufgaben verteilt. Fertig ist sie noch nicht. Bisher sind es einzelne Abläufe je Projekt, die ich im Chat mit Codex und Claude steuere, meist per Diktat. Zu mir kommt nur, was mich braucht: Die Abläufe melden sich per Telegram bei Fehlern oder mit einer Vorschau. Einen ersten Aufbau mit 35 Rollen für acht Projekte habe ich am 05.10.2026 angehalten: Rund 200 von 286 Aufgaben waren Prüfen, Planen und Weiterleiten. Ab dem 09.10.2026 lief für Zodiacally ein kleinerer Aufbau: Feste Abläufe schreiben Artikel und X-Posts, Prüfskripte entscheiden, was live geht. Den Artikel-Teil habe ich am 30.10.2026 pausiert.

## So arbeite ich

- Architektur, Datenmodell und Abnahmekriterien lege ich fest. Den Code schreiben Agenten nach Regeln, die als `AGENTS.md` im Repository liegen.
- Was die KI an Code liefert, ist ein Entwurf. Ich reviewe ihn, bevor er online geht. Automatisierte Tests gehören dazu: Zodiacally hat über 4.000, Outava über 2.500 (Stand Oktober 2026).
- Sprachmodelle setze ich für Sprache ein: Absichten aus Text lesen und Texte schreiben. Auswahl, Preise, Berechnungen und Links kommen aus Code und Daten.

## Zur Einordnung

Viele meiner Repositories sind privat. Ich zeige sie gern im Gespräch.

Code entsteht bei mir über Agenten. Lesen, prüfen und Fehler eingrenzen kann ich selbst. Meine Grundlagen in Python, Django und SQL stammen aus einer einjährigen Vollzeit-Weiterbildung am Digital Career Institute.
