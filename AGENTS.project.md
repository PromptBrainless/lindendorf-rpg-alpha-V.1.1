# Lindendorf — Pflicht vor jedem Auftrag

Das Spiel existiert. Nicht neu bauen, nicht scaffolden, keine zweite Engine.

Repo: nur `PromptBrainless/SpielVersion1.0`. Remote `origin`. Keine Spiegel.

## Zuerst lesen

1. Diese Datei.
2. `docs/KONTEXT_NEUES_FENSTER.md` — was wahr ist und was liegen bleibt.
3. Danach nur die Datei, die der Auftrag nennt.

`docs/UMBAU_UMGEBUNG.md` ist eine Entscheidungsliste. Sie ist kein Auftrag.
Die Nummern dort nicht umsetzen, solange der Nutzer sie nicht nennt.

Ältere Blätter (`HANDOFF.md`, `PROJEKTKONTEXT.md` vor dem 23. September,
`ANWEISUNGEN_MANUS.md`, `PROMPT_QUESTREIHE.md`) führen nicht. Steht dort
ein nächster Schritt, gilt er nicht.

## Wahrheit

Der Code gewinnt gegen jede Markdown-Datei.

| Was | Wo |
|---|---|
| Ablauf, bedingte Sätze | `src/game/script.ts`, `quest-*.ts`, `lager-content.ts` |
| Text, den der Spieler sieht | längste Fassung aus Karte, `ki-auflagen.json`, `volltexte.ts` — nur wenn sie dieselbe Handlung sagt |
| Wissen | `knowledge.ts`, abgeleitet, nicht gespeichert |
| Lore | `src/game/lore.ts`, GM-Grenze, keine Spielerzeile |
| Namen, Flags, Labels | `docs/QUESTREGISTER.md`, bei Zweifel der Code |
| Stimme im Spiel | `src/game/werkstatt-vertrag.ts` |
| Neue Quest | Skill `lindendorf-questreihe`, eine Quest pro Block |
| Seite nachschlagen | Skill `lindendorf` |

## Nicht tun

- Texte kürzen. Stichpunkte. Pathos. „In einer Welt.“
- Eine längere Fassung behalten, die eine andere Handlung erzählt. Beispiel, das schon falsch war: der Held sitzt in Fenns Mulde. Richtig: Fenn sitzt, das Kesseljahr kommt nur beim Warten.
- Lore, Nachbarszenen oder Namen in eine Seite schreiben, deren Ausgangstext sie nicht hat. Grovin, Rennik und das Kesseljahr sind an die Wahl gebunden.
- Am Brunnen heißt sie die Müllerin. Lene heißt sie in der Mühle.
- Renniks zweite Schuld hängt nicht an seiner Wand. Sie steckt im Papier aus dem Mahlstein.
- Die Schlusskarte ist die Rückkehr zu Holm. Kein Abschied vom Tal. Folgen nur für Wege, die gegangen wurden.
- Flags, ArtKeys, Endtitel, Engine, Runtime, Auth, DB, Router ohne Auftrag.
- Hub nach Zahlenindex. Immer nach Label.
- `public/art/` ohne Bildplan anfassen.
- `text-pack.json` als Kanon behandeln. Er legt alte Sätze nur auf, wenn die erste Zeile noch passt.

## Stimme, wenn du schreibst

Deutsch. Du. Präsens. „…“.
Befund, nicht Urteil. Geruch, Kälte, Gewicht, Arbeit.
Schöne Sätze nur, solange das Hässliche konkret bleibt.
Was geschieht, bleibt. Keine neue Handlung.

## Danach prüfen

`npm run typecheck`
`npm run check:prosa`
`npm run check:lore`
`npm run check:textvergleich`
`npm run check:knowledge`

Grün behaupten nur, wenn der Lauf grün war.
