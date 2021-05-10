---
slug: /posdealers/get-started/after-sales/switch-scu
title: 'How-To: SCU austauschen'
---

You can find the english version of the scu switch guide [here](https://docs.fiskaltrust.cloud/docs/posdealers/rollout-doc/how-to/switch-scu).

# How-To: SCU austauschen

Diese Anleitung beschreibt, wie Sie in einer Cashbox die Zuordnung einer Queue zur verwendeten SCU mit einer neuen SCU austauschen. Das hier beschriebene Feature ist hilfreich für den Fall, dass Sie eine TSE austauschen möchten.

## Schritte

Generell sind zwei Fälle für den Austausch zu unterscheiden:

1. Die Queue ist noch nicht aktiv (Inbetriebnahme-Beleg wurde noch nicht gesendet)
2. Die Queue ist bereits aktiv (Inbetriebnahme-Beleg wurde bereits gesendet)

## Queue ist noch nicht aktiv

### SCU befindet sich in derselben Cashbox wie die Queue

Im diesem Fall ist der Austauch unkompliziert und besteht aus folgenden Schritten:

1. Alte SCU aus der Cashbox entfernen
2. Neue SCU in die Cashbox einfügen
3. Queue mit neuer SCU verbinden
4. Konfigurationsänderung publizieren ("Rebuild configuration")
5. fiskaltrust.Middleware neu starten

### SCU befindet sich in einer anderen Cashbox

1. Queue mit neuer SCU verbinden
4. Konfigurationsänderung publizieren ("Rebuild configuration")
5. fiskaltrust.Middleware neu starten

## Queue ist bereits aktiv

Im Falle, dass die Queue bereits aktiv ist, wird der Austausch in einem zweistufigen Prozess vorgenommen. Dies ermöglicht den einfachen Wechsel einer Hardware-TSE, falls dafür nur ein Steckplatz im Rechner zur Verfügung steht und somit nur eine der beiden Hardware-TSEs (alt oder neu) angesteckt werden kann. Ein solcher Wechsel der Hardware-TSE wird nach dem Senden des Belegs zur Initialisierung des Tauschs und vor dem Senden des Belegs zum Abschließen des Tauschs vorgenommen (s.u.).

Um den Austausch der SCU vorzunehmen, gehen Sie wie folgt vor:

### SCU befindet sich in derselben Cashbox wie die Queue

1. Neue SCU der Cashbox hinzufügen (alte SCU nicht aus der Cashbox entfernen)
2. Die Queue mit der neuen SCU verbinden
3. Konfigurationsänderung publizieren ("Rebuild configuration")
4. fiskaltrust.Middleware neu starten
5. Tagesabschlußbeleg (daily-closing) an die Queue senden, um die Daten der alten SCU zu sichern
6. Beleg zur Initialisierung des Tauschs (initiate-switch-receipt) an die Queue senden
(Anmerkung: Falls es hierbei um den Wechsel einer Hardware-TSE geht und im Rechner nur ein Steckplatz zur Verfügung steht, wechseln Sie nach dem Senden des Belegs zur Initialisierung des Tauschs die Hardware-TSE aus - alt gegen neu )
7. Beleg zum Abschließen des Tauschs (finish-switch-receipt) an die Queue senden
8. Im fiskaltrust.Portal die alte SCU aus der Cashbox löschen
9. Konfigurationsänderung publizieren ("Rebuild configuration")
10. fiskaltrust.Middleware neu starten

Die oben genannten Belegtypen müssen vom KassenHersteller im POSSystem implementiert worden sein. Eine detailierte Beschreibung der genannten Belegtypen finden Sie in unserer [Middleware API Dokumentation](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/germany/reference-tables/ftreceiptcase) für KassenHersteller.

### SCU befindet sich in einer anderen Cashbox

1. Die Queue mit der neuen SCU verbinden
2. Konfigurationsänderung publizieren ("Rebuild configuration")
3. fiskaltrust.Middleware neu starten
4. Tagesabschlußbeleg (daily-closing) an die Queue senden, um die Daten der alten SCU zu sichern
5. Beleg zur Initialisierung des Tauschs (initiate-switch-receipt) an die Queue senden
(Anmerkung: Falls es hierbei um den Wechsel einer Hardware-TSE geht und im Rechner nur ein Steckplatz zur Verfügung steht, wechseln Sie nach dem Senden des Belegs zur Initialisierung des Tauschs die Hardware-TSE aus - alt gegen neu )
6. Beleg zum Abschließen des Tauschs (finish-switch-receipt) an die Queue senden

Die oben genannten Belegtypen müssen vom KassenHersteller im POSSystem implementiert worden sein. Eine detailierte Beschreibung der genannten Belegtypen finden Sie in unserer [Middleware API Dokumentation](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/germany/reference-tables/ftreceiptcase) für KassenHersteller.
