---
title: Grundlagen der Git- und GitHub-Dokumentation
description: In diesem Artikel werden eine Übersicht über Git, GitHub-Repository und die Art der Organisierung von Inhalten sowie Benennungskonventionen für die Adobe-Dokumentation erläutert.
exl-id: 2b2ec764-4201-4bcd-802d-a034d6675793
source-git-commit: 90122796acee9214ba96360eb7b5ff5c321a4bd6
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 100%

---

# Grundlagen der Git- und GitHub-Dokumentation

## Überblick

Wenn Sie nur kleinere Textänderungen an Artikeln vornehmen müssen, müssen Sie die Details dieses Artikels nicht kennen. In diesem Artikel wird der Arbeitsablauf für umfangreiche Bearbeitungen beschrieben, z. B. das Erstellen neuer Artikel, das Hinzufügen von Bildern oder die laufende Bearbeitung der Adobe-Dokumentation.

Als Mitarbeiter am Inhalt von Adobe-Dokumentation können Sie mit mehreren Werkzeugen und Prozessen interagieren. Sie können parallel mit anderen Mitarbeitern am selben Projekt arbeiten, möglicherweise auch am selben Inhalt und zur gleichen Zeit. Dies ist alles durch Git- und GitHub-Software möglich.

Git ist ein Open-Source-Versionskontrollsystem, das die Zusammenarbeit ermöglicht. Mehrere Mitarbeiter können an Dateien arbeiten, die sich in *Repositorys* befinden.

GitHub ist ein webbasierter Hosting-Dienst für Git-Repositorys, z. B. zum Speichern von [docs.adobe.com](https://docs.adobe.com)-Inhalt. GitHub hostet für jedes Projekt das Haupt-Repository, von dem aus Mitarbeiter Kopien für ihre eigene Arbeit erstellen können.

## Git

Git verfügt über einen eindeutigen Beitragsarbeitsablauf und eine Terminologie, um das verteilte Modell zu unterstützen. Es gibt beispielsweise keine Dateisperrung, die normalerweise mit Check-out-/Check-in-Vorgängen verknüpft ist. Git ermöglicht die noch feinere Lösung von Änderungen, wobei Dateien Byte für Byte miteinander verglichen werden.

Git verwendet außerdem eine stufige Struktur zum Speichern und Verwalten von Inhalten für ein Projekt:

- *Repository*: Wird auch als *Repo* bezeichnet und ist die höchste Speichereinheit. Ein Repository enthält mindestens eine Verzweigung.
- *Verzweigung*: Alle Repositorys enthalten eine Hauptverzweigung (die gewöhnlich den Namen „Main“ trägt) und mindestens eine weitere Verzweigung, die zur erneuten Zusammenführung mit der Hauptverzweigung vorgesehen ist. Die Hauptverzweigung ist die aktuelle Version und Quelle, aus der Inhalt veröffentlicht wird. Sie ist die übergeordnete Ebene, von der aus alle anderen Verzweigungen im Repository erstellt werden.

Mitarbeiter interagieren mit Git, um Repositorys auf den lokalen und GitHub-Ebenen zu aktualisieren und zu manipulieren:

- Lokal über Werkzeuge wie GitHub Desktop.
- Über [www.github.com](https://www.github.com), wo Git zur Verwaltung der Abstimmung von Beiträgen integriert wird, die in das Haupt-Repository zurückfließen.

## GitHub

Alle Arbeitsabläufe beginnen und enden auf der GitHub-Ebene, wo das Haupt-Repository für ein Adobe-Dokumentationsprojekt gespeichert wird. Die Kopien, die Mitarbeiter für ihre eigene Verwendung erstellen, werden auf mehrere Computer verteilt. Diese Kopien werden schließlich wieder mit dem GitHub-Haupt-Repository des Projekts abgestimmt.

### Verzeichnisorganisierung

Die Standard-/Hauptverzweigung eines Projekts liefert die aktuelle Version eines Inhalts für das Projekt. Der Inhalt in der Hauptverzweigung – sowie der daraus erstellten Verzweigungen – ist ebenso angeordnet wie die Artikelthemen. Unterverzeichnisse werden zum Organisieren von Inhalts- und Bildassets verwendet.

In der Regel befindet sich ein `help`-Hauptverzeichnis im Stamm des Repositorys. Das Artikelverzeichnis enthält eine Reihe von Unterverzeichnissen. Artikel in den Unterverzeichnissen werden als Markdown-Dateien formatiert, die eine *.md*-Erweiterung verwenden.

Im Stamm dieses Verzeichnisses finden Sie allgemeine Artikel, die sich auf den Gesamtdienst oder das gesamte Produkt beziehen. In der Regel können Sie dann eine weitere Reihe von Unterverzeichnissen finden, die den Funktionen/Diensten oder allgemeinen Szenarien entsprechen.

### Assetverzeichnis

Benutzerhandbuch-Verzeichnisse enthalten `/assets`-Unterverzeichnisse für Bilddateien, auf die in einem Verzeichnis verwiesen wird.

<!--

### Markdown file template

For convenience, the root directory of each repository typically contains a Markdown template file named `template.md`. You can use this template file as a "starter file" if you need to create a new article for submission to the repository. The file contains:

- A **metadata header** at the top of the file, delineated by two, 3-hyphen lines. It contains the various tags used for tracking information related to the article. It also includes SEO optimizations and reporting processes that Adobe uses to evaluate the performance of the content. So the metadata is important!
- Various **examples of using Markdown** to format the elements of an article.
- General **instructions on the use of Markdown extensions**, which you can use for various types of alerts.
- Examples of **embedding video** by using an iframe.
- General **instructions on the use of docs.adobe.com extensions**, which you can use for special controls such as buttons and selectors.

-->

## Pull-Anfragen

Eine *Pull-Anfrage* bietet Mitarbeitern eine praktische Möglichkeit, einen Satz von Änderungen vorzuschlagen, die auf die Standardverzweigung angewendet werden. Die Änderungen (auch als *Zusagen* bezeichnet) werden in der Verzweigung eines Mitarbeiters gespeichert. GitHub kann so zuerst die Auswirkungen der *Zusammenführung* in der Standardverzweigung modellieren. Eine Pull-Anfrage dient auch als Mechanismus, um Mitarbeitern Feedback aus einem Build-/Validierungsprozess durch den Pull-Anfrageprüfer bereitzustellen und so potenzielle Probleme oder Fragen zu klären, bevor die Änderungen in der Standardverzweigung zusammengeführt werden.

Je nach Größe der Änderungen, die Sie vorschlagen möchten, gibt es zwei Möglichkeiten, etwas durch Pull-Anfragen beizutragen: Wir behandeln dies im Detail später im Abschnitt [GitHub-Arbeitsablauf](local-repo.md) in diesem Handbuch.
