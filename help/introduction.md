---
title: Handbuch für Mitwirkende an der Adobe-Dokumentation
seo-title: Contributor guide overview for Adobe Experience Cloud technical documentation
description: In diesem Handbuch wird beschrieben, wie Sie Vorschläge und Ergänzungen zur Dokumentations-Website von Adobe hinzufügen können.
seo-description: The guide describes how you can contribute to the [!UICONTROL Adobe Experience Cloud] technical documentation.
exl-id: 1294d0c6-897e-49c0-bf27-fd7d122f1fc8
source-git-commit: 90122796acee9214ba96360eb7b5ff5c321a4bd6
workflow-type: ht
source-wordcount: '800'
ht-degree: 100%

---

# Handbuch für Mitwirkende an der Adobe-Dokumentation

In diesem Handbuch wird beschrieben, wie Sie zur Adobe Enterprise-Hilfe auf Experience League beitragen können.

## Was ist eine kollaborative Dokumentation?

Die technische Dokumentation und die Aktivierungsinhalte für Adobe Experience Cloud und andere Adobe Enterprise-Produkte basieren auf Open-Source-Prinzipien, die GitHub, Markdown und Adobe Experience Cloud-Lösungen nutzen.

Dieses Open-Source-Modell verbessert die Qualität der Inhalte und die Kommunikation zwischen Kunden sowie Dokumentations- und Produkt-Teams. Auf jeder Seite können Sie jetzt Nutzbarkeit von Inhalten, Protokollprobleme und sogar Inhaltsvorschläge als Git-Pull-Anfragen (PRs) bewerten. Die Adobe-Dokumentationsteams überwachen die Beiträge und Probleme täglich und nehmen nach Bedarf Aktualisierungen und Anpassungen vor.

## Arbeiten mit kollaborativer Dokumentation

Benutzende dieses Materials haben – unabhängig davon, ob sie Beschäftigte, Partner oder (potenzielle) Kunden oder Kundinnen sind – die Möglichkeit, auf unterschiedliche einfache Weise zu dieser Dokumentation beizutragen.

* Bewerten Sie die Nützlichkeit der Seite
* Melden Sie ein Problem mit einer bestimmten Seite
* Bearbeiten Sie den Content – ob durch kleine Einfügungen oder das Verfassen ganzer Artikel – unter Verwendung von Kreativelementen und Code

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
1. Klicken Sie auf **[!UICONTROL Edit this page]** in der rechten Spalte, um zur Markdown-Quelldatei auf GitHub zu gelangen.

   ![Bearbeiten Sie das Symbol für diese Seite](/help/assets/git_edit.png)

1. Klicken Sie auf das Stiftsymbol, um den Artikel zu bearbeiten.

   >[!NOTE]
   >
   >Wenn das Stiftsymbol ausgegraut ist, müssen Sie sich bei Ihrem GitHub-Konto anmelden oder ein neues Konto erstellen.

   ![Position des Stiftsymbols](assets/edit-icon.png)

1. Nehmen Sie Ihre Änderungen im Web-Editor vor.

   Sie können auf die Registerkarte **[!UICONTROL Preview changes]** klicken, um die Formatierung Ihrer Änderung zu überprüfen.
1. Nachdem Sie Ihre Änderungen vorgenommen haben, scrollen Sie zum Ende der Seite.

   Geben Sie einen Titel und eine Beschreibung für Ihren Pull Request ein und klicken Sie dann auf **[!UICONTROL Propose file change]**, wie in der folgenden Abbildung dargestellt:

   ![Vorschlagen von Änderungen](assets/submit-pull-request.png)

   >[!NOTE]
   >
   >Wenn Sie eine Validierungsfehlermeldung erhalten, in der Sie zum Unterschreiben einer Lizenzvereinbarung für Mitwirkende (Contributor License Agreement, CLA) aufgefordert werden, klicken Sie auf **[!UICONTROL Details]**, um die Lizenzvereinbarung zu öffnen. Unterschreiben Sie die Vereinbarung, falls akzeptabel. Schließen und öffnen Sie dann die Pull-Anfrage und fahren Sie fort.

Und das war&#39;s auch schon. Mitglieder des Dokumentations-Teams überprüfen Ihre Pull Request und fügen Sie zur Merge-Warteschlange hinzu. Vielen Dank!

## Melden eines Problems

Eine weitere einfache Möglichkeit, uns auf ein Problem mit einem Inhalt hinzuweisen, ist die Verwendung von **[!UICONTROL Log an Issue]**.

1. Wenn Sie problematischen Inhalt finden, klicken Sie auf das **[!UICONTROL Log an Issue]**-Symbol in der rechten Spalte.

   ![](assets/git_log_issue.png)

   >[!NOTE]
   >
   >Um ein Problem zu melden, müssen Sie sich bei Ihrem GitHub-Konto anmelden oder ein Konto erstellen.

   Durch Klicken auf diesen Link können Sie uns rasch über die GitHub-Benutzeroberfläche ein Ticket senden.

   Die URL der problematischen Seite wird automatisch im Beschreibungsfeld eingetragen.

1. Geben Sie den Titel ein, fügen Sie eine kurze Beschreibung des Problems hinzu und klicken Sie dann auf *Submit new issue*.

   ![](assets/git_issue_example.png)

Durch die Übermittlung eines Tickets wird das Inhalts-Team über diese Seite informiert, das dann das Problem beheben kann. Wenn wir den Inhalt aktualisiert haben, teilen wir Ihnen dies in der GitHub-Problemoberfläche mit und Sie werden bei Aktualisierung oder Schließung des Problems per E-Mail informiert.

## GitHub-Berechtigungen verstehen

Die GitHub-Bearbeitungsbenutzeroberfläche passt sich Ihren Repository-Berechtigungen an. Die vorherigen Bilder beziehen sich auf Mitarbeiter, die keine Schreibrechte für das Ziel-Repository besitzen. GitHub erstellt in Ihrem Konto automatisch eine Abspaltung des Ziel-Repositorys. Wenn Sie über Schreibzugriff für das Ziel-Repository verfügen, erstellt GitHub im Ziel-Repository eine neue Verzweigung.

Adobe verwendet Pull-Anfragen für alle Änderungen, selbst für Mitarbeiter, die über Schreibzugriff verfügen. Für die meisten Repositorys ist die `main`-Verzweigung geschützt, sodass Aktualisierungen als Pull-Anfragen übermittelt werden müssen.

Die Bearbeitung im Browser eignet sich am besten für geringfügige oder selten durchgeführte Änderungen. Wenn Sie große Beiträge einbringen oder erweiterte Git-Funktionen verwenden, empfehlen wir Ihnen, das [Repository abzuspalten und lokal zu arbeiten](setup/full-workflow.md).

## Feedback geben

Bei einer Lösung, die so groß wie die von Adobe ist, wird die Dokumentation ständig bearbeitet. Wenn Sie Fehler finden, protokollieren Sie ein Problem, und wenn Sie Vorschläge zu Material haben, teilen Sie uns dies mit. Teilen Sie uns mit, wonach Sie gesucht haben. Lassen Sie uns wissen, wenn Sie nicht finden konnten, was Sie benötigen, oder wenn Sie Schwierigkeiten hatten, Ihre Aufgabe abzuschließen. Teilen Sie uns mit, wie wir Ihnen beim Erlernen unserer Lösungen helfen können.

Das Team für kollaborative Dokumentation bedankt sich herzlich bei allen Autorinnen und Autoren und Inhaltsproduzierenden in Experience League.
