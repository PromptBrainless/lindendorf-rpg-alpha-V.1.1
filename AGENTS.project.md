# Lindendorf — Pflicht vor jedem Auftrag

Das Spiel existiert. Nicht neu bauen, nicht scaffolden, keine zweite Engine.

## Aktives Projekt

Aktives Haupt-Repository: `PromptBrainless/lindendorf-rpg-alpha-V.1.1`.

Ältere Lindendorf-Repositories und andere Projekte von `PromptBrainless` dürfen bei Bedarf als Vergleichs- und Ideenquellen durchsucht werden. Sie sind keine automatische Quelle für den aktuellen Kanon. Inhalte aus älteren Ständen dürfen nur nach Prüfung übernommen werden.

`export/spielversion1-7170673/` ist ein archivierter/exportierter Vergleichsstand innerhalb dieses Repositories. Er ist nicht die aktive Arbeitsquelle und darf nicht als zweite Implementierungswahrheit behandelt werden. Abweichungen zwischen dem Hauptbaum und dem Export sind zugunsten des aktiven Hauptbaums zu prüfen.

## Zuerst lesen

1. Diese Datei.
2. `docs/KONTEXT_NEUES_FENSTER.md` — was wahr ist und was liegen bleibt.
3. Danach nur die Datei, die der Auftrag nennt.

`docs/UMBAU_UMGEBUNG.md` ist eine Entscheidungsliste. Sie ist kein Auftrag. Die Nummern dort nicht umsetzen, solange der Nutzer sie nicht nennt.

Ältere Blätter (`HANDOFF.md`, `PROJEKTKONTEXT.md` vor dem 23. September, `ANWEISUNGEN_MANUS.md`, `PROMPT_QUESTREIHE.md`) führen nicht automatisch. Steht dort ein nächster Schritt, gilt er nicht ohne erneute Prüfung oder ausdrücklichen Auftrag.

## Wahrheit

Der Code gewinnt gegen widersprechende Markdown-Dateien. Wiki und Anhänge sind Prüf-, Dokumentations- und Ideenquellen; sie werden nicht stillschweigend als neue Spielregeln umgesetzt.

| Was | Wo |
|---|---|
| Aktiver Ablauf, bedingte Sätze | `src/game/script.ts`, `src/game/quest-*.ts`, `src/game/lager-content.ts` |
| Text, den der Spieler sieht | längste Fassung aus Karte, `ki-auflagen.json`, `volltexte.ts` — nur wenn sie dieselbe Handlung sagt |
| Wissen | `src/game/knowledge.ts`, abgeleitet, nicht gespeichert |
| Lore | `src/game/lore.ts`, GM-Grenze, keine Spielerzeile |
| Namen, Flags, Labels | `docs/QUESTREGISTER.md`, bei Zweifel der Code |
| Stimme im Spiel | `src/game/werkstatt-vertrag.ts` |
| Neue Quest | Skill `lindendorf-questreihe`, eine Quest pro Block |
| Seite nachschlagen | Skill `lindendorf` |
| Weltwerkzeug-Kanon | aktive Kanonquellen und implementierte Daten; keine freien Entwürfe oder unbestätigten Wiki-Ideen |

## Charaktererschaffung, Klassen und Karrieren

Die Karriereinhalte im Wiki und in den zugehörigen Arbeitsmaterialien bleiben erhalten und werden später vollständig bearbeitet. Sie sind für die weitere Projektplanung relevant, aber noch nicht automatisch vollständig in der laufenden Engine implementiert.

Für Lindendorf gilt zunächst:

- Klasse bezeichnet ein soziales Milieu.
- Karriere bezeichnet den aktuellen Beruf beziehungsweise die Arbeit.
- Stufe bezeichnet den Entwicklungsstand innerhalb der Karriere.
- Flussvolk, Freisassen, Gesetzlose und vergleichbare Begriffe sind Herkunfts- oder soziale Begriffe, keine Fantasy-Rassen.
- Fantasy-Rassen werden nicht eingeführt.
- Volltexte zu Karrieren werden nicht durch Kurzfassungen ersetzt.
- Karriereeffekte, Questzugänge, Status, Talente und Ausrüstung werden erst nach vollständigem Inhaltsabgleich und ausdrücklicher Umsetzung bearbeitet.

Schicksal und Glück dürfen als spätere Spielsysteme ergänzt werden. Ihre genaue Form, Werte, Wiederherstellung und Folgen müssen vor der Implementierung an Lindendorf angepasst und entschieden werden.

## Quellenbereiche

- `src/` und `public/art/` bilden den aktiven implementierten Projektstand.
- `wiki/` enthält relevante Kanon-, Dokumentations-, Planungs- und Arbeitsseiten. Fast alle NPC-Seiten sind für den Abgleich relevant, aber ihre Aussagen müssen gegen Code und aktuelle Projektregeln geprüft werden.
- `docs/` enthält technische und redaktionelle Projektunterlagen.
- `attachments/` enthält das Hauptprojekt ergänzende Arbeitsmaterialien, Entwürfe, Ideen, Volltexte, Medien und Archive. Anhänge sind nicht automatisch veraltet, aber auch nicht automatisch verbindlicher Kanon.
- Ältere Repositories dürfen nützliche Inhalte liefern. Vor einer Übernahme müssen sie mit dem aktiven Code, dem Kanon und den aktuellen Projektregeln verglichen werden.
- Bereits verwendete Audio-, Video- und Bildassets dürfen als aktive Medienreferenzen behandelt werden, wenn sie im Code, in `public/` oder in den aktuellen Assetregistern eingebunden sind.

## Weltwerkzeug

Das Weltwerkzeug soll ausschließlich den bestätigten Lindendorf-Kanon verwalten und anzeigen. Es soll keine unbestätigten Entwürfe, freien Wiki-Ideen oder nicht beschlossenen Erweiterungen als Kanon ausgeben.

Das Weltwerkzeug braucht eine Generalüberholung. Diese Generalüberholung darf nicht stillschweigend eine neue Engine, neue Runtime, neue Authentifizierung, neue Datenbank, neue Routerstruktur, neue Flags oder neue ArtKeys einführen. Zuerst sind Datenquellen, Kanongrenzen, Rollen, Abhängigkeiten und aktuelle Implementierung zu prüfen; danach wird ein separater Umbauplan erstellt.

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
- Wiki-Karrieren, Schicksal, Glück, Status oder soziale Rollen ungeprüft als fertige Regeln behandeln.
- Inhalte aus `export/spielversion1-7170673/` oder alten Repositories ungeprüft in den Hauptbaum übernehmen.
- `text-pack.json` pauschal als alleinigen Kanon behandeln. Es darf alte Sätze nur auflegen, wenn die erste Zeile und die Handlung noch passen; die aktive Kanonfassung muss nachvollziehbar bleiben.

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

Für das Weltwerkzeug zusätzlich die betroffenen Editor-, Welt- und Datenprüfungen ausführen, sobald der konkrete Umbau feststeht.

Grün behaupten nur, wenn der Lauf grün war.
