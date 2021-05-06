---
slug: /posdealers/get-started/after-sales/switch-scu
title: 'How-To: SCU austauchen'
---

# How-To: SCU austauchen

Diese Anleitung beschreibt, wie Sie in einer Cashbox die Zuordnung einer Queue zur verwendeten SCU mit einer neuen SCU austauschen. Voraussetzung hierfür ist, dass sich die Queue und die SCU(s) in derselben Cashbox befinden.
Das hier beschriebene Feature ist hilfreich für den Fall, dass Sie eine TSE austauschen möchten.

## Schritte

Generell sind zwei Fälle für den Austausch zu unterscheiden:

1. Die Queue ist noch nicht aktiv (Inbetriebnahme-Beleg wurde noch nicht gesendet)
2. Die Queue ist bereits aktiv (Inbetriebnahme-Beleg wurde bereits gesendet)

## Queue ist noch nicht aktiv

Im diesem Fall ist der Austauch unkompliziert und besteht aus folgenden Schritten:

1. Alte SCU aus der Cashbox entfernen
2. Neue SCU in die Cashbox einfügen
3. Queue mit neuer SCU verbinden
4. Konfigurationsänderung publizieren (rebuild configuration)
5. fiskaltrust Service neu starten

## Queue ist bereits aktiv

Im Falle, dass die Queue bereits aktiv ist, müssen Sie wie folgt vorgehen:

1. Neue SCU der Cashbox hinzufügen (alte SCU nicht aus der Cashbox entfernen)
2. Die Queue mit der neuen SCU verbinden
3. Konfigurationsänderung publizieren ("Rebuild configuration)"
4. fiskaltrust Service neu starten
5. Tagesabschlußbeleg (daily-closing) an die Queue senden, um die Daten der alten SCU zu sichern
6. Beleg zur Initialisierung des Tauschs (initiate-switch-receipt) an die Queue senden
7. Beleg zum Abschließen des Tauschs (finish-switch-receipt) an die Queue senden
8. Im fiskaltrust.Portal die alte SCU aus der Cashbox löschen
9. Konfigurationsänderung publizieren ("Rebuild configuration")
10. fiskaltrust Service neu starten
11. Initialisierungsbeleg (initial-operation) an die Queue senden

Die oben genannten Belegtypen müssen vom KassenHersteller im POSSystem implementiert worden sein. Eine detailierte Beschreibung der genannten Belegtypen finden Sie in unserer [Middleware API Dokumentation](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/germany/reference-tables/ftreceiptcase) für KassenHersteller.

