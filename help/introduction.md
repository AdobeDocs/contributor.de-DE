---
title: Mitarbeiter-Handbuch für Adobe-Dokumentation
seo-title: Contributor guide overview for Adobe Experience Cloud technical documentation
description: In diesem Handbuch wird beschrieben, wie Sie Vorschläge und Ergänzungen zur Dokumentationsseite von Adobe hinzufügen können.
seo-description: The guide describes how you can contribute to the [!UICONTROL Adobe Experience Cloud] technical documentation.
exl-id: 1294d0c6-897e-49c0-bf27-fd7d122f1fc8
source-git-commit: 90122796acee9214ba96360eb7b5ff5c321a4bd6
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 70%

---

# Mitarbeiter-Handbuch für Adobe-Dokumentation

In diesem Handbuch wird beschrieben, wie Sie zur Adobe der Enterprise-Hilfe bei der Experience League beitragen können.

## Was ist eine partizipative Dokumentation?

Die technische Dokumentation und der Aktivierungsinhalt für Adobe Experience Cloud und andere Adobe Enterprise-Produkte basieren auf Open-Source-Prinzipien, die GitHub-, Markdown- und Adobe Experience Cloud-Lösungen verwenden.

Dieses Open-Source-Modell verbessert die Qualität und Kommunikation von Inhalten zwischen Kunden, Dokumentationsteams und Produktteams. Auf jeder Seite können Sie jetzt Nutzbarkeit von Inhalten, Protokollprobleme und sogar Inhaltsvorschläge als Git-Pull-Anfragen (PRs) bewerten. Die Adobe-Dokumentationsteams überwachen die Beiträge und Probleme täglich und nehmen nach Bedarf Aktualisierungen und Anpassungen vor.

## Arbeiten mit kollaborativer Dokumentation

Als Anwender dieses Materials haben Sie - unabhängig davon, ob Sie Angestellter, Partner, Kunde oder potenzieller Kunde sind - die Wahl, auf verschiedene einfache Weise zu dieser Dokumentation beizutragen.

* Bewerten der Nützlichkeit der Seite
* Problem mit einer bestimmten Seite protokollieren
* Senden Sie eine schnelle Bearbeitung durch das Authoring ganzer Artikel, einschließlich Assets und Codebeispielen

In diesem Handbuch wird alles beschrieben, was Sie für einen Beitrag zu diesem Materialsatz wissen müssen.

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
-->

## Vorhandene Dokumente schnell bearbeiten

Das schnelle Bearbeiten ist eine gute Möglichkeit, kleine Fehler in Dokumenten zu beheben oder fehlenden Inhalt hinzuzufügen. Wenn ein Artikel wie unten gezeigt eine Schaltfläche zum Bearbeiten anzeigt, können Sie selbst eine schnelle Korrektur vornehmen. Wenn Sie das Dokument bearbeiten, übermitteln Sie eine Pull-Anfrage (PA) an uns, um die Korrektur/den Vorschlag an uns zu senden, und wir können den Vorschlag prüfen, genehmigen und veröffentlichen.

1. Unterschreiben Sie die [Lizenzvereinbarung für Mitarbeiter (CLA)](http://opensource.adobe.com/cla.html), falls akzeptabel.

   Sie müssen nur einmal eine Adobe-Lizenzvereinbarung für Mitarbeiter übermitteln.
1. Klicken **[!UICONTROL Edit this page]** in der rechten Spalte, um zur Markdown-Quelldatei auf GitHub zu wechseln.

   ![Bearbeiten Sie das Symbol für diese Seite](/help/assets/git_edit.png)

1. Klicken Sie auf das Stiftsymbol, um den Artikel zu bearbeiten.

   >[!NOTE]
   >
   >Wenn das Stiftsymbol ausgegraut ist, müssen Sie sich bei Ihrem GitHub-Konto anmelden oder ein neues Konto erstellen.

   ![Position des Stiftsymbols](assets/edit-icon.png)

1. Nehmen Sie Ihre Änderungen im Webeditor vor.

   Sie können auf die Registerkarte **[!UICONTROL Preview changes]** klicken, um die Formatierung Ihrer Änderung zu überprüfen.
1. Nachdem Sie Ihre Änderungen vorgenommen haben, scrollen Sie zum unteren Rand der Seite.

   Geben Sie einen Titel und eine Beschreibung für Ihre PA ein und klicken Sie auf **[!UICONTROL Propose file change]** wie in der folgenden Abbildung dargestellt:

   ![Änderung vorschlagen](assets/submit-pull-request.png)

   >[!NOTE]
   >
   >Wenn Sie eine Validierungsfehlermeldung zum Unterschreiben einer Lizenzvereinbarung für Mitarbeiter (CLA) erhalten, klicken Sie auf **[!UICONTROL Details]**, um die Lizenzvereinbarung zu öffnen. Unterschreiben Sie die Vereinbarung, falls akzeptabel. Schließen und öffnen Sie dann die Pull-Anfrage und fahren Sie fort.

Das ist alles. Mitglieder des Dokumentationsteams überprüfen Ihre Pull-Anfrage und führen sie zusammen. Vielen Dank!

## Problem protokollieren

Eine weitere einfache Möglichkeit, uns über ein Problem mit einem Inhaltselement zu informieren, besteht darin, **[!UICONTROL Log an Issue]**.

1. Wenn ein Problem mit einem Inhaltselement auftritt, klicken Sie auf das **[!UICONTROL Log an Issue]**-Symbol in der rechten Spalte.

   ![](assets/git_log_issue.png)

   >[!NOTE]
   >
   >Um ein Problem zu protokollieren, müssen Sie sich bei Ihrem GitHub-Konto anmelden oder ein Konto erstellen.

   Wenn Sie auf diesen Link klicken, können Sie über die GitHub-Problemoberfläche ein kurzes Ticket mit Experience League protokollieren.

   Die URL der Seite mit dem Problem wird automatisch in das Beschreibungsfeld eingetragen.

1. Füllen Sie den Titel aus, schreiben Sie eine kurze Erläuterung des Problems und klicken Sie dann auf *Submit new issue*.

   ![](assets/git_issue_example.png)

Durch die Übermittlung eines Problems wird das Inhaltsteam über diese Seite informiert, das Ihr Problem beheben kann. Wenn wir den Inhalt aktualisiert haben, teilen wir Ihnen dies in der GitHub-Problemoberfläche mit und Sie werden bei Aktualisierung oder Schließung des Problems per E-Mail informiert.

## GitHub-Berechtigungen verstehen

Die GitHub-Bearbeitungsbenutzeroberfläche passt sich Ihren Repository-Berechtigungen an. Die vorherigen Bilder beziehen sich auf Mitarbeiter, die keine Schreibrechte für das Ziel-Repository besitzen. GitHub erstellt in Ihrem Konto automatisch eine Abspaltung des Ziel-Repositorys. Wenn Sie über Schreibzugriff für das Ziel-Repository verfügen, erstellt GitHub im Ziel-Repository eine neue Verzweigung.

Adobe verwendet Pull-Anfragen für alle Änderungen, selbst für Mitarbeiter, die über Schreibzugriff verfügen. Für die meisten Repositorys ist die `main`-Verzweigung geschützt, sodass Aktualisierungen als Pull-Anfragen übermittelt werden müssen.

Die Bearbeitung im Browser eignet sich am besten für geringfügige oder selten durchgeführte Änderungen. Wenn Sie große Beiträge einbringen oder erweiterte Git-Funktionen verwenden, empfehlen wir Ihnen, das [Repository abzuspalten und lokal zu arbeiten](setup/full-workflow.md).

## Feedback geben

Bei einer Lösung, die so groß wie die von Adobe ist, wird die Dokumentation ständig bearbeitet. Wenn Sie Fehler finden, protokollieren Sie ein Problem, und wenn Sie Vorschläge zu Material haben, teilen Sie uns dies mit. Teilen Sie uns mit, wonach Sie gesucht haben. Lassen Sie uns wissen, wenn Sie nicht finden konnten, was Sie benötigen, oder wenn Sie Schwierigkeiten hatten, Ihre Aufgabe abzuschließen. Teilen Sie uns mit, wie wir Ihnen beim Erlernen unserer Lösungen helfen können.

Das Team für die gemeinsame Dokumentation und alle Autoren und Inhaltsinhaber der Experience League danken.
