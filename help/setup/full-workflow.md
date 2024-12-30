---
title: GitHub-Beitragsarbeitsablauf für umfangreiche Änderungen
description: Erfahren Sie, wie Sie über Experience League Beiträge zur Adobe-Dokumentation leisten können.
exl-id: ad467ad4-abd2-4166-8659-e29c48d268ec
source-git-commit: a3c283c5c0d181beacc566262743528d5ff9f7d2
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 96%

---

# GitHub-Beitragsarbeitsablauf für umfangreiche Änderungen

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Überblick

Dieser Arbeitsablauf eignet sich für einen Mitarbeiter, der eine umfangreiche Änderung vornehmen muss oder häufig zum Repository beitragen wird. Mitarbeiter mit häufig vorgenommenen Beiträgen verfügen normalerweise über kontinuierliche (langfristig durchgeführte) Änderungen, die mehrere Build-/Test-/Staging-Zyklen betreffen oder vor Pull-Anfrageschließung und Zusammenführung mehrere Tage umfassen.

### Terminologie

Bevor Sie beginnen, prüfen wir einige der Git/GitHub-Begriffe, die in diesem Arbeitsablauf verwendet werden.

| Name | Beschreibung |
|-----------|-------------|
| Abspaltung | Wird normalerweise als Nomen verwendet, wenn eine Kopie eines GitHub-Haupt-Repositorys gemeint ist. In der Praxis ist eine Abspaltung nur ein anderes Repository. Es ist jedoch ein spezielles Repository, da GitHub eine bidirektionale Verbindung zum übergeordneten bzw. Haupt-Repository unterhält. Es wird manchmal als Verb verwendet, z. B. „Sie müssen das Repository zuerst abspalten.“ |
| Remote | Eine benannte Verbindung zu einem Remote-Repository, z. B. „Ursprung“ oder „Upstream“. Git bezeichnet diese als Remotes, da sie zum Referenzieren eines Repositorys verwendet werden, das auf einem anderen Computer gehostet wird. In diesem Arbeitsablauf ist ein Remote immer ein GitHub-Repository. |
| Ursprung | Der Name, der der Verbindung zwischen Ihrem lokalen Repository und dem Repository zugewiesen wurde, von dem sie geklont wurde. In diesem Arbeitsablauf stellt der Ursprung die Verbindung zu Ihrer Abspaltung dar. Er wird manchmal als Name für das Ursprungs-Repository verwendet, z. B. „Denken Sie daran, Ihre Änderungen an den Ursprung weiterzugeben.“ |
| Upstream | Wie das Ursprungsremote ist auch Upstream eine benannte Verbindung zu einem anderen Repository. In diesem Workflow stellt Upstream die Verbindung zwischen Ihrem lokalen Repository und dem Haupt-Repository dar, von dem aus Ihre Abspaltung erstellt wurde. Es wird manchmal als Name für das Upstream-Repository verwendet, z. B. „Denken Sie daran, die Änderungen vom Upstream zu beziehen.“ |

Wenn Sie nicht mit Git- und GitHub-Konzepten wie einem Repository oder einer Verzweigung vertraut sind, prüfen Sie zunächst die [Git- und GitHub-Grundlagen](git-fundamentals.md).

## Arbeitsablauf

>[!IMPORTANT]
>
> Falls noch nicht geschehen, müssen Sie die Schritte im Abschnitt [Einstellungen](github-signup.md) ausführen.

In diesem Arbeitsablauf treten Änderungen in einem sich wiederholenden Zyklus auf. Ausgehend vom lokalen Repository Ihres Geräts fließen sie wieder in die GitHub-Abspaltung, in das GitHub-Haupt-Repository und wieder lokal zurück, während Sie Änderungen von anderen Mitarbeitern übernehmen.

### GitHub-Fluss verwenden

Denken Sie an die [Git- und GitHub-Grundlagen](git-fundamentals.md): Ein Git-Repository enthält einen Hauptzweig sowie weitere Verzweigungen mit laufenden Arbeiten, die noch nicht in den Hauptzweig integriert wurden. Wann immer Sie logisch zusammenhängende Änderungen eingeben, ist es am besten, einen *Arbeitszweig* zu erstellen, um Ihre Änderungen über den Workflow zu verwalten. Wir nennen dies hier Arbeitszweig, da es sich um einen Arbeitsbereich zum Iterieren/Verfeinern von Änderungen handelt, bis er wieder in den Hauptzweig integriert werden kann.

Durch Isolieren verwandter Änderungen gegenüber einer spezifischen Verzweigung können Sie diese Änderungen unabhängig voneinander steuern sowie einführen und auf einen bestimmten Zeitpunkt im Veröffentlichungszyklus ausrichten. Je nach Art der Arbeit können Sie in Ihrem Repository tatsächlich ganz einfach mehrere Arbeitsverzweigungen verwenden. Es ist nicht ungewöhnlich, gleichzeitig an mehreren Verzweigungen zu arbeiten, die jeweils ein anderes Projekt repräsentieren.

>[!NOTE]
>
>Ihre Änderungen im Hauptzweig vorzunehmen *ist nicht empfehlenswert*. Nehmen wir an, Sie verwenden den Hauptzweig, um Änderungen an einer Funktion mit einer zeitlich geplanten Veröffentlichung vorzunehmen. Sie schließen die Änderungen ab und warten darauf, sie zu veröffentlichen. In der Zwischenzeit erhalten Sie eine dringende Anfrage, etwas zu beheben, weshalb Sie die entsprechende Änderung an einer Datei im Hauptzweig vornehmen und die Änderung dann veröffentlichen. In diesem Beispiel veröffentlichen Sie versehentlich sowohl die Fehlerbehebung *als auch* die Änderungen, die Sie für die Veröffentlichung an einem bestimmten Datum vorbehalten haben.

Der nächste Schritt besteht darin, eine neue Arbeitsverzweigung in Ihrem lokalen Repository zu erstellen, um Ihre vorgeschlagenen Änderungen zu erfassen. Jeder Git-Client ist anders, wenden Sie sich also an die Hilfe für Ihren bevorzugten Client. Einen Überblick über den Prozess finden Sie im GitHub-Leitfaden zum [GitHub-Fluss](https://guides.github.com/introduction/flow/).

## Verarbeitung von Pull-Anfragen

Sie senden vorgeschlagene Änderungen, indem Sie sie in einer neuen Pull-Anfrage (PA) bündeln, die der PA-Warteschlange des Ziel-Repositorys hinzugefügt wird. Durch eine Pull-Anfrage wird das GitHub-Zusammenarbeitsmodell aktiviert, indem die Änderungen von Ihrer Arbeitsverzweigung abgerufen und in einer anderen Verzweigung zusammengeführt werden. In den meisten Fällen ist diese andere Verzweigung die Standard-/Hauptverzweigung im Haupt-Repository.

### Validierung

Bevor Ihre Pull-Anfrage in der Zielverzweigung zusammengeführt werden kann, muss sie möglicherweise mindestens einen PA-Validierungsprozess durchlaufen. Validierungsprozesse können je nach Umfang der vorgeschlagenen Änderungen und den Regeln des Ziel-Repositorys variieren. Nachdem Ihre Pull-Anfrage gesendet wurde, können Sie erwarten, dass der Inhalt überprüft und gegebenenfalls im Haupt-Repository zusammengeführt wird.

### Überprüfen und abmelden

Nachdem die gesamte PR-Verarbeitung abgeschlossen ist, sollten Sie die Ergebnisse (PR-Kommentare, Vorschau-URLs usw.) überprüfen, um festzustellen, ob zusätzliche Änderungen an den Dateien erforderlich sind, bevor Sie die Zusammenführung abzeichnen. Wenn ein PA-Prüfer Ihre Pull-Anfrage überprüft hat, kann dieser auch Feedback über Kommentare geben, wenn vor der Zusammenführung Probleme/Fragen bestehen.

Wenn die Pull-Anfrage problemlos und abgezeichnet ist, werden Ihre Änderungen in der übergeordneten Verzweigung zusammengeführt und die Pull-Anfrage wird geschlossen.

### Veröffentlichung läuft

Denken Sie daran, dass Ihre Pull-Anfrage von einem PA-Prüfer zusammengeführt werden muss, bevor die Änderungen in die nächste geplante Veröffentlichung aufgenommen werden können. Pull-Anfragen werden normalerweise in der Reihenfolge der Übermittlung geprüft/zusammengeführt. Wenn Ihre Pull-Anfrage für eine bestimmte Veröffentlichung zusammengeführt werden muss, müssen Sie mit Ihrem PA-Prüfer zusammenarbeiten, um sicherzustellen, dass die Zusammenführung vor der Veröffentlichung erfolgt.
