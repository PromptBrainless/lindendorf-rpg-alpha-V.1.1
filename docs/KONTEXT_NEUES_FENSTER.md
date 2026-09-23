# Kontext — neues Fenster

**Stand:** 23. September 2026. Pflicht nach `AGENTS.project.md`.

Aktives Repo: [PromptBrainless/lindendorf-rpg-alpha-V.1.1](https://github.com/PromptBrainless/lindendorf-rpg-alpha-V.1.1).
Vergleichs- und Archivstand: [export/spielversion1-7170673/](../export/spielversion1-7170673/). Der Export ist kein aktiver Arbeitsbaum und keine zweite Implementierungswahrheit.

## Was das Spiel ist

Lindendorf, illustriertes Textabenteuer. Deutsch, Du, Präsens.
Fluss, unverändert:

> Heldenerstellung → Prolog → Dorf-Schleife → Glockenweg oder Wald → Lager → Ende

Start: Stärke, Geschick, Charisma je 10. W10. Schwellen 8 / 12 / 15.
Zehn Lagen vor dem Tal. Höchstens drei Zustände.

## Was schon sitzt

| Stück | Datei |
|---|---|
| Mühle, Brunnen, Kesseljahr | `quest-muehle.ts`, `quest-brunnen.ts`, `quest-kesseljahr.ts` |
| Hauptfluss, Lager | `script.ts`, `lager-content.ts` |
| Weltwerkzeug | HUD **Welt**, `src/components/welt/WeltEditor.tsx`, Verträge `src/game/gm/` |
| Wissen | 22 Keys, `knowledge.ts` |
| Lore-Grenze | 41 Fakten, `src/game/lore.ts` |
| Textvergleich | `src/game/textvergleich.ts`, `npm run check:textvergleich` |
| Stimme | `werkstatt-vertrag.ts`, nur die offene Seite |

Nicht neu erfinden: `SpielleiterPanel`, `EditorApp`, `WeltEngine`, ein zweites Runtime.
`/editor` ist die Passworttür. `?welt` gilt nicht.

## Was die letzte Sitzung geändert hat

Abgleich, kein neuer Plot.

- Fenn sitzt an der Kirchmauer. Der Held nicht.
- Bertok steht beim ersten Besuch nicht unter Druck.
- Renniks Wand zeigt Bertoks Schein. Die zweite Schuld bleibt im Mahlstein.
- Hinter dem Stein nennt Vahls Großvater und die Aufteilung.
- Die Schlusskarte ist die Rückkehr zu Holm.
- Karrieren, Schicksal, Glück, Status und Herkunftsbegriffe bleiben erhalten, werden jedoch später als eigener Ausbau bearbeitet.

## Was liegen bleibt

`docs/UMBAU_UMGEBUNG.md` listet acht mögliche Anpassungen der Prompts.
Keine davon anfangen, bevor der Nutzer die Nummer nennt.

Nicht als Nächstes ausdenken: neue Quest, neue Flags, neue Bilder, kürzere Texte, Lager noch einmal extrahieren, Glockenweg noch einmal bauen. Beides ist spielbar.

## Wenn der Auftrag unklar ist

Nachfragen. Nicht den Erneuerungsplan als Auftrag lesen. Nicht die Manus-Anweisung. Nicht einen alten Handoff.
