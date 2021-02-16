---
slug: /posdealers/get-started/after-sales/hardware-tse-reklamation
title: 'Troubleshooting: Hardware TSE Reklamation'
---

# Vorgang bei Hardware TSE und Kartenleser Reklamationen



###### Wenn ein Endkunde sich bei Ihnen meldet, es scheint als stimme mit der Hardware TSE oder dem Kartenleser etwas nicht, bitte ich Sie folgende Tests durchzuführen zu lassen:



- Wird im Betriebssystem ein Laufwerksbuchstabe angezeigt für die TSE? (siehe Beispiel) 

![laufwerksbuchstabe](C:\Users\MichelleLuksch\OneDrive - fiskaltrust consulting gmbh\Dokumente\GitHub\getting-started\posdealers\images\laufwerksbuchstabe.png)

- Haben Sie die Hardware TSE schon an einem anderen SD-Kartenleser/USB Port ausprobiert bzw. einen anderen Kartenleser probiert?
- Wird die Hardware TSE in einem anderen Computer einwandfrei erkannt?

-  Haben Sie schon in den Kartenslot gepustet, um sicherzustellen, dass kein Staub das Problem verursacht? 

- Haben Sie das erweiterte Logging für die Middleware aktiviert? Prüfen Sie bitte ob in dem Log Fehlermeldungen angezeigt werden, welche einen Hinweis auf die Ursache geben können.			

  https://docs.fiskaltrust.cloud/docs/faq/germany#change-the-logging-verbosity

- Manche Kartenleser haben einen eigenen Treiber, der die Verbindung zur Hardware TSE blockieren kann. Hier hilft es oft den eigenen Treiber zu entfernen und durch den Microsoft Standard Treiber zu ersetzen.


- Die Hardware TSE kann nur an einem physischen Computer sicher und einwandfrei angesprochen werden. Das Verbinden des USB-Ports in eine virtuelle Maschine funktioniert bei den meisten virtuellen Umgebungen nicht.




###### Bitte prüfen Sie all diese wesentlichen Punkte sorgfältig, um kostenpflichtige Rückweisungen zu vermeiden.

 Falls all diese Punkte nicht das Problem beheben, bitte ich Sie in Zusammenarbeit mit Ihrem Endkunden folgendes Formular auszufüllen und abzuschicken:	

https://link.fiskaltrust.cloud/tse-rma-request-de
