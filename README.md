# Aleks Paramonov

AI Developer aus Hamburg. Ich baue Software-Produkte mit Coding-Agenten (Claude Code, Codex) und nehme nur ab, was die Tests bestanden hat.

Ich suche eine Festanstellung in Hamburg, vor Ort, hybrid oder remote.

Portfolio mit Fallstudien zu allen Projekten: **[aleksparamonov.de](https://aleksparamonov.de)**

> In English: I build software products with coding agents and ship only what passes tests. Based in Hamburg, looking for a permanent role on site, hybrid or remote.

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

## Weitere Projekte

- **Outava** ist eine Event-App für Hamburg (Flutter, Supabase), gemeinsam mit einem Geschäftspartner. Mein Teil ist die gesamte Technik. Der Import verarbeitet rund 50.000 Termine je Lauf und überspringt unveränderte Termine (altes Verfahren 97 Minuten, neues im Folgelauf 29 Minuten). Die Suche umfasste im September 2026 rund 59.000 Veranstaltungen, mehr als ein einzelner Import, weil der vorhandene Bestand dazugehört. Dazu kommen über 2.500 automatisierte Tests (Stand 22.10.2026). Stand: Testversion, noch nicht im Store, letzter Stand 10/2026.
- **Afuku** ist ein Actionspiel für den PC in Unreal Engine 5, das ich mit einem zweiten Entwickler baue. Agenten arbeiten dort über MCP-Server direkt in Blender und Unreal.

## So arbeite ich

- Architektur, Datenmodell und Abnahmekriterien lege ich fest. Den Code schreiben Agenten nach Regeln, die als `AGENTS.md` im Repository liegen.
- Was die KI liefert, ist ein Entwurf. Zodiacally hat über 4.000 automatisierte Tests, Outava über 2.500 (Stand Oktober 2026). Im letzten vollen Lauf der Zodiacally-App fielen 9 von 3.056 Tests durch: 6 erwarteten noch den früheren Kaufablauf, 2 scheiterten an Zeilenenden einer Datendatei, 1 an einer zu engen Bildgrenze unter Windows. Die gezielten Nachtests bestanden.
- Sprachmodelle setze ich für Sprache ein: Absichten aus Text lesen und Texte schreiben. Auswahl, Preise, Berechnungen und Links kommen aus Code und Daten.
- Ich weiß auch, wann Agenten zu viel sind. Einen Aufbau mit 35 Rollen habe ich betrieben, angehalten und auswerten lassen: Von 286 Aufgaben waren rund 200 keine Arbeit am Produkt. Ergebnis ist ein Plan für zwei Agenten und ein Skript. Er ist noch nicht umgesetzt.

## Zur Einordnung

Viele meiner Repositories sind privat. Ich zeige sie gern im Gespräch.

Code entsteht bei mir über Agenten. Lesen, prüfen und Fehler eingrenzen kann ich selbst. Meine Grundlagen in Python, Django und SQL stammen aus einer einjährigen Vollzeit-Weiterbildung am Digital Career Institute.
