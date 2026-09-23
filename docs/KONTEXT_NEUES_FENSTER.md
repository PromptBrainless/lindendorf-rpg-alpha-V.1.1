# Kontext — neues Fenster

**Stand:** 23. September 2026. Pflicht nach `AGENTS.project.md`.

Aktives Repo: [PromptBrainless/lindendorf-rpg-alpha-V.1.1](https://github.com/PromptBrainless/lindendorf-rpg-alpha-V.1.1).
Inhaltlicher Stand: `wiki/`. Nicht das GitHub-Wiki, der Ordner im Repo.

## Was das Spiel heute tut

Lindendorf, illustriertes Textabenteuer. Deutsch, Du, Präsens.
Fluss, noch unverändert:

> Heldenerstellung → Prolog → Dorf-Schleife → Glockenweg oder Wald → Lager → Ende

Start: Stärke, Geschick, Charisma je 10. W10. Schwellen 8 / 12 / 15.
Zehn Lagen vor dem Tal. Höchstens drei Zustände. Noch keine Klassen und keine Karrierestufen im Code.

## Was schon spielbar ist

| Stück | Datei |
|---|---|
| Mühle, Brunnen, Kesseljahr | `quest-muehle.ts`, `quest-brunnen.ts`, `quest-kesseljahr.ts` |
| Hauptfluss, Lager | `script.ts`, `lager-content.ts` |
| Weltwerkzeug | HUD **Welt**, `src/components/welt/WeltEditor.tsx` |
| Wissen | 22 Keys, `knowledge.ts` |
| Lore-Grenze | `src/game/lore.ts`, am Wiki ausgerichtet |
| Stimme | `werkstatt-vertrag.ts`, nur die offene Seite |

## Was das Wiki jetzt vorgibt und der Code noch nicht erzählt

- Pakt unter der Kapelle. Drei Familien: Vahl, Dennek, Holm. Etwa dreißig Jahre.
- Umverteilung in Mühle, Steinbruch, Lagerhäuser. Ilse zählt, wen das Amt streicht.
- Rotes Wachs als Löschmarke. Glocke als Signal.
- Mühle als Versteck und Verteiler, nicht nur als Schuld bei Rennik.
- Banditen als Wache eines Transportwegs.
- Enden als Zustand des Dorfes, ohne Reinigung: `wiki/Enden.md`.
- Klassen, Karrieren, Status, Schicksal: dokumentiert, nicht mechanisch.

Eine Szene erst umschreiben, wenn der Auftrag sie nennt. Reihenfolge: `wiki/Queststruktur.md`. Den Pakt nicht in die Ankunft vorziehen.

## Nicht anfassen ohne Auftrag

Engine, Runtime, Auth, neue ArtKeys, Hauptfluss durch eine neue Quest ersetzen.
