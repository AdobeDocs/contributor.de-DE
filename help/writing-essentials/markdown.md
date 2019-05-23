---
lastModified: '2018-06-28'
title: Markdown zum Schreiben von Dokumentation verwenden
seo-title: Markdown zum Schreiben von Adobe-Dokumentation verwenden
description: In diesem Artikel finden Sie die Grundlagen und Referenzinformationen für die Markdown-Sprache, die zum Schreiben von Artikeln verwendet wird.
seo-description: In diesem Artikel finden Sie die Grundlagen und Referenzinformationen für die Markdown-Sprache, die zum Schreiben von Artikeln für Adobe-Dokumentation verwendet wird.
translation-type: tm+mt
source-git-commit: e7382ef4aefc69c6b4e7d78b7f34eaf897596eaf

---


# Markdown zum Schreiben von technischer Dokumentation verwenden

Die technischen Adobe-Dokumentationsartikel werden in einer einfachen Markup-Sprache namens [Markdown](https://daringfireball.net/projects/markdown/) geschrieben, die einfach zu lesen und zu lernen ist.

Wenn wir Adobe Docs-Inhalt in GitHub speichern, kann eine Version von Markdown mit dem Namen [GitHub Flavored Markdown (GFM)](https://help.github.com/categories/writing-on-github/) verwendet werden, die zusätzliche Funktionen für allgemeine Formatierungsanforderungen bietet. Außerdem erweiterte Adobe Markdown auf verschiedene Arten, um bestimmte Hilfefunktionen wie Anmerkungen, Tipps und eingebettete Videos zu unterstützen.

## Markdown-Grundlagen

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

<!--
To format superscript (H<sub>2</sub>O) and subscript (e=mc<sup>2</sup>) text:

```markdown
This is subscript H<sub>2</sub>O and superscript e=mc<sup>2</sup>.
```
-->

Um Markdown-Formatierungszeichen zu ignorieren, verwenden Sie \ vor dem Zeichen:

```markdown
This is not \*italicized\* type.
```

### Nummerierte Listen und Aufzählungslisten

Um nummerierte Listen zu erstellen, beginnen Sie eine Zeile mit „1.“ oder „1)“. Verwenden Sie jedoch nicht beide Formate in derselben Liste, sonst wird eine neue Liste gestartet. Sie müssen die Zahlen nicht speziell angeben. GitHub erledigt das für Sie.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Angezeigt:

1. Dies ist Schritt 1.
1. Dies ist der nächste Schritt.
1. Dies ist ein weiterer Schritt, der dritte.

<!-- markdownlint-disable MD037 -->
Um Listen mit Aufzählungszeichen zu erstellen, beginnen Sie eine Zeile mit „\*“, „-“ oder „+“, aber mischen Sie die Formate nicht in derselben Liste. (Wenn Sie die Formate wie „\*“ und „\+“ kombinieren, starten Sie im Grunde eine neue Liste.)
<!-- markdownlint-disable MD037 -->

```markdown
- First item in an unordered list.
- Another item.
- Here we go again.
```

Angezeigt:

- Erstes Element in einer ungeordneten Liste.
- Ein weiteres Element.
- Und noch ein weiteres.

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

1. Richten Sie Ihre Tabelle und Codeblöcke ein.
1. Führen Sie diesen Schritt aus.

   ![Bildschirm](assets/no-localize/adobe_standard_logo.png)
1. Stellen Sie sicher, dass die Tabelle wie folgt aussieht:

   | Hallo | Welt |
   |---|---|
   | Wie | geht&#39;s? |
1. Dies ist der vierte Schritt.

   >[!NOTE]
   >
   >Dies ist Anmerkungstext.
1. Führen Sie einen anderen Schritt aus.

### Tabellen

Tabellen sind nicht Teil der Markdown-Kernspezifikation, doch Adobe unterstützt sie in einem gewissen Maße. Markdown unterstützt keine Listen mit mehreren Zeilen in Zellen. Es empfiehlt sich, mehrere Zeilen in Tabellen zu vermeiden. Sie können Tabellen mit dem Strichzeichen (|) erstellen, um Spalten und Zeilen abzutrennen. Mit Bindestrichen wird die Kopfzeile der einzelnen Spalten erstellt, während die Striche die Spalten trennen. Fügen Sie vor der Tabelle eine leere Zeile ein, damit sie korrekt angezeigt wird.

```markdown
| Header | Another header | Yet another header |
|------------|:---------------:|-----------------------:|
| row 1 | centered column 2 | right-aligned column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Angezeigt:

| Kopfzeile | Noch eine Kopfzeile | Und eine weitere Kopfzeile |
|------------|:---------------:|-----------------------:|
| Zeile 1 | zentrierte Spalte 2 | rechtsbündige Spalte 3 |
| Zeile 2 | Zeile 2 Spalte 2 | Zeile 2 Spalte 3 |

Einfache Tabellen funktionieren in Markdown angemessen. Tabellen, die mehrere Absätze oder Listen in einer Zelle enthalten, sind jedoch schwer zu bearbeiten. Für solche Inhalte empfehlen wir ein anderes Format, z. B. Überschriften und Text.

Weitere Informationen zum Erstellen von Tabellen finden Sie unter:

- GitHub – [Informationen mit Tabellen organisieren](https://help.github.com/articles/organizing-information-with-tables/)
- Webapp [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
- [HTML-Tabellen in Markdown konvertieren](https://jmalarcon.github.io/markdowntables/)

### Links

Die Markdown-Syntax für einen Inline-Link besteht aus dem `[link text]`-Teil, der den Hyperlinktext enthält, gefolgt vom `(file-name.md)`-Teil, der die URL oder den Dateinamen enthält, mit der/dem verlinkt wird:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com) or <https://www.adobe.com>
```

Angezeigt:

[Adobe](https://www.adobe.com) oder <https://www.adobe.com>

Verwenden Sie relative Links für Verknüpfungen zu Artikeln (Querverweise) im Repository. Sie können alle relativen Link-Operanden verwenden, z. B.../ (aktuelles Verzeichnis), ../ (ein Verzeichnis zurück) und ../../ (zwei Verzeichnisse zurück).

```markdown
See [Overview example article](../../overview.md)
```

Weitere Informationen zur Verknüpfung finden Sie im Artikel [Links](linking.md) in diesem Handbuch zur Verknüpfungssyntax.

### Bilder

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Angezeigt:

![Adobe-Logo](assets/no-localize/adobe_standard_logo.png "Tooltip")

### Codeblöcke

Markdown unterstützt die Platzierung von Codeblöcken sowohl in einem Satz als auch als separater „abgegrenzter“ Block zwischen Sätzen. Weitere Informationen finden Sie unter [Native Markdown-Unterstützung für Codeblöcke.](https://daringfireball.net/projects/markdown/syntax#precode)

Verwenden Sie Backticks „\`“, um Inline-Codestile in einem Absatz zu erstellen. Um einen bestimmten mehrzeiligen Codeblock zu erstellen, fügen Sie vor und nach dem Codeblock (in Markdown als „abgegrenzter Codeblock“ und in AEM einfach als „Codeblock“ bezeichnet) drei Backticks „\`\`\`“ vor und nach dem Codeblock ein. Fügen Sie bei abgegrenzten Codeblöcken die Codesprache nach dem ersten Satz Backticks ein, sodass Markdown die Codesyntax korrekt hervorhebt. Beispiel: \`\`\`javascript

Beispiele:

```markdown
This is `inline code` within a paragraph of text.
```

Angezeigt:

Dies ist `inline code` in einem Textabschnitt.

Dies ist ein abgegrenzter Codeblock:

```markdown
\```javascript
function test() {
 console.log("notice the blank line before this function?");
\```
```

Angezeigt:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

Sie können Eigenschaften für Codeblöcke angeben, um die Zeilennummern (standardmäßig aktiviert) zu deaktivieren oder einen Zeilenumbruch hinzuzufügen (standardmäßig deaktiviert). Verwenden Sie {line-numbers=&quot;no&quot;} und {line-wrap=&quot;yes&quot;}. Diese Eigenschaften sind benutzerdefinierte Markdown-Erweiterungen.

\`\`\`javascript {line-numbers=&quot;no&quot;}
function test() {
console.log(&quot;Ist Ihnen die leere Zeile vor dieser Funktion aufgefallen?&quot;);
\`\`\`

### Definitionslisten

Eine Definitionsliste ist eine Markdown-Erweiterung, die die Komponente „Definitionsliste“ in AEM unterstützt. Eine Definitionsliste besteht aus einem Begriff und seiner Definition.

<!--

```markdown
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

Displayed:

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
--->

#### Anmerkungen und Kommentare

Kommentare (Anmerkungen) werden nicht in den öffentlichen Hilfeartikeln angezeigt. Kommentare werden jedoch in den öffentlichen Markdown-Dateien angezeigt, die Benutzer sehen und bearbeiten können.

## Benutzerspezifische Markdown-Erweiterungen

Adobe-Artikel verwenden Standard-Markdown für die meisten Artikelformatierungen wie Absätze, Links, Listen und Überschriften. Für eine reichhaltigere Formatierung können Artikel erweiterte Markdown-Funktionen verwenden, z. B.:

- Hinweisblöcke
- Eingebettete Videos
- Nicht lokalisieren
- Komponenteneigenschaften, z. B. Zuweisen einer anderen Kopfzeilen-ID zu einer Kopfzeile

Verwenden Sie das Markdown-Blockanführungszeichen (&gt;) am Anfang jeder Zeile, um eine erweiterte Komponente wie einen Hinweis anzubinden. Wenn Sie Unterkomponenten in Komponenten verwenden müssen, fügen Sie für diesen Unterkomponentenabschnitt eine zusätzliche Ebene von Blockanführungszeichen (&gt;  &gt;) hinzu. Beispielsweise sollte ein HINWEIS in einem NICHTLOKALISIEREN-Abschnitt mit &gt;    &gt; beginnen.

Einige gängige Markdown-Elemente wie Kopfzeilen und Codeblöcke umfassen erweiterte Eigenschaften. Wenn Sie die Standardeigenschaften ändern müssen, fügen Sie die Parameter in geschweiften Klammern /{ /} nach der Komponente hinzu. Erweiterte Eigenschaften werden im Kontext beschrieben.

### Hinweisblöcke

Sie können aus vier Arten von Hinweisblöcken wählen, um die Aufmerksamkeit auf bestimmte Inhalte zu lenken:

- `[!NOTE]`
- `[!CAUTION]`
- `[!TIP]`
- `[!IMPORTANT]`

Im Allgemeinen sollten Hinweise sparsam verwendet werden, da sie stören können. Obwohl sie auch Codeblöcke, Bilder, Listen und Links unterstützen, sollten Sie Ihre Hinweise einfach und geradlinig halten.


```markdown
>[!NOTE]
>This is a standard NOTE block.
```

Angezeigt:

>[!NOTE]
>Dies ist ein standardmäßiger HINWEIS-Block.

```markdown
>[!TIP]
>This is a standard tip.
```

Angezeigt:

>[!TIP]
>Dies ist ein Standardtipp.

### Videos

Eingebettete Videos werden nicht nativ in Markdown gerendert, Sie können aber diese Markdown-Erweiterung verwenden.

```markdown
>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)
```

Angezeigt:

>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)

### Mehr wie dieses

Die Komponente „Mehr wie dieses“ in AEM wird am Ende eines Artikels angezeigt. Es werden zugehörige Links angezeigt. Wenn der Artikel gerendert wird, kann er wie Ebene-2-Kopfzeilen (##) formatiert werden, ohne dem Mini-Inhaltsverzeichnis hinzugefügt zu werden.

<!--
```markdown
>[!MORE]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html){target="new-window"}
```

Displayed:

>[!MORE]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html){target="new-window"}
-->

### DNL – Do Not Localize (nicht lokalisieren) – und UICONTROL

In einigen Fällen müssen wir bestimmte Inhaltsabschnitte in einem Artikel so kennzeichnen, dass sie auf Englisch bleiben.
Wörter, Ausdrücke und andere Elemente müssen in unseren Übersetzungssystemen entsprechend deklariert werden, so kann ein gesteuertes Lexikon verwaltet werden.

Wörter oder Ausdrücke, die nicht lokalisiert werden sollen, können Sie in die `[!DNL]`-Erweiterung einschließen.

Für Elemente in der Benutzeroberfläche und Menüs einer Lösung verwenden wir die `[!UICONTROL]`-Erweiterung.

**Beispiel:**

In [!DNL Adobe Target] können Sie Ihre Tests direkt auf einer [!DNL Target]-aktivierten Seite erstellen.

**Quelle:**

```markdown
In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.
```

**Beispiel**

Verwenden Sie den [!UICONTROL Visual Experience Composer] in [!DNL Target], um Ihren Test direkt auf einer Seite zu erstellen.

**Quelle:**

```markdown
Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.
```

## Gotchas und Fehlerbehebung

### Alternativtext

Alternativtext, der Unterstriche enthält, wird nicht richtig gerendert. Statt dies zu verwenden:

```markdown
![Settings_Step_2] (/assets/settings_step_2.png)
```

empfehlen wir die Verwendung von Bindestrichen (-) anstelle von Unterstrichen (_) in Dateinamen.

```markdown
![Settings-Step-2] (/assets/settings-step-2.png)
```

### Apostrophe und Anführungszeichen

Wenn Sie Text in einen Markdown-Bearbeiter kopieren, kann der Text „smarte“ (geschweifte) Apostrophe oder Anführungszeichen enthalten. Diese müssen kodiert oder in einfache Apostrophe oder Anführungszeichen geändert werden. Andernfalls erhalten Sie korrupte Zeichen wie die folgenden, wenn die Datei veröffentlicht wird: Itâ€™s

Im Folgenden finden Sie die Kodierungen für die „smarten“ Versionen dieser Interpunktionszeichen:

- Anführungszeichen links (öffnend): `&#8220;`
- Anführungszeichen rechts (schließend): `&#8221;`
- Rechts (schließend) einfaches Anführungszeichen oder Apostroph: `&#8217;`
- Links (öffnend) einfaches Anführungszeichen (selten verwendet): `&#8216;`

### Spitze Klammern

Wenn Sie spitze Klammern im Text (nicht im Code) in Ihrer Datei verwenden, zum Beispiel, um einen Platzhalter anzugeben, müssen Sie die spitzen Klammern manuell kodieren. Andernfalls wird in Markdown davon ausgegangen, dass sie ein HTML-Tag sein sollen.

Kodieren Sie beispielsweise `<script name>` als `&lt;script name&gt;`

### Et-Zeichen in Titeln

Et-Zeichen (&amp;) sind in Titeln nicht zulässig. Verwenden Sie stattdessen „und“ oder die `&amp;`-Kodierung.

## Siehe auch

### Markdown-Ressourcen

- [Markdown-Einführung](https://daringfireball.net/projects/markdown/syntax)
- [GitHub-Markdown-Grundlagen](https://help.github.com/articles/markdown-basics/)
