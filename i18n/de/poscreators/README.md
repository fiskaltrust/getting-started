---
slug: /poscreators/get-started
title: Get started für KassenHersteller
---

# Erste Schritte für KassenHersteller

## Übersicht

Dieser Leitfaden stellt KassenHerstellern eine Übersicht der von uns empfohlenen Phasen bzw. Schritte der Integration mit fiskaltrust zur Verfügung. Er baut auf unsere [Lead Presentation für KassenHersteller](lead-presentation.md) auf, welche wir als Vorlektüre empfehlen.

Im Einzelnen sind folgende Schritte zu durchlaufen:

![integration phases](images/pos-creator-integration-phases-de.png)

1. [Registrierung im Live Portal](#registrierung-im-live-portal)
2. [Registrierung im Sandbox Portal](#registrierung-im-sandbox-portal)
3. [Integration der fiskaltrust.Middleware ins Kassensystem](#integration-der-fiskaltrustmiddleware-ins-kassensystem)
4. [Onboarding der KassenHändler](#onboarding-der-kassenhändler)
5. [Pilotinstallation](#pilotinstallation)
6. [Handover zum Rollout an den KassenHändler](#handover-zum-rollout-an-den-kassenhändler)

Im Folgenden werden wir auf die einzelnen Schritte detailierter eingehen.

## Registrierung im Live Portal

### Firmendaten und Kooperationsvertrag

Um kostenlosen KassenHersteller-Support von fiskaltrust zu erhalten, müssen Sie sich zuerst in unserem fiskaltrust.Portal registrieren. Dieses finden Sie unter  [https://portal.fiskaltrust.de](https://portal.fiskaltrust.de/). 

Sobald Sie sich im fiskaltrust.Portal registriert haben, wird Ihnen ein Formular zur Auswahl Ihrer Rolle angezeigt. Wählen Sie die Option "KassenHersteller" und unterschreiben Sie unseren Kooperationsvertrag, indem Sie Ihren Namen ins Eingabefeld eingeben. Sollten Sie zudem auch KassenHändler sein, wählen Sie bitte danach auch diese Option aus. 

Durch die Registrierung im Live fiskaltrust.Portal und die digitale Unterschrift unseres Kooperationsvertrags sind sie nun berechtigt unseren kostenlosen KassenHersteller-Support für Einrichtungsfragen und Onboarding in Anspruch zu nehmen. Sie können unser Support-Team unter [info@fiskaltrust.de](mailto:info@fiskaltrust.de) erreichen.

### Registrieren Ihres Kassensystems

Registrieren bzw. Erfassen Sie als Nächstes Ihr(e) Kassensystem(e) unter dem Menüpunkt "Kassensysteme". 

## Registrierung im Sandbox Portal

Nach der Registrierung im Live fiskaltrust.Portal wiederholen Sie die oben beschriebenen Schritte zur Registrierung im Sandbox fiskaltrust.Portal [https://portal-sandbox.fiskaltrust.de](https://portal-sandbox.fiskaltrust.de/). Dadurch erhalten Sie Zugriff auf unsere Testumgebung und können zuerst dort, zum Testen, die Integration der fiskaltrust.Middlware und die technische Vorbereitung des Rollout vornehmen.


## Integration der fiskaltrust.Middleware ins Kassensystem

Die fiskaltrust.Middleware bietet Ihnen Compliance-as-a-Service im Fiskalisierungsbereich. Sie muss dafür in Ihr Kassensystem integriert werden. In unserer [Anleitung zur Integration der fiskaltrust.Middleware](middleware-integration.md) stellen wir Ihnen diesbezüglich eine detaillierte Anleitung zur Anbindung und zur Kommunikation mit der fiskaltrust.Middleware zur Verfügung. Sobald Sie die normalen, "einfachen" Vorgänge Ihres Kassensystems abgebildet haben, empfehlen wir Ihnen parallel zur Weiterentwicklung bereits mit dem nächsten Schritt (Oboarding der KassenHändler) zu starten.

## Onboarding der KassenHändler

Schon während der Integration der fiskaltrust.Middleware, bzw. sobald Sie Ihre "Make-or-Buy" Entscheidung getroffen haben, empfehlen wir Ihnen mit dem Onboarding Ihrer KassenHändler zu beginnen, damit Sie sich rechtzeitig, gemeinsam mit Ihren KassenHändler, auf den Rollout vorbereiten. 

Es ist wichtig Ihre KassenHändler möglichst früh einzubeziehen, denn die KassenHändler müssen unter anderen folgende Schritte absolvieren bevor Sie die fiskaltrust.Middleware an die KassenBetreiber ausrollen können:

1. Registrierung im fiskaltrust.Portal und digitale Unterzeichnung des fiskaltrust KassenHändler Kooperationsvertrags.
2. Je nach Gegebenheiten und geplanten Einkaufsmengen muss durch den KassenHändler einen Rahmenvertrag bezüglich der Abnahmemengen über einen bestimmten Zeitraum und den dazugehörigen Mengenrabatten von fiskaltrust angefordert, ausgehandelt und unterzeichnet werden.
3. Der KassenHändler muss alle KassenBetreiber ins fiskaltrust fiskaltrust.Portal einladen, wo diese vor dem Rollout die Nutzungsvereinbarung für die fiskaltrust.Middleware unterzeichnen müssen.
4. Zugriffsrechte von den  KassenBetreiber auf Ihre Accounts anfordern, so dass der KassenHändler im  Namen des KassenBetreibers Produktansprüche (Entitlements) einlösen und  aktivieren kann.
5. Zugriffsrechte von den  KassenBetreiber auf Ihre Accounts anfordern, so dass der KassenHändler im  Namen des KassenBetreibers die Konfiguration der fiskaltrust.Middleware Instanzen vornehmen kann, die dann beim KassenBetreiber installiert werden.
6. Für den korrekten DSFinV-K Export muss der KassenHändler die Angaben aus dem Kassensystem mit den Stammdaten des KassenBetreibers im fiskaltrust.Portal verknüpfen.
7. Technische Planung und Vorbereitung für den Rollout zusammen mit dem KassenHersteller.

Die oben dargestellten Schritte können sehr zeitaufwendig sein. Deshalb empfehlen wir dringen, dass Sie Ihre KassenHändler früh informieren und insbesondere sie so früh wie möglich im fiskaltrust.Portal einladen, so dass die KassenHändler mit Ihren Vorbereitungen beginnen können.

## Lösung komplexer Business Cases

In jeder Branche können spezifische und komplexe Geschäftsfälle vorkommen, die eine besondere Behandlung in Bezug auf die Anfragen an die fiskaltrust.Middleware erfordern. Sollten Sie Unterstützung bei der korrekten Handhabung solcher komplexen Fälle benötigen, kontaktieren Sie bitte unter <a href="mailto:support@fiskaltrust.de">support@fiskaltrust.de</a> unser Support Team. Wir unterstützen Sie gerne bei der Abbildung.

## Pilotinstallation

Nachdem Sie die Integration der fiskaltrust.Middleware vorgenommen und getestet haben, Ihre KassenHändler einbezogen haben und mit diesen den Rollout vorbereitet haben, indem Sie zum Beispiel Templates zur Automatisierung vorbereitet und getestet haben, empfehlen wir Ihnen gemeinsam mit Ihren KassenHändler eine Pilotinstallation bei einem Kunden vorzunehmen. Damit können Sie Ihre Implementierung und den Rollout im Echtbetrieb testen und die KassenHändler auf die Übergabe zum Massenrollout vorbereiten.

## Handover zum Rollout an den KassenHändler

Sobald eine erfolgreiche Pilotinstallation in Zusammenarbeit mit Ihren KassenHändler durchgeführt wurde, können Sie nun die Übergabe zum Massenrollout an Ihre KassenHändler vornehmen.

## Weiterführende Informationsquellen

- Deutsche fiskaltrust Website: [https://fiskaltrust.de](https://fiskaltrust.de/)
- fiskaltrust Dokumentations-Plattform: [https://docs.fiskaltrust.cloud](https://docs.fiskaltrust.cloud/)
- FAQ: [ fiskaltrust.DocumentationPortal  - faq](https://docs.fiskaltrust.cloud/doc/faq/qna/market-de.html) und [Github faq repo](https://github.com/fiskaltrust/faq) zum Anlegen von Issues (Fragen).
- fiskaltrust Gihub repos: [https://github.com/fiskaltrust](https://github.com/fiskaltrust)
- fiskaltrust Videos: [Youtube Channel](https://www.youtube.com/channel/UCmMlqO4L3AzkEhh6WYA8BJg)



