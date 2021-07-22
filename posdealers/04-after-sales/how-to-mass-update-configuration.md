---
slug: /posdealers/get-started/after-sales/mass-configuration-update
title: 'How-To: Massenupdate von CashBoxen'
---

# How-To: Massenupdate von CashBoxen

Für einen Massenupdate bereits ausgerollter CashBoxen stellt fiskaltrust unter dem Portalmenüpunkt ```Konfiguration -> Update``` die Möglichkeit zur Verfügung viele der CashBoxen gleichzeitig zu aktualisieren. 

Wird zum Beispiel eine neue Package Version des Persistenzlayer benötigt, so kann diese für alle betroffenen CashBoxen gleichzeitig aktualisiert werden:



![Massenupdate](../02-pre-sales/media/mass-update.png)



Im oben dargestellten Screenshot wird für alle Queues mit der `fiskaltrust.Middleware.Queue.SQLite` Package Version 1.3.3 die Konfiguration auf die Version 1.3.5 upgedatet. Zusätzlich werden automatisch die entsprechenden CashBoxen aktualisiert und zusammengebaut (siehe Rebuild Configuration checkbox rechts).

Um die neuen Konfigurationen wirksam werden zu lassen, müssen folgende Schritte vorgenommen werden:

1. Rebuild Configuration für die CashBox im fiskaltrust.Portal (Zusammenbauen/Aktualisieren der CashBox)
2. Stoppen der Middleware und Neustart des Launchers an der Kasse. 

Der Launcher lädt daraufhin automatisch die neue Version der CashBox, wendet diese an und startet die Middleware mit der neuen Konfiguration.

