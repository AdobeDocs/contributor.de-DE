---
lastModified: 2018-06-28T00:00:00Z
title: Autorenstil-Richtlinien für externe Mitarbeiter
description: Erfahren Sie mehr über Authoring und redaktionelle Richtlinien für externe Mitwirkende in der Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2227'
ht-degree: 8%

---

# Autorenstil-Richtlinien für externe Mitarbeiter{#guidelines}

Auf dieser Seite finden Sie redaktionelle Richtlinien für externe Autoren, die Inhalte erstellen oder bestehende Inhalte in Experience League aktualisieren. Bevor Sie beginnen, stellen Sie Folgendes sicher:

* Machen Sie sich mit [Markdown](markdown.md) Authoring
* Prüfen Sie die Rechtschreibung und Grammatik in Ihren Artikeln
* Verwenden Sie einen freundlichen Ton, eine konsistente Darstellung und einfache Sätze, um die maschinelle Übersetzung zu verbessern
* Folgen [Best Practices](#writing-tips) und redaktionelle Standards auf dieser Seite

## Stilrichtlinien{#style-guidelines}

Beachten Sie beim Schreiben der Dokumentation Folgendes.

* **Halten Sie sich kurz**: Verschwenden Sie keine Wörter. Halten Sie die Sätze kurz und knapp. Der Artikel soll fokussiert bleiben. Halten Sie die Anzahl der Hinweise gering.
* **Konzentrieren Sie sich auf die Zielgruppe und den Zweck**: Bevor Sie mit dem Schreiben beginnen, legen Sie eindeutig fest, wer der Kunde ist und welche Aufgabe er durchführen möchte. Schreiben Sie Ihren Artikel, um dem Kunden bei dieser Aufgabe zu helfen.
* **Verwenden Sie Beispiele**: Stellen Sie Beispiele zur Erläuterung von Konzepten bereit.
* **Organisieren Sie Ihren Inhalt**: Erstellen Sie Abschnitte, um die Anweisungen in besser verwaltbare Gruppen von Schritten zu unterteilen. Verwenden Sie einen Screenshot, wenn er der Klärung dient.

## Best Practices für das technische Schreiben{#writing-tips}

Technisches Schreiben, insbesondere für die Softwaredokumentation, ist eine spezialisierte Branche. Sogar der produktivste Romanautor wird beim Versuch des technischen Schreibens gewitzt - nicht weil das Material komplex oder technisch ist, sondern weil es nicht einfach ist, komplexe, technische Informationen zu erstellen _einfach_. Um erfolgreich zu sein, muss der Inhalt strukturkonsistent, scannbar, wiederverwendbar und ohne Struktur- und Syntaxfehler durch die Veröffentlichungs-Pipeline fließen.

In den folgenden Abschnitten werden häufig auftretende Probleme beschrieben, auf die neue Autoren achten müssen:

### Überschriften nicht durch Text getrennt (doppelte Überschriften){#double-headings}

Wenn Sie über zwei Überschriften ohne Text verfügen, der sie voneinander trennt, fügen Sie fehlenden Text hinzu (um die zweite Themenüberschrift einzuführen). Sie können auch eine der Überschriften entfernen. Die zweite ist wahrscheinlich unnötig.

Beispiel: _Übersicht_ erfüllt hier keinen Zweck:

![Doppelte Überschriften](assets/headings-double.png)

* Wenn Ihre zweite Überschrift zufällig _Übersicht_, ist es wahrscheinlich unnötig. Ihr H1-Absatz und Ihr erster Absatz dienen als konzeptionelle Übersicht über das Thema des Artikels.

* Für SEO-Zwecke können eigenständige Überschriften wie _Übersicht_ und _Einführung_ sind von selbst nicht nützlich. Nennen Sie das Produkt oder die Funktion, die Sie einführen. (Beispiel: _Übersicht über Fallout-Berichte_)

### Inkonsistente Querverweisüberschriften{#maps}

Verwendung _Weitere Informationen_ Überschriften für Querverweislisten (oder Karten). Beispiel:

![Querverweisliste](assets/headings-more-info.png)

**Leitlinien für Querverweislisten**

* Verwenden einer Aufzählungsliste für die Querverweise
* Verwenden Sie für die formalen Namen von Guides oder Seitennamen kursiv (wenn Sie keinen Linktext verwenden).
* Die Überschrift (oder eine Überschrift) nicht abschneiden
* Zahlen in Überschriften vermeiden

### Nicht übereinstimmender Inhaltsverzeichnis-Eintrag, Breadcrumb und Seitenname{#toc}

Da wir die Inhaltsverzeichnis-Datei (Inhaltsverzeichnis) manuell verwalten, sind diese Inkongruenzen einfache Fehler. Stellen Sie sicher, dass Ihr Inhaltsverzeichnis mit Ihrem Seitennamen (H1) übereinstimmt. Stellen Sie außerdem sicher, dass sie mit dem Breadcrumb übereinstimmt.

**Leitlinien zu Inhaltsverzeichnissen und Listen**

* Möglicherweise müssen Sie Ihren TOC-Eintrag verkürzen, er muss sich jedoch eindeutig auf den Seitennamen und Breadcrumb beziehen.
* Breadcrumbs werden aus den Titel-Metadaten abgerufen, sodass sie (für SEO-Zwecke) unterschiedlich sein können.

### Anführungszeichen anstelle kursiver Zeichen{#quotes}

Es ist schwer, dem Hinzufügen von Anführungszeichen um ein Wort oder eine Wortgruppe zu widerstehen. Anführungszeichen sind jedoch für das Anführungszeichen von Sprache vorgesehen und werden fast nie in der Produktdokumentation verwendet.

**Anführungszeichen**

* In der Regel funktionieren Kursivformatierungen besser als Anführungszeichen (für Fehlermeldungen, eindeutige oder fremde Wörter usw.).
* Verwenden Sie für Elemente der Benutzeroberfläche Fettdruck und UICONTROL.

### Verfahren{#steps}

Schreiben einer Prozedur (das _Aufgabe_ Inhaltstyp) ist kein Talent, mit dem wir geboren werden. Die Erstellung eines lesbaren, klaren Verfahrens wird praktiziert.

**Leitlinien für Schritte**

* Ein Verfahren ist eine Reihe von Schritten. Ein Schritt ist eine kurze, nummerierte _ein Satz_ Befehl.
* Beginnen Sie jeden Schritt entweder mit einem Verb oder dem _nach_ infinitiv (Orientierung des Lesers zum Ziel, wie in _Um angemeldet zu bleiben, aktivieren Sie **Voranmeldung**_). Wenn ein Schritt innerhalb des Gesamtverfahrens ein bestimmtes Ziel hat, nennen Sie das Ziel vor der Aktion.
* Wenn Sie Informationen über den Schritt haben (einen Inhaltstyp namens _Schrittinformationen_, fügen Sie sie nach dem Schritt (eingerückt mit dem Schritt) oder nach dem Asset (Screenshot, Video oder Liste mit Beschreibungen der Benutzeroberfläche) hinzu.
* Wenn Ihr Schritt zwei Aktionen hat (z. B. _Wählen Sie dies aus und stellen Sie dann fest, dass_), schreiben Sie es als einen einzigen, kurzen Satz.
* Begrenzen Sie Ihre Aufgabe auf etwa sieben bis zehn Schritte. Wenn Sie mehr als zehn Schritte in einer Aufgabe erstellen, müssen Sie sie wahrscheinlich in zwei Aufgaben unterteilen. Nützen Sie hier Ihr bestes Urteilsvermögen.
* Verwenden Sie in der Produktdokumentation keine Überschriften als Schritte. (Ausnahme unten für Tutorials.)
* Bei mehrseitigen Tutorials können Überschriften als Schritte zulässig sein. Führen Sie sie jedoch nicht auf. Rechtschreibweise _Schritt 1:_, _Schritt 2:_ usw.

**Beispielverfahren**

Hier finden Sie eine gut strukturierte Anleitung zur Anmeldung bei der Adobe:

So melden Sie sich bei Adobe an:

1. on `Adobe.com`auswählen **Experience Cloud**.
1. Auswählen **Anmelden**.
1. Auswählen **Persönliches Konto**.
1. Um sich weiterhin anzumelden, wählen Sie **Anmeldung beibehalten**.
1. Geben Sie Ihren Namen und Ihr Kennwort ein.
1. Auswählen **Anmelden**.

### Parallele Listen{#lists}

Die Verwendung der parallelen Konstruktion für Listen erleichtert das Lesen und Scannen. Zu den Listen gehören ein Inhaltsverzeichnis (Inhaltsverzeichnis), Aufzählungslisten (unsortiert) oder nummerierte Listen.

Beispiel-Inhaltsverzeichnis mit parallelen Einträgen:

![Paralleles Inhaltsverzeichnis](assets/parallel-toc.png)

Das vorherige Inhaltsverzeichnis ist ein gutes Beispiel, da:

* Konzeptbezogene übergeordnete Einträge sind Begriffe oder Substanzausdrücke.
* Verfahren (Aufgaben) sind aktive Verben (nicht Gerunds)
* Alle Einträge verwenden die Satzgroßschreibung

## Metadaten für Titel und Beschreibung{#metadata}

_Titel_ und _description_ Metadaten sind für SEO, Inhaltssuche und Qualitätsbewertungen von Inhalten in der Experience League wichtig.

Im Folgenden finden Sie Beispiele für Titel und Beschreibungen:

**Beschreibungen für Konzeptartikel**

* _Erfahren Sie mehr über Segmente in Adobe Analytics. Hier erhalten Sie Hilfe beim Konfigurieren des Segmentierungsbereichs in einem Arbeitsbereich._
* _Hier erhalten Sie Hilfe zur Verwendung von Segmenten in einem Seitenansichtsbericht in Adobe Analytics._

**Beschreibungen für Verfahren-/Aufgabenartikel**

* _Erfahren Sie, wie Sie ein Segment in Adobe Analytics erstellen._
* _Erstellen Sie ein Segment in Adobe Analytics. Erfahren Sie, wie Sie einen Bericht basierend auf dem erstellten Segment auswählen, konfigurieren und ausführen._

Die verwendete Komponente hängt von der Größe und dem Umfang des Artikels ab.

**Titel für einen Konzeptartikel**

* _Segmente in Seitenansichtsberichten_

**Titel für einen Prozess-/Aufgabenartikel**

* _Erstellen eines Segments für einen Bericht &quot;Seitenansichten&quot;_

(Beachten Sie, dass die Produktnamen und der Produktname automatisch zu den Titeln hinzugefügt werden.)

## Möglichkeiten zur Verbesserung der Klarheit (und der Acrolinx-Werte){#tips}

Im Folgenden finden Sie einfache Möglichkeiten zur Verbesserung von Inhaltserstellung, Klarheit und Lesbarkeit. Diese helfen auch bei der Verbesserung von Acrolinx-Stilwerten und CQI-Werten auf ExL.

| Leitlinien | Informationen zu  |
|---|---|
| Aktive Stimme verwenden | Passiv Stimme in aktive Stimme ändern |
| Aktuelle Spannung verwenden | **Schwach:** *Campaign v8 wird im Juni veröffentlicht.* <p>**Stark:** *Campaign v8 wird im Juni veröffentlicht.*<p>Aktuelle Spannungen sind für Kunden immer leichter zu lesen. |
| Vermeiden Sie schwache, unnötige Adverbien | *Sehr*, *extrem*, *unglaublich*.... <p>Adverben sind zusätzliche Wörter, die keine wichtige Bedeutung hinzufügen, wenn Sie starke und präzise Verben, Klauseln und Adjektive verwenden. |
| Verwenden Sie starke Verben für Titel und [Inhaltsverzeichnis-Einträge](#using-toc) | Beispiele:<p>**Schwach:** *Erstellung und Verwaltung von Eigenschaften* <p>**Stark:** *Erstellen und Verwalten von Eigenschaften* |
| Satz verwenden [Großschreibung](https://docs.microsoft.com/en-us/style-guide/capitalization) | Wenn du im Zweifel bist, mach dir keine Großschreibung. Verwenden Sie in Überschriften die Groß-/Kleinschreibung im Stil von Satzteilen. Eigene Nomen und das erste Wort nach einem Doppelpunkt großschreiben. In den Verfahren stimmen Sie die Groß-/Kleinschreibung überein, die Sie auf der Benutzeroberfläche sehen. |
| Diese kleinen Tipps für mehr Klarheit | <ul><li>Vermeiden *Um* (keine Bedeutung). Alles, was du brauchst *auf.*</li><li>Vermeiden *Verwenden Sie.* Es hört sich vielleicht technischer an, aber nicht. *Ausnutzen* bedeutet *, insbesondere von etwas, das nicht für den Zweck bestimmt war, das*.</li><li>Semikolons vermeiden: Verwenden Sie stattdessen einen Punkt und beginnen Sie einen neuen Satz. Semikolons führen zu unnötiger Komplexität.</li><li>Doppelpunkt: Verwenden Sie Doppelpunkte, um eine Liste einzufügen. Verwenden Sie Doppelpunkte sparsam in Sätzen. Großschreibung des ersten Wortes nach einem Doppelpunkt in einem Satz.</li><li>Verwenden Sie das Oxford-Komma (drei Kommas in einer Liste).</li><li>Halten Sie die Satzlänge unter 39 Wörtern.</li><li>Navigation: use _gehen Sie zu_ oder _navigieren zu_.</li><li>Vermeiden Sie unformatierten URL-Text (verwenden Sie benutzerfreundlichen Link-Text), es sei denn, die Anzeige des Pfads ist wichtig.</li></ul> |
| Rechtschreibprüfung in VSC verwenden | Installieren Sie die Code-Rechtschreibprüfung (Erweiterung) in Visual Studio Code. |
| Änderung _click_ nach _gehen Sie zu_ oder _select_ | _Klicken_ ist ein gerätespezifisches Wort (mit Zugänglichkeitsproblemen), und der Trend besteht darin, von diesem abzurücken. Im Folgenden finden Sie Vorschläge zur Änderung:<ul><li>Navigation: _Wechseln Sie zu Datei > Drucken_.</li><li>Klicken: _Select File > Print_ oder _OK auswählen_. </li></ul>Siehe [Beschreibung der Interaktionen mit der Benutzeroberfläche](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) für weitere Ideen zur besten Wortwahl in verschiedenen Situationen. |
| Ausführen von Acrolinx in VSC | Acrolinx sucht nach Stil- und Grammatikproblemen. Er überprüft URLs, Terminologie, Rechtschreibung und mehr. Dies hilft Ihnen, die Übersetzungen in Experience League-Inhalten zu verbessern. |

{style=&quot;table-layout:auto&quot;}

Einige weitere Best Practices und Ressourcen:

* [Scannerinhalt](https://docs.microsoft.com/en-us/style-guide/scannable-content/): Helfen Sie Lesern, schnell zu finden, was sie brauchen, oder erkennen Sie genauso schnell, wenn sie nicht dort sind, wo sie sein müssen. Das Schreiben, um das Scannen zu erleichtern, kann dabei helfen.
* **Zahlen:** Im Textkörper können Sie ganze Zahlen von null bis neun ausdrucken und Zahlen von 10 oder mehr verwenden. Siehe [Zahlen](https://docs.microsoft.com/en-us/style-guide/numbers).
* Schreib, wie du sprichst, projektiere Freundlichkeit und komme schnell zum Punkt.

Siehe [Die 10 beliebtesten Tipps zum Schreiben](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) im [Microsoft® Stilhandbuch](https://docs.microsoft.com/en-us/style-guide/welcome/) für weitere Informationen.

## Alternativtext{#alt-text}

Fügen Sie Ihren Assets (Bildern) aussagekräftigen Alternativtext hinzu. Betrachten Sie Alternativtext, der Folgendes erfüllt:

* Das Ziel, das Kunden erreichen können (Aufgaben- oder Konzeptname)
* Die angezeigte Funktion oder Seite
* Der angezeigte Symbolname

Google berücksichtigt den Alternativtext in SEO-Ergebnissen.

## Lokalisierung - DNL und UICONTROL{#localization}

Sie müssen sich keine Gedanken darüber machen, ob Ihr Produkt lokalisiert ist oder welche Sprachen ExL verwendet. Sie können jedoch zur Verbesserung der Lokalisierungsqualität beitragen, indem Sie gegebenenfalls die beiden folgenden (erforderlichen) Markdown-Tags anwenden:

* `DNL`

   DNL-Mittel _nicht lokalisieren_. Sie verwenden es nur für markenmarkierte Produktnamen der Adobe, die alle auf Englisch bleiben müssen.

   Syntaxbeispiele: `[!DNL Adobe Campaign]` oder `[!DNL Workfront]`

   DNL ist nicht für Dateinamen oder URLs vorgesehen.

* `UICONTROL`

   UICONTROL gibt ein Steuerelement in der Benutzeroberfläche an (z. B. eine Option, ein Feld, eine Registerkarte, eine Seite, eine Gruppe von Optionen oder einen Funktionsnamen in der Benutzeroberfläche).

   Syntaxbeispiel: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Sie müssen diese Tags vor der Lokalisierung Ihres Inhalts anwenden.

### Verwenden von Adobe in Produktnamen{#product-names}

Für die Unternehmensidentität schließen wir normalerweise Folgendes ein: _Adobe_ in der ersten Referenz eines Produkts auf der Anführungsebene. Abhängig von Platzgründen können Sie die Adobe in einer Überschrift ablegen. Dann sollte jedoch der erste Verweis in der Textkopie den vollständigen Namen enthalten. Bestimmte Produkte, wie _Adobe Audition_ und _Adobe Premiere Pro_, erfordern die Verwendung von Adobe auf erster oder auffälliger Referenz in jedem Sicherheitenelement, da es Teil des rechtlichen, markenspezifischen Namens ist.

## Erste Absätze{#firstparas}

Ihr erster Absatz sollte das Thema definieren und beschreiben, was der Leser aus dem Lesen des Artikels lernt.

Beispiel für ersten Absatz (Konzept):

_Zielgruppen sind Sammlungen von Besuchern (eine Liste von Besucher-IDs). Der Zielgruppendienst von Adobe verwaltet die Übersetzung von Besucherdaten in die Zielgruppensegmentierung. Auf diese Weise erfolgt die Erstellung und Verwaltung von Zielgruppen so ähnlich wie die Erstellung und Verwendung von Segmenten, mit dem zusätzlichen Vorteil, dass die Zielgruppensegmente für die Experience Cloud freigegeben werden können._

Beispiel für ersten Absatz (Aufgabe):

_Erstellen Sie die Kundenattributquelle (CSV- und FIN-Dateien) und laden Sie die Daten hoch. Sobald Sie dazu bereit sind, aktivieren Sie die Datenquelle. Geben Sie die Attributdaten nach Aktivierung der Datenquelle an Analytics und Target weiter._

### SEO-Tipps für erste Absätze{#seo}

* Suchbegriffe in die ersten Absätze aufnehmen.
* Verwenden Sie Begriffe, die Leser verwenden.
* Fügen Sie Synonyme und ggf. frühere Begriffe ein. Beispiel: &quot;Der Experience Cloud-ID-Dienst (ECID), zuvor bekannt als _Besucher-ID_ oder als Akronyme wie MID bietet MCVID eine universelle, beständige ID zum Identifizieren von Besuchern.&quot;
* Schließen Sie SEO-Begriffe in Links ein.
* Vermeiden Sie es, wichtige Begriffe in komplexen Tabellen zu platzieren. Komplexe Tabellen liefern keine zuverlässigen Suchergebnisse. Text in Bildern wird nicht gesucht. Untertitel werden durchsucht.

## Großschreibung{#capitalization}

* Der Stil der Adobe verwendet für alle Titel, Überschriften, Unterüberschriften und Seitennavigationselemente eine großformatige Groß-/Kleinschreibung im Stilstil.
* Alle Wörter werden in Kleinbuchstaben geschrieben, mit Ausnahme des ersten Wortes und der richtigen Namen, wie z. B. die Namen von Marken, Lösungen und Diensten.
* Passen Sie die Groß-/Kleinschreibung in den Produktnamen von Tools, Optionen, Menüelementen, Dialogfeldern und Feldern an.

## Inhaltsverzeichnis{#using-toc}

Die `TOC.md` ist Ihr Inhaltsverzeichnis. Jeder Leitfaden sollte einen enthalten.

**Redaktionelle Anleitungen für ein Inhaltsverzeichnis**

* Großschreibung: Verwenden Sie für jeden Eintrag immer die Groß-/Kleinschreibung (ohne Abkürzungen). Beschreiben Sie nur formale Produktnamen oder Schnittstellenelemente (Seiten, Registerkarten, Felder, Optionen usw.). Passen Sie die Benutzeroberfläche an, wenn Sie darauf verweisen.
* Verb-Formular und -Parallelität: Verwenden Sie zwingend ein Verb und vermeiden Sie Geringe. Inhaltsverzeichnisse sind Listen. Versuchen Sie daher meistens, Listen parallel zu halten. Es gibt Ausnahmen, die manchmal nicht vermieden werden können. Verwenden Sie für konzeptionelle Seiten Nomen und Nomen. Verwenden Sie für Aufgaben Verben.

**Syntaxhinweise**

* Eine Abschnittsüberschrift (übergeordnet) im Inhaltsverzeichnis kann kein Link sein. Es gibt keine Seite mit Inhalt. Sie sollte einen Anker enthalten, z. B. `{#processing-rules}`.
* Sie müssen die richtige Syntax für Inhaltsverzeichnisüberschriften verwenden (z. B. `+ Processing rules {#processing-rules}`) und Links zu Inhaltsartikeln (z. B. `+ [Article name](article.md)`).
* Inhaltsverzeichnis-Artikeleinträge können eine gekürzte Version des Artikeltitels sein. Befolgen Sie die Standards für das Schreiben von Übersichten, Konzepten und Aufgaben in diesem Dokument.
* Vermeiden Sie es, dieselbe Datei mehrmals einem Inhaltsverzeichnis (oder mehreren Inhaltsverzeichnissen) hinzuzufügen. Dies führt zu seltsamem Verhalten.
* Wenn Ihr Repository mehrere Benutzerhandbücher enthält, müssen sich Ihre Benutzerhandbuch-Verzeichnisse auf derselben Ebene befinden, z. B. die Unterverzeichnisse innerhalb der `help` Verzeichnis. Jeder Benutzerhandbuch-Ordner muss über eine TOC-Datei verfügen. Keine verschachtelten Benutzerhandbücher.

## Fett und kursiv{#bold}

* Verwenden Sie fett gedruckten Text nur für Oberflächenelemente, auf die Sie in einem Verfahren klicken (und mit UICONTROL).
* Verwenden Sie Kursivformatierung für Hervorhebung oder wenn ein Wort ohne Wörter verwirrend ist. Zum Beispiel ein fremdes Wort, oder wenn Sie ein Wort beschreiben oder einen Begriff definieren.
