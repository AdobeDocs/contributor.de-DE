---
title: Markdown zum Schreiben von Dokumentation verwenden
description: Erfahren Sie mehr über die Grundlagen des Markdown-Authorings. Suchen Sie Referenzinformationen für die Markdown-Sprache, die zum Schreiben von Artikeln verwendet wird.
exl-id: 3e5726e2-139e-4e44-ae5b-8a3ae4782faf
source-git-commit: fff920c9e98ca821a4180157174c2a2ee1b84cb8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 100%

---

# Markdown zum Schreiben von technischer Dokumentation verwenden

Die technischen Adobe-Dokumentationsartikel werden in einer einfachen Markup-Sprache namens [Markdown](https://daringfireball.net/projects/markdown/) geschrieben, die einfach zu lesen und zu lernen ist.

Wenn wir Adobe Docs-Inhalt in GitHub speichern, kann eine Version von Markdown mit dem Namen [GitHub Flavored Markdown (GFM)](https://help.github.com/categories/writing-on-github/) verwendet werden, die zusätzliche Funktionen für allgemeine Formatierungsanforderungen bietet. Außerdem erweiterte Adobe Markdown auf verschiedene Arten, um bestimmte Hilfefunktionen wie Anmerkungen, Tipps und eingebettete Videos zu unterstützen.

## Markdown-Grundlagen

In den folgenden Abschnitten werden die Grundlagen des Authorings in Markdown beschrieben.

### Überschriften

Um eine Überschrift zu erstellen, verwenden Sie ein Hash-Zeichen (#) am Anfang einer Zeile:

```
# This is level 1 (article title)
## This is level 2
### This is level 3
#### This is level 4
##### This is level 5
```

### Einfacher Text

Ein Absatz erfordert keine spezielle Syntax in Markdown.

Um Text **fett** zu formatieren, schließen Sie ihn in doppelte Sternchen ein. Um Text *kursiv* zu formatieren, schließen Sie ihn in einfache Sternchen ein:

```markdown
   This text is **bold**.
   This text is *italic*.
   This text is both ***bold and italic***.
```

Um Markdown-Formatierungszeichen zu ignorieren, verwenden Sie \ vor dem Zeichen:

```markdown
This is not \*italicized\* type.
```

### Nummerierte Listen und Aufzählungslisten

Um nummerierte Listen zu erstellen, beginnen Sie eine Zeile mit `1.` oder `1)`, aber mischen Sie die Formate nicht in derselben Liste. Sie müssen die Zahlen nicht speziell angeben. GitHub erledigt das für Sie.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Angezeigt:

1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.

Um Listen mit Aufzählungszeichen zu erstellen, beginnen Sie eine Zeile mit „\*“, „-“ oder „+“, aber mischen Sie die Formate nicht in derselben Liste. (Mischen Sie Aufzählungsformate wie \* und \+ nicht innerhalb desselben Dokuments.)

```markdown
* First item in an unordered list.
* Another item.
* Here we go again.
```

Angezeigt:

* First item in an unordered list.
* Another item.
* Und noch ein weiteres.

Sie können auch Listen in Listen einbetten und Inhalte zwischen Listenelementen hinzufügen.

```markdown
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/no-localize/adobe_standard_logo.png)

1. Make sure that your table looks like this: 

   | Hello | World |
   |---|---|
   | How | are you? |  

1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.
```

Angezeigt:

1. Set up your table and code blocks.
1. Perform this step.

   ![Bildschirm](assets/no-localize/adobe_standard_logo.png)

1. Make sure that your table looks like this:

   | Hello | World |
   |---|---|
   | How | are you? |

1. This is the fourth step.

   >[!NOTE]
   >
   >Dies ist Anmerkungstext.

1. Do another step.

### Tabellen

Tabellen sind nicht Teil der Markdown-Kernspezifikation, doch Adobe unterstützt sie in einem gewissen Maße. Markdown unterstützt keine Listen mit mehreren Zeilen in Zellen. Best practice ist, mehrere Zeilen in Tabellen zu vermeiden. Sie können Tabellen mit dem Strichzeichen (|) erstellen, um Spalten und Zeilen abzutrennen. Mit Bindestrichen wird die Kopfzeile der einzelnen Spalten erstellt, während die Striche die Spalten trennen. Fügen Sie vor der Tabelle eine leere Zeile ein, damit sie korrekt angezeigt wird.

```markdown
| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Angezeigt:

| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |

Einfache Tabellen funktionieren in Markdown angemessen. Tabellen, die mehrere Absätze oder Listen in einer Zelle enthalten, sind jedoch schwer zu bearbeiten. Für solche Inhalte empfehlen wir ein anderes Format, z. B. Überschriften und Text.

Weitere Informationen zum Erstellen von Tabellen finden Sie unter:

* GitHub – [Informationen mit Tabellen organisieren](https://docs.github.com/de/github/writing-on-github/organizing-information-with-tables)
* Webapp [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
* [HTML-Tabellen in Markdown konvertieren](https://jmalarcon.github.io/markdowntables/)

### Links

Die Markdown-Syntax für einen Inline-Link besteht aus dem `[link text]`-Teil, der den Hyperlinktext enthält, gefolgt vom `(file-name.md)`-Teil, der die URL oder den Dateinamen enthält, mit der/dem verlinkt wird:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com)
```

Angezeigt:

[Adobe](https://www.adobe.com)

Verwenden Sie relative Links für Verknüpfungen zu Artikeln (Querverweise) im Repository. Sie können alle relativen Link-Operanden verwenden, z. B. ./ (aktuelles Verzeichnis), ../ (ein Verzeichnis zurück) und ../../ (zwei Verzeichnisse zurück).

```markdown
See [Overview example article](../../overview.md)
```

Weitere Informationen zur Verknüpfung finden Sie im Artikel [Links](linking.md) in diesem Handbuch zur Verknüpfungssyntax.

### Bilder

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Angezeigt:

![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")

### Codeblöcke

Markdown unterstützt die Platzierung von Codeblöcken sowohl in einem Satz als auch als separater „abgegrenzter“ Block zwischen Sätzen. Weitere Informationen finden Sie unter [Native Markdown-Unterstützung für Code-Blöcke](https://daringfireball.net/projects/markdown/syntax#precode)

Verwenden Sie Backticks (`` ` ``), um Inline-Code-Stile innerhalb eines Absatzes zu erstellen. Um einen bestimmten mehrzeiligen Code-Block zu erstellen, fügen Sie drei Backticks (` ``` `) vor und nach dem Code-Block ein (in Markdown „umgrenzter Code-Block“ genannt und in AEM einfach eine „Code-Block“-Komponente). Fügen Sie bei abgegrenzten Code-Blöcken die Code-Sprache nach dem ersten Satz Backticks ein, sodass Markdown die Code-Syntax korrekt hervorhebt. Beispiel: ` ```javascript`

Beispiele:

```markdown
This is `inline code` within a paragraph of text.
```

Angezeigt:

This is `inline code` within a paragraph of text.

Dies ist ein abgegrenzter Codeblock:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

## Benutzerspezifische Markdown-Erweiterungen

Adobe-Artikel verwenden Standard-Markdown für die meisten Artikelformatierungen wie Absätze, Links, Listen und Überschriften. Für eine reichhaltigere Formatierung können Artikel erweiterte Markdown-Funktionen verwenden, z. B.:

* Hinweisblöcke
* Eingebettete Videos
* Übersetzungs-Tags
* Komponenteneigenschaften, z. B. Zuweisen einer anderen Überschriften-ID zu einer Überschrift und Festlegen einer Bildgröße

Verwenden Sie das Markdown-Blockanführungszeichen (>) am Anfang jeder Zeile, um eine erweiterte Komponente wie einen Hinweis anzubinden.

Einige gängige Markdown-Elemente wie Kopfzeilen und Codeblöcke umfassen erweiterte Eigenschaften. Wenn Sie die Standardeigenschaften ändern müssen, fügen Sie die Parameter in geschweiften Klammern /{ /} nach der Komponente hinzu. Erweiterte Eigenschaften werden im Kontext beschrieben.

### Hinweisblöcke

Sie können aus vier Arten von Hinweisblöcken wählen, um die Aufmerksamkeit auf bestimmte Inhalte zu lenken:

* `[!NOTE]`
* `[!TIP]`
* `[!IMPORTANT]`
* `[!CAUTION]`
* `[!WARNING]`
* `[!ADMINISTRATION]`
* `[!AVAILABILITY]`
* `[!PREREQUISITES]`
* `[!ERROR]`
* `[!ADMINISTRATION]`
* `[!INFO]`
* `[!SUCCESS]`

Im Allgemeinen sollten Hinweise sparsam verwendet werden, da sie stören können. Obwohl sie auch Codeblöcke, Bilder, Listen und Links unterstützen, sollten Sie Ihre Hinweise einfach und geradlinig halten.


```markdown
>[!NOTE]
>
>This is a standard NOTE block.
```

```markdown
>[!TIP]
>
>This is a standard TIP.
```

```markdown
>[!IMPORTANT]
>
>This is an IMPORTANT note.
```

Angezeigt:

![Gerenderte Hinweise](assets/notes-rendered.png)

### Videos

Eingebettete Videos werden nicht nativ in Markdown gerendert, Sie können aber diese Markdown-Erweiterung verwenden.

```markdown
>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)
```

Angezeigt:

>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)

### Mehr wie dieses

Die Komponente „Mehr wie dieses“ in AEM wird am Ende eines Artikels angezeigt. Es werden zugehörige Links angezeigt. Wenn der Artikel gerendert wird, kann er wie Ebene-2-Kopfzeilen (##) formatiert werden, ohne dem Mini-Inhaltsverzeichnis hinzugefügt zu werden.

![mehr wie diese Syntax](assets/more-like-this-syntax.png)

Angezeigt:

>[!MORELIKETHIS]
>
>* [Artikel 1](https://helpx.adobe.com/de/support/analytics.html)
>* [Artikel 2](https://helpx.adobe.com/de/support/audience-manager.html)

### UICONTROL und DNL

Alle unsere Markdown-Hilfeinhalte werden zunächst durch maschinelle Übersetzung lokalisiert. Wenn die Hilfe noch nie lokalisiert wurde, behalten wir die maschinelle Übersetzung bei. Wenn der Hilfeinhalt jedoch in der Vergangenheit lokalisiert wurde, fungiert der maschinell übersetzte Inhalt als Platzhalter, während der Inhalt manuell übersetzt wird.

**``**

Während der maschinellen Übersetzung werden Elemente, die mit ``-Tags versehen sind, für die entsprechende Übersetzung mit einer lokalen Anpassungsdatenbank abgeglichen. Für den Fall, dass die Benutzeroberfläche nicht lokalisiert ist, ermöglicht dieses Tag dem System, die Benutzeroberflächenreferenz in Englisch für die jeweilige Sprache zu belassen (z. B. Analytics-Referenzen in Italienisch).

**Beispielquellinhalt:**

![Beispiel-UICONTROL-Text](assets/sample-uicontrol.png)

<!--
**Source:**

```markdown
1. Go to the **[!UICONTROL Run Process]** screen.
1. Choose **[!UICONTROL File] > [!UICONTROL Print] > [!UICONTROL Print All]** to print all the files on your server.
1. The [!UICONTROL Processing Rules] dialog box appears.
```

>[!NOTE]
>
>Of the two tagging options, this is the most crucial to deliver high quality and is mandatory.
-->

**`[!DNL]`**

In der Regel wird eine „Nicht übersetzen“-Liste verwendet, um den maschinellen Übersetzungsprogrammen mitzuteilen, was auf Englisch bleiben soll. Zu den häufigsten Begriffen gehören lange Lösungsnamen wie „Adobe Analytics“, „Adobe Campaign“ und „Adobe Target“. Es kann jedoch vorkommen, dass zwingend Englisch genutzt werden muss, weil der betreffende Begriff auf eine bestimmte oder allgemeine Weise verwendet werden kann. Am naheliegendsten sind Kurzbezeichnungen für die Lösungen wie „Analytics“, „Campaign“, „Target“ usw. Es wäre für eine Maschine schwierig zu verstehen, dass es sich um Lösungsnamen und nicht um allgemeine Begriffe handelt. Das Tag kann auch für Namen/Funktionen von Drittanbietern verwendet werden, die immer in Englisch bleiben, oder für kürzere Textabschnitte wie eine Wortgruppe oder einen Satz, die in Englisch bleiben müssen.

**Beispielquellinhalt:**

![Beispiel-DNL-Text](assets/sample-dnl.png)

<!--
**Source:**

```markdown
* With [!DNL Target], you can create A/B tests to find the optimal 
* Adobe Analytics is a powerful solution to collect analytics on your site. [!DNL Analytics] can also help you with reporting to easily digest that data.
```
-->

## Gotchas und Fehlerbehebung

### Alternativtext

Alternativtext, der Unterstriche enthält, wird nicht richtig gerendert. Statt dies zu verwenden:

```markdown
![Settings_Step_2](/assets/settings_step_2.png)
```

Unsere Best practice ist es, Bindestrichen (-) anstelle von Unterstrichen (_) in Dateinamen zu verwenden.

```markdown
![Settings-Step-2](/assets/settings-step-2.png)
```

### Apostrophe und Anführungszeichen

Wenn Sie Text in einen Markdown-Bearbeiter kopieren, kann der Text „smarte“ (geschweifte) Apostrophe oder Anführungszeichen enthalten. Diese müssen kodiert oder in einfache Apostrophe oder Anführungszeichen geändert werden. Andernfalls erhalten Sie korrupte Zeichen wie die folgenden, wenn die Datei veröffentlicht wird: Itâ€™s

Im Folgenden finden Sie die Kodierungen für die „smarten“ Versionen dieser Interpunktionszeichen:

* Anführungszeichen links (öffnend): `&#8220;`
* Anführungszeichen rechts (schließend): `&#8221;`
* Rechts (schließend) einfaches Anführungszeichen oder Apostroph: `&#8217;`
* Links (öffnend) einfaches Anführungszeichen (selten verwendet): `&#8216;`

### Spitze Klammern

Wenn Sie spitze Klammern im Text (nicht im Code) in Ihrer Datei verwenden, zum Beispiel, um einen Platzhalter anzugeben, müssen Sie die spitzen Klammern manuell kodieren. Andernfalls wird in Markdown davon ausgegangen, dass sie ein HTML-Tag sein sollen.

Kodieren Sie beispielsweise `<script name>` als `&lt;script name&gt;`

### Et-Zeichen in Titeln

Et-Zeichen (&amp;) sind in Titeln nicht zulässig. Verwenden Sie stattdessen „und“ oder die `&amp;`-Kodierung.

## Siehe auch

### Markdown-Ressourcen

* [Markdown-Einführung](https://daringfireball.net/projects/markdown/syntax)
* [GitHub-Markdown-Grundlagen](https://docs.github.com/de/github/writing-on-github/getting-started-with-writing-and-formatting-on-github)
