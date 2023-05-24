---
title: Git-Repository lokal einrichten
description: Dieser Artikel enthält Anleitungen zum Erstellen Ihres lokalen Git-Repositorys und zum Beitrag zur Adobe-Dokumentation, einschließlich des Abspaltungs- und Klonvorgangs.
exl-id: 679c07a2-030b-4a30-ba14-7780f88dae11
source-git-commit: a3c283c5c0d181beacc566262743528d5ff9f7d2
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 100%

---

# Lokales Git-Repository für Dokumentation einrichten

In diesem Artikel werden die Schritte zum Einrichten eines Git-Repositorys auf Ihrem lokalen Computer beschrieben, das dem Beitrag zur Adobe-Dokumentation dient. Mitarbeiter können ein lokal geklontes Repository verwenden, um neue Artikel hinzuzufügen, umfangreiche Änderungen an vorhandenen Artikeln vorzunehmen oder Grafiken zu ändern.

>[!IMPORTANT]
>Wenn Sie nur geringfügige Änderungen an einem Artikel vornehmen, müssen Sie die Schritte in diesem Artikel *nicht* ausführen. Sie können einfach auf das Bearbeitungssymbol klicken und Text in Ihrem Browser bearbeiten.

## Überblick

Um zur Adobe-Dokumentation beizutragen, können Sie das entsprechende Repository in Ihr eigenes GitHub-Konto abspalten, um Lese-/Schreibberechtigungen zu erhalten. Anschließend können Sie Markdown-Dateien lokal erstellen und bearbeiten, indem Sie das entsprechende Dokumentations-Repository klonen. Danach verwenden Sie Pull-Anfragen zum Zusammenführen (Senden) von Änderungen in das schreibgeschützte zentral freigegebene Repository.

* Entsprechendes Repository bestimmen
* Repository in Ihr GitHub-Konto abspalten
* Lokalen Ordner für die geklonten Dateien wählen
* Repository auf Ihren lokalen Computer klonen
* Upstream-Remotewert konfigurieren

## Repository bestimmen

Sie spalten das entsprechende Repository in Ihr eigenes GitHub-Konto ab, um dafür Lese-/Schreibberechtigungen zu erhalten und Ihre vorgeschlagenen Änderungen speichern zu können. Die Dokumentation von [!UICONTROL Adobe Experience Cloud] befindet sich in verschiedenen Repositorys unter [github.com](https://www.github.com/adobedocs).

1. Wenn Sie sich nicht sicher sind, welches Repository zu verwenden ist, rufen Sie den Artikel mit Ihrem Webbrowser auf. Wählen Sie rechts oben im Artikel den Link **Bearbeiten** (Stiftsymbol). (Wenn Sie keinen Link zum Bearbeiten sehen, ist dieser Inhalt in GitHub noch nicht verfügbar.)

Um zur Adobe-Dokumentation beizutragen, können Sie Markdown-Dateien lokal erstellen und bearbeiten, indem Sie das entsprechende Dokumentations-Repository klonen. Danach verwenden Sie Pull-Anfragen zum Zusammenführen von Änderungen in das schreibgeschützte zentral freigegebene Repository.

<!---
![GitHub Triangle](/assets/git-and-github-initial-setup.png)

If you're new to GitHub, watch the following video for a conceptual overview of the forking and cloning process:

>[!VIDEO https://channel9.msdn.com/Blogs/CoolMoose/Git-Repository-Setup/player]
-->

## Repository abspalten

Erstellen Sie mithilfe des entsprechenden Repositorys eine Abspaltung des Repositorys in Ihrem eigenen GitHub-Konto mithilfe der GitHub-Website.

Da alle Hauptdokumentations-Repositorys schreibgeschützten Zugriff bieten, also keine Änderungen an Inhalt direkt in den Repositorys vorgenommen werden können, ist eine persönliche Abspaltung erforderlich. Um Änderungen vorzunehmen, müssen Sie eine Pull-Anfrage (PA) von Ihrer Abspaltung an das Haupt-Repository senden. Zur Vereinfachung dieses Prozesses benötigen Sie zunächst Ihre eigene Kopie des Repositorys, für die Sie Schreibzugriff haben. Eine GitHub-*Abspaltung* erfüllt diesen Zweck.

1. Rufen Sie die GitHub-Seite des Haupt-Repositorys auf und klicken Sie oben rechts auf die Schaltfläche **Fork**.

   ![GitHub-Abspaltung](assets/fork-simple.png)

1. Wenn Sie dazu aufgefordert werden, wählen Sie über die entsprechende Kachel Ihr GitHub-Konto als Ziel aus, in dem die Abspaltung erstellt werden soll. Nach dieser Aufforderung wird eine Kopie des Repositorys innerhalb Ihres GitHub-Kontos erstellt, die als „Abspaltung“ bezeichnet wird.

1. Wählen Sie einen Ordnernamen, den Sie einfach eingeben und sich merken können.

   Einige Repositorys können groß sein. Wählen Sie einen Speicherort mit verfügbarem Speicherplatz.

   >[!NOTE]
   >
   >Vermeiden Sie die Auswahl eines lokalen Ordnerpfads, der innerhalb eines anderen Git-Repository-Ordnerspeicherorts verschachtelt ist. Zwar können Git-geklonte Ordner nebeneinander gespeichert werden, das Verschachteln von Git-Ordnern ineinander hingegen führt zu Fehlern beim Datei-Tracking.

## Lokalen Klon des Repositorys erstellen

Beim Erstellen eines Klons des abgespalteten Repositorys laden Sie eine Kopie der Dateien auf Ihren Computer herunter. Wenn Sie fertig sind, können Sie die Änderungen von Ihrem lokalen Laufwerk auf das abgespaltete Repository auf dem Server übertragen. Anschließend können Sie eine Pull-Anfrage senden, um die Änderungen vorgelagert im Haupt-Repository zusammenzuführen.

Bei diesen Schritten wird vorausgesetzt, dass Sie GitHub Desktop verwenden. Wenn Sie einen anderen Client verwenden, nehmen Sie entsprechende Anpassungen vor.

1. Klicken Sie auf **Clone or download** und wählen Sie dann **Open in Desktop**, um eine Kopie des Repositorys (Ihre Abspaltung) in das aktuelle Verzeichnis auf Ihrem Computer abzulegen.

   ![Klonen eines Repositorys](assets/clone-pulldown.png)

1. Verwenden Sie GitHub Desktop, damit lokale Dateien stets mit dem abgespalteten Repository synchronisiert sind.

Weitere Informationen finden Sie in der [GitHub Desktop-Dokumentation](https://help.github.com/desktop/).
