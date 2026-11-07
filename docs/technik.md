# Technischer Einstieg

> Fachlich geprüft am: 2026-11-04. Einrichtung vor dem ersten Produktcode.

## Festgelegter Stack

TypeScript, Phaser und Vite für das Browser-Spiel. Vitest für die zustandsbasierte Spiellogik und Playwright für die spielbare Strecke. Die konkreten Versionen und der vollständige Lockfile werden im Gerüst-Ticket eingeführt und geprüft. Bis dahin benötigt die Einrichtungsbasis nur Node und `yaml`, das die übernommenen Factory-Werkzeuge verwenden.

## Geplante Trennung

- `src/domain/`: Pflanzenmerkmale, Beispielsammlungen, simuliertes Lernen, Vorhersage und Missionszustand; ohne Phaser oder Browser-DOM.
- `src/game/`: Szenen, Eingabe, Figuren, Darstellung und Dialoganzeige; verwendet die Domänenlogik.
- `src/content/`: Dialoge und Missionsdaten; ohne eingebettete Ablaufsteuerung.
- `test/`: sinnvolle Domänen- und Regressionstests.
- `e2e/`: Browserprüfung des vollständigen Spielabschnitts.

Diese Ordner sind eine Planung und werden zusammen mit ihrem ersten Inhalt angelegt. Der Gerüst-Auftrag prüft die Grenzen mit dem vorhandenen Factory-Werkzeugbestand.

## Einrichtungsprüfung

`npm ci` installiert die gelockten Einrichtungsabhängigkeiten. `npm run verify` prüft Factory-Drift, Factory-Links, Skill-Zeiger, Kontextgröße, Steuerzeichen, interne Referenzen, Lockfile und Diff-Größe. Diese Befehle testen kein Spiel. Vor dem ersten Produktcode erweitert das Gerüst-Ticket die Verifikation um Typprüfung, Lint, Tests und Build; Browserabnahme gehört zur ersten bedienbaren Ausgabe.

Die lokalen Factory-Syncs werden mit `npm run factory:sync -- --quelle <Factory-Klon> --tag <Tag>` ausgeführt. Absolute Pfade werden nicht in die Projektkonfiguration geschrieben.

## Dienste und Rechte

Es werden keine Zugangsdaten aus anderen Projekten kopiert. Die Einrichtung von Langfuse, privaten Projekt-Token und wirksamen Laufzeitrechten wird getrennt nachgewiesen. Das vorhandene GitHub-CLI-Login ist kein Nachweis dafür, dass GitHub Actions das persönliche Project-Board bearbeiten darf. Fehlende `PROJECT_TOKEN`-Berechtigungen bleiben als Einrichtungslücke sichtbar.
