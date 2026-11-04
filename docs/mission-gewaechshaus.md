# Erste Mission: Die roten Blumentöpfe

> Fachlich geprüft am: 2026-11-04. Spezifikation für den ersten vollständigen Spielabschnitt.

## Anlass und Lernziel

Ein Gewächshausbewohner hat einen Pflanzenhelfer mit Beispielen vorbereitet. Auf der bisherigen Probe wirkt er zuverlässig. Bei neuen Pflanzen werden gesunde Exemplare unnötig behandelt und kranke übersehen.

Der Spieler soll entdecken: In der ursprünglichen Beispielsammlung standen kranke Pflanzen immer in roten Töpfen, gesunde immer in blauen. Der Helfer nutzt die falsche Eigenschaft. Eine neue Probe muss Pflanzenzustand und Topffarbe unabhängig voneinander kombinieren.

## Ablauf

1. In der Werkstatt den Auftrag erhalten und im Gewächshaus den Helfer ausprobieren.
2. Beispiele betrachten: Zustand und Topffarbe sind erkennbar und zusätzlich textlich beschrieben. Der tatsächliche Pflanzenzustand ist die Referenz, die Vorhersage des Helfers wird davon getrennt dargestellt.
3. Eine bekannte, gleichartig verzerrte Probe zeigt eine hohe Trefferquote. Die Anzeige sagt ausdrücklich, auf welchen Beispielen sie beruht.
4. Der Spieler kombiniert gesunde Pflanzen mit roten und kranke Pflanzen mit blauen Töpfen. Die falschen Vorhersagen werden sichtbar; keine Pflanze wird dauerhaft beschädigt.
5. Eine ausgeglichene Beispielsammlung zusammenstellen: gesund/rot, gesund/blau, krank/rot und krank/blau. Anschließend den simulierten Helfer neu vorbereiten.
6. Eine getrennte, zuvor nicht verwendete Prüfung mit anderen Pflanzen durchführen. Trainings- und Prüfdaten sind verschiedene Datensätze; ihre Trennung bleibt technisch erhalten.
7. Vorher/Nachher vergleichen. Eine kurze Entscheidungssituation prüft, ob der Spieler einen neuen Helfer mit 100 Prozent Trefferquote auf bekannten Beispielen sofort einsetzen oder erst unabhängig prüfen würde. Begründung und Experiment bilden gemeinsam den Abschluss.

## Simulationsvertrag

Für die erste Version genügt ein deterministischer, transparenter Lernalgorithmus über vereinfachte Merkmale; keine Bildanalyse und kein Modellanbieter. Der genaue Algorithmus wird im Logik-Ticket festgelegt und dokumentiert. Er muss die falsche Abkürzung aus den Anfangsbeispielen tatsächlich ableiten und bei hinreichend geeigneten Beispielen das Zustandsmerkmal wählen. Ein bloßer Missionsschalter, der nach einer Dialogantwort alle Vorhersagen korrigiert, erfüllt das Ziel nicht.

Die vereinfachte Darstellung macht Pflanzenzustand und Topffarbe kontrollierbar. Texte nennen den Helfer eine Simulation. Das Spiel behauptet weder, dass reale Modelle genau so lernen, noch dass eine ausgeglichene Beispielsammlung jeden KI-Fehler beseitigt.

## Prüffälle

- Die ursprüngliche Beispielsammlung besteht die bekannte Probe, scheitert aber an den vertauschten Töpfen.
- Nur mehr Beispiele derselben Verzerrung hinzuzufügen behebt den Fehler nicht.
- Eine geeignete Sammlung verbessert die getrennte Prüfung; die Auswertung zeigt richtige und falsche Fälle samt Nenner.
- Ein einzelner Gegenfall darf nicht pauschal als vollständige Reparatur gelten.
- Prüfpflanzen dürfen nicht in den Trainingspool verschoben werden, um das Ergebnis zu schönen.
- Wiederholen und Neustarten stellt einen reproduzierbaren Ausgangszustand her.
- Dialoge, Topfmerkmale und Entscheidungen sind ohne Farberkennung verständlich.
- Ein Reload nach Abschluss darf nicht unbeabsichtigt einen falschen Abschluss anzeigen. Persistenz ist kein Bestandteil des ersten Abschnitts; ein Neustart darf ausdrücklich neu beginnen.

## Abnahme im Browser

Eine Person kann den vollständigen Weg ohne Entwicklerkonsole spielen. Tastatur und Zeiger funktionieren. Der Fehler vor der Verbesserung und der unabhängige Vergleich danach sind sichtbar. Kein unlösbarer Zwischenzustand; Neustart ist erreichbar. Zusätzlich zur Browserprüfung erfolgt ein fachlicher Review auf irreführende KI-Aussagen.
