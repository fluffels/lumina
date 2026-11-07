# Pilot für Claude und Codex

> Fachlich geprüft am: 2026-11-04. Ziel und Abnahmevertrag; laufende Ergebnisse gehören in Issues und Pull Requests.

## Zweck

Lumina ist ein abgegrenztes neues Produktprojekt. Bestehende andere Projekte und der Factory-Kern werden durch diesen Pilot nicht umgebaut. Die Fabrik soll dieselben verbindlichen Phasen und Qualitätsanforderungen für Claude und Codex tragen. Rollen, Hook-Registrierungen und Werkzeuge dürfen sich je Laufzeit unterscheiden.

Der bekannte TypeScript-/Phaser-/Vite-Stack reduziert gleichzeitige Änderungen. Ein anderer Stack wird erst nach belastbaren Durchläufen geprüft. Es entsteht kein zweiter Orchestrator und kein Ersatzwerkzeug zum Umgehen einer fehlenden Fähigkeit.

## Gemeinsame Quelle

Factory-Besitz kommt aus einem veröffentlichten Tag per `factory-sync`. Herkunft und Hashes stehen in `.factory/sync-stand.json`. Das Projekt pflegt Produktregeln und seine Konfiguration. Änderungen am Kern werden upstream umgesetzt, vorerst durch Claude, und anschließend per Tag übernommen.

Der verbindliche Codex-Stand und die offenen Nachweisgrenzen stehen im [synchronisierten Einstieg](codex/einstieg.md). Eine erfolgreiche Synchronisation, vorhandene Rollen-Dateien oder grüne lokale Prüfungen erteilen keine autonome Freigabe.

## Reihenfolge der Nachweise

1. Einrichtung: Regelquellen, Skills, Projektzuordnung, Board und Factory-Herkunft sind nachvollziehbar; nötige Dienste und Rollen werden in der wirklichen Zielsession geprüft.
2. Factory-Gesamtabnahme: tatsächliche Hooks, Rechtebegrenzung, unabhängige Review-/Holdout-Rollen und Tracing einschließlich Ausfall- und Negativfällen bestehen die dort geforderte Abnahme. Bis dahin keine autonomen Codex-Ticketläufe.
3. Codex allein: mehrere abgegrenzte Produktaufträge vollständig nach dem freigegebenen Ablauf erledigen. Auftragstreue, Nacharbeit, nötige Eingriffe, tatsächlicher Aufwand und Prüfnachweise erfassen.
4. Übergaben: Codex übernimmt einen von Claude hinterlassenen Stand und umgekehrt. Kontext aus Repository und Ticket reicht für die Fortsetzung; ein privater Chat ist keine versteckte Voraussetzung.
5. Parallelität: getrennte Tickets, atomare Claims und getrennte Worktrees; keine gegenseitigen Dateiänderungen oder aufgeräumten fremden Arbeitsstände.

Ein manueller Schritt wird als manueller Schritt dokumentiert. Er ist kein Beleg für einen automatisch wirksamen Hook. „Nicht geprüft“ und „fehlgeschlagen“ bleiben unterscheidbar.

## Befundformat

Pro Abweichung: Session und Laufzeitversion, konkreter Auftrag, erwartete Phase, tatsächliches Verhalten, reproduzierbarer Beleg, Auswirkung, vorhandenes zuständiges Factory-Issue und nächster prüfbarer Schritt. Keine Secrets, privaten Pfade oder vollständigen Transkripte in Issues kopieren.

Kernbefunde werden in vorhandene Factory-Arbeit eingeordnet. Produktspezifische Fehler werden Lumina-Tickets. Die erste Einrichtung wird nicht als Beleg für einen autonomen Produktlauf gezählt.
