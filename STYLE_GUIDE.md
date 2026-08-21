# Echo-Station Statusseite – Gestaltungsregeln

Diese Regeln gelten für die statische Statusseite in `index.html`.

## Verbindlicher Stand

Das mit dem Statusseiten-Commit vom August 2026 eingeführte Erscheinungsbild ist die feste Grundlage für alle weiteren Aktualisierungen. Künftige Arbeiten aktualisieren in erster Linie Texte, Statusangaben und den Fahrplan. Eine Neugestaltung erfolgt nur nach ausdrücklicher Freigabe.

## Design nicht verändern

Folgende Elemente bleiben erhalten:

- warme, ruhige Beige-/Teal-Farbpalette;
- Boska als Überschriftenschrift und Satoshi als Textschrift;
- Sticky-Header mit Logo, Seitennavigation und Farbschema-Schalter;
- heller und dunkler Darstellungsmodus;
- großzügiger Hero-Bereich;
- Statuskarten mit kompakten Badges;
- Listen mit grünen Häkchen für abgeschlossene Arbeiten;
- vertikaler Fahrplan für die nächsten Schritte;
- responsive Darstellung für Desktop und Mobilgeräte;
- schlichter Footer `Echo-Station · Stand <Monat Jahr>`.

Ohne ausdrückliche Freigabe werden keine Farben, Schriften, Abstände, Kartenformen, Navigationselemente oder Seitenbereiche grundlegend ersetzt.

## Erlaubte Aktualisierungen

Reguläre Statusupdates dürfen:

- bestehende Texte sachlich aktualisieren;
- neue abgeschlossene Meilensteine unter „Bisher umgesetzt“ ergänzen;
- Status-Badges passend ändern;
- erledigte Fahrplanpunkte verschieben oder neue nächste Schritte ergänzen;
- den Monat im Footer aktualisieren;
- kleine Fehler bei Rechtschreibung, Barrierefreiheit oder responsiver Darstellung korrigieren.

## Inhalt und Sprache

Die Seite richtet sich an ein gemischtes Team. Nicht alle Leser sind technisch versiert.

- kurz, sachlich und verständlich schreiben;
- erklären, welchen Nutzen eine Funktion hat;
- technische Begriffe nur verwenden, wenn sie notwendig sind;
- keine werblichen, pathetischen oder selbstbezogenen Formulierungen;
- keine Fülltexte wie „gehört zur Geschichte und zum Fundament“;
- keine unnötigen Wiederholungen zwischen Status, Meilensteinen und Fahrplan.

Bevorzugte Überschriften sind beispielsweise:

- `Aktueller Stand`
- `Funktionsübersicht`
- `Bisher umgesetzt`
- `Abgeschlossene Arbeiten im Überblick.`
- `Nächste Schritte`

## Keine flüchtigen oder internen Details

Auf der Statusseite erscheinen grundsätzlich nicht:

- Commit-SHAs, Branch-Namen oder GitHub-Arbeitsstände;
- interne Dateipfade, Ports, Service-Namen oder SSH-Details;
- Passwörter, Tokens, private Adressen oder Betriebsgeheimnisse;
- kurzlebige Bestandszahlen und momentane Einzelwarnungen;
- technische Migrationsnummern oder detaillierte Rollout-Protokolle.

Stattdessen werden stabile Aussagen verwendet, zum Beispiel: „Der Katalog wird automatisch geprüft“ oder „Wichtige Einstellungen werden regelmäßig gesichert“.

## Historie bewahren

Abgeschlossene Arbeiten werden nicht stillschweigend entfernt. Wenn ein früherer technischer Weg durch eine neue Lösung ersetzt wird, bleibt der erreichte Meilenstein in verständlicher Form erhalten. Veraltete Betriebsdetails werden dabei entfernt oder als früherer Projektstand eingeordnet.

## Arbeitsweise

1. Vor jeder Änderung den aktuellen Code und die letzten Statusseiten-Commits prüfen.
2. Produkt-Repository und Status-Repository niemals im selben Task verändern.
3. Änderungen möglichst als inhaltlichen Diff halten.
4. Vor dem Commit Navigation, Anker, Dark Mode, Desktop- und Mobilansicht prüfen.
5. `git diff --check` ausführen und sicherstellen, dass keine internen Details veröffentlicht werden.
6. Designänderungen nur nach separater ausdrücklicher Freigabe durchführen.
