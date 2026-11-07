# Lumina – die Stadt der denkenden Maschinen

> Fachlich geprüft am: 2026-11-04. Produktvision; Name ist ein Arbeitstitel, seine Verfügbarkeit wurde nicht geprüft.

## Versprechen

Ein gemütliches 2D-Abenteuer, in dem Erwachsene ohne KI-Vorkenntnisse durch Ausprobieren lernen, KI sinnvoll einzusetzen und ihre Grenzen zu erkennen. Fachbegriffe werden erst eingeführt, nachdem der Spieler das zugehörige Problem erlebt hat.

Du kommst als neues Mitglied in eine Erfinderwerkstatt. Die Stadt bereitet ein Fest vor. Mechanische Helfer unterstützen die Bewohner, machen aber nachvollziehbare Fehler. Du erkundest die Stadt, sammelst Informationen, probierst Lösungen aus und beobachtest die Folgen. Die Werkstatt ist dein Ausgangspunkt; gelöste Aufgaben verändern die Stadt sichtbar.

## Spielschleife

Beobachten → mit Bewohnern sprechen → Informationen oder Beispiele sammeln → Helfer ausprobieren → Ergebnis untersuchen → gezielt verbessern → an neuen Fällen prüfen.

Das Spiel besteht aus räumlichen Interaktionen und Experimenten. Dialoge erklären den Anlass. Ein Quiz oder das Zusammensetzen eines vermeintlich perfekten Prompts ersetzt das Experiment nicht. Fehler dürfen folgenlos zurückgesetzt und verglichen werden; Schnelligkeit wird nicht belohnt.

## Stadt und Lernziele

| Ort | Spielproblem | Lernziel |
| --- | --- | --- |
| Werkstatt | Helfer vorbereiten, Experimente wiederholen und vergleichen | Ziel, Randbedingungen und Erfolgskriterien unterscheiden |
| Gewächshaus | Pflanzenhelfer verwechselt Topffarbe und Pflanzenzustand | Verzerrte Daten, Abkürzungen und unabhängige Testfälle erkennen |
| Lieferhof | Ein Roboter bekommt einen unvollständigen Auftrag | Kontext, Grenzen und nötige Rückfragen erkennen |
| Stadtarchiv | Überzeugende Geschichten widersprechen den Quellen | Behauptungen prüfen und Unsicherheit ausdrücken |
| Fabrikviertel | Mehrere Maschinen übergeben sich Arbeit und vervielfachen einen Fehler | Arbeitsschritte, Übergaben, Prüfpunkte und menschliche Entscheidungen gestalten |

Die Fabrik ist ein späterer begehbarer Stadtteil des Spiels. Sie ist fachlich vom Entwicklungswerkzeug „Agenten-Fabrik“ zu unterscheiden. Spieler sollen dort eine kleine Produktionskette aufbauen und beobachten können, wie ein ungeprüfter Fehler weitergereicht wird. Konkrete Produktionsmechanik und Lerninhalt werden erst nach dem Gewächshaus ausgearbeitet.

## Erster Spielabschnitt

Werkstatt als Einstieg und ein Gewächshaus mit einem Bewohner, einem Pflanzenhelfer und einer vollständigen Mission. Zielumfang: ungefähr zehn bis fünfzehn Minuten, anschließend durch Spieltests prüfen. Der genaue Ablauf steht in [Gewächshaus](mission-gewaechshaus.md).

Erfolg bedeutet: Der Spieler kann eine irreführende hohe Trefferquote durch einen eigenen Gegenversuch hinterfragen, die Beispielsammlung verbessern und die Verbesserung an vorher ungesehenen Pflanzen prüfen.

## Gestaltung

Gemütliche, farbige Stadt mit kleinen mechanischen Helfern, klarer Silhouette und gut lesbaren Texten. Eigene Orte, Figuren und Gestaltung. Interaktionen müssen sowohl mit Tastatur als auch mit Zeiger bedienbar sein. Farbe allein darf keine für die Lösung nötige Information tragen. Dialoge müssen ohne Zeitdruck lesbar sein.

## Grenzen der ersten Version

Keine offene Welt, kein Crafting- oder Wirtschaftssystem, keine Multiplayer-Funktion, keine echten KI-APIs und kein Benutzerkonto. Die KI-Mechanik wird als didaktische Simulation kenntlich gemacht. Begrenzungen realer Systeme werden nicht als universelle Gesetzmäßigkeiten aus der Simulation abgeleitet.

Weitere Stadtteile und eine bebaubare Fabrik bleiben Erweiterungen. Laufende Reihenfolge, Blocker und Implementierungsstand stehen ausschließlich im GitHub-Board.
