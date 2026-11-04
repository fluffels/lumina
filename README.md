# Lumina – die Stadt der denkenden Maschinen

Ein gemütliches 2D-Lernspiel über den sinnvollen Umgang mit KI. Du hilfst den Bewohnern einer Stadt, untersuchst die Fehler ihrer mechanischen Helfer und verbesserst deren Arbeit durch eigene Experimente.

Der erste Spielabschnitt führt von der Werkstatt ins Gewächshaus: Ein Pflanzenhelfer verwechselt Topffarbe und Pflanzenzustand. Später können Lieferhof, Stadtarchiv und ein bebaubares Fabrikviertel folgen.

## Projektunterlagen

- [Spielidee und Welt](docs/spielidee.md)
- [Erste Mission: Die roten Blumentöpfe](docs/mission-gewaechshaus.md)
- [Technischer Einstieg](docs/technik.md)
- [Claude-/Codex-Pilot und Abnahme](docs/fabrik-pilot.md)
- [Arbeitsanweisung](AGENTS.md) und [Projekt-Brain](docs/referenz/anlaufstellen.md)
- [Backlog und Reihenfolge](https://github.com/users/fluffels/projects/4)

## Einrichtung

Node gemäß `engines.node` in `package.json` verwenden; `.nvmrc` legt Node 24 als Entwicklungsstand fest.

```sh
npm ci
npm run verify
```

Diese Prüfung umfasst die Einrichtungsbasis und den Factory-Bezug. Es gibt noch kein spielbares Produkt und noch keinen `dev`- oder `build`-Befehl. Das [Spielgerüst-Ticket](https://github.com/fluffels/lumina/issues/3) führt TypeScript, Phaser, Vite und die vollständigen Produktprüfungen ein.

## Gemeinsame Agenten-Fabrik

Factory-Besitz ist aus dem Tag `v0.8.0` des Repositories `fluffels/self-improving-agent-harness-and-factory` synchronisiert. Regeln und Werkzeuge werden dort weiterentwickelt und über den regulären Sync übernommen. `npm run check:factorydrift` prüft die unveränderte Herkunft; `npm run skills:sync -- --check` die Skill-Zeiger.

Der [Codex-Einstieg](docs/codex/einstieg.md) ist ein Prototyp mit gesperrtem autonomem Ticketlauf. Die [Lumina-Einrichtung](https://github.com/fluffels/lumina/issues/2) muss reale Rollen, Dienste und Freigaben nachweisen. Kubernia und Speaker-Tooling werden durch dieses Projekt nicht verändert.

Repository und Board bleiben privat. Die aktuelle GitHub-API verweigert Rulesets für dieses private Repository mit einem Upgrade-Hinweis; Branch-Erzwingung ist daher noch nicht eingerichtet. `PROJECT_TOKEN` und der projektbezogene Langfuse-Nachweis fehlen ebenfalls. Diese Grenzen sind in Ticket 2 festgehalten. Secret-Scan und Dependabot-Inbox sind übernommen; optionale Module mit nicht nachgewiesenen privaten Code-Scanning-Voraussetzungen sind nicht aktiviert.

## Erste Meilensteine

1. **Gewächshaus:** Gerüst, lernende Simulation, vollständige Mission und unabhängige Abnahme.
2. **Fabrik-Pilot:** Laufumgebung nachweisen, danach freigegebene Codex-Aufträge und Übergaben zwischen Claude und Codex prüfen.
3. **Stadt erweitern:** Archiv und Fabrikviertel nach dem ersten Spielabschnitt ausarbeiten.

Der Name ist ein Arbeitstitel. Eine Namens- oder Rechteprüfung ist noch nicht erfolgt. Es wird keine Open-Source-Lizenz erteilt.
