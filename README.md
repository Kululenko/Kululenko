# Aleks Paramonov

AI Developer aus Hamburg. Ich baue Software-Produkte mit Coding-Agenten (Claude Code, Codex) und nehme nur ab, was Tests und Auswertungen besteht.

Ich suche eine Festanstellung in Hamburg oder remote.

> In English: I build software products with coding agents and ship only what passes tests. Based in Hamburg, looking for a permanent role there or remote in Germany.

## Öffentlich einsehbar

**[zodiacally-ephemeris](https://github.com/Kululenko/zodiacally-ephemeris)** ist eine Ephemeride für Astrologie-Software in reinem JavaScript, gebaut auf den NASA/JPL-Daten DE440. Das Repository enthält einen Benchmark gegen die Swiss Ephemeris, den jeder selbst nachrechnen kann:

- Sonne weicht um höchstens 3,0 Millibogensekunden ab, der Mond um höchstens 8,7.
- Ein vollständiges Chart ist warm rund 14-mal schneller berechnet (Node.js, Apple M1).
- Wo die Bibliothek schwächer ist, steht es dabei: langsamerer Kaltstart, weniger Himmelskörper, kürzerer Zeitraum.

Die Engine läuft seit Oktober 2026 in [zodiacally.com](https://zodiacally.com).

## Live

| Produkt | Was es ist | Technik |
| --- | --- | --- |
| [zodiacally.com](https://zodiacally.com) | Astrologie-Plattform mit eigener Ephemeriden-Engine und KI-Deutungen, dazu eine Flutter-App | Astro, React, Node.js, Supabase, Flutter, Stripe |
| [geschenkideengenerator.com](https://geschenkideengenerator.com) | Geschenkfinder. Das Sprachmodell liest nur ein Profil aus dem Freitext, die Vorschläge wählt Code aus dem eigenen Katalog. | JavaScript, Netlify Functions, OpenAI API |
| [proteinvergleich.com](https://www.proteinvergleich.com) | Preisvergleich für 439 Proteinpulver mit täglichem Preisabruf | Next.js, TypeScript, GitHub Actions |

## In Arbeit

- **Outava** ist eine Event-App für Hamburg (Flutter, Supabase). Die Importstrecke verarbeitet rund 50.000 Datensätze je Lauf, die Volltextsuche deckt 59.005 Events ab, dazu gehören 2.108 Tests. Stand: Testversion, noch nicht im Store.
- **Afuku** ist ein Action-Roguelite in Unreal Engine 5, das ich zu zweit entwickle. Agenten arbeiten dort über MCP-Server direkt in Blender und Unreal.

## So arbeite ich

- Architektur, Datenmodell und Abnahmekriterien lege ich fest. Den Code schreiben Agenten nach Regeln, die als `AGENTS.md` im Repository liegen.
- KI-Ergebnis ist ein Entwurf. In den Repositories von Zodiacally und Outava laufen zusammen über 5.000 automatisierte Tests.
- Sprachmodelle setze ich dort ein, wo sie stark sind: Absichten aus Text lesen. Auswahl, Preise und Links kommen aus Code und Daten.
- Ich weiß auch, wann Agenten zu viel sind. Einen Aufbau mit 35 Rollen habe ich betrieben, ausgewertet und auf zwei reduziert, weil der Großteil Koordination war.

## Zur Einordnung

Die meisten meiner Repositories sind privat. Ich zeige sie gern im Gespräch.

Code entsteht bei mir über Agenten. Lesen, prüfen und Fehler eingrenzen kann ich selbst. Meine Grundlagen in Python, Django und SQL stammen aus einer einjährigen Vollzeit-Weiterbildung am Digital Career Institute. Die älteren öffentlichen Repositories hier sind Übungen aus dieser Zeit.
