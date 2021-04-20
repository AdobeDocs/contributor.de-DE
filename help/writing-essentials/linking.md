---
lastModified: 2018-06-28T00:00:00Z
title: Links in der Dokumentation verwenden
seo-title: Links in der Adobe Git-/Markdown-Dokumentation verwenden
description: Dieser Artikel enthält Anleitungen zum Erstellen von Links zu Inhalten und Bildern.
seo-description: Dieser Artikel enthält Anleitungen zum Erstellen von Links zu Inhalten und Bildern für die Adobe-Dokumentation.
exl-id: f9d61aa9-931c-4654-ab21-c6e47936954e
translation-type: ht
source-git-commit: dad1df81797e6078645449501ed0661cf4bcf3ce
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# Links in der Dokumentation verwenden

Dieser Artikel beschreibt die Verwendung von Hyperlinks in Dokumentationsseiten. Links können mit einigen unterschiedlichen Konventionen einfach in Markdown eingefügt werden. Links verweisen auf Inhalte auf derselben Seite, auf andere benachbarte Seiten oder auf externe Sites und URLs.

>[!IMPORTANT]
>Alle Links sollten idealerweise sicher sein (`https` vs. `http`), wenn das Ziel dies unterstützt (was überwiegend der Fall sein sollte).

## Link zu URLs

Die Wörter, die Sie in den Linktext einschließen, sollten dem Titel der Seite entsprechen, auf die Sie verlinken, oder spezifischem, beschreibendem Text.

**Beispiele:**

- `For more information, see the [overview article](https://github.com/AdobeDocs/target.en/help/overview.md).`

- `For more details, see [Adobe Legal Concerns](https://www.adobe.com/legal).`

## Link von einem Artikel zu einem anderen

Verwenden Sie die folgende Linksyntax, um einen Inline-Link von einem Artikel zu einem anderen innerhalb desselben Repositorys zu erstellen:

- Ein Artikel in einem Ordner verlinkt auf einen anderen Artikel im selben Verzeichnis:

   `[link text](article-name.md)`

- Ein Artikel verlinkt aus einem Unterverzeichnis auf einen Artikel im Stammverzeichnis:

   `[link text](../article-name.md)`

- Ein Artikel verlinkt aus einem untergeordneten Unterverzeichnis auf einen Artikel im Stammverzeichnis:

   `[link text](../../article-name.md)`

- Ein Artikel im Stammordner verlinkt auf einen Artikel in einem Unterverzeichnis:

   `[link text](./directory/article-name.md)`

- Ein Artikel in einem Unterverzeichnis verlinkt auf einen Artikel in einem anderen Unterverzeichnis:

   `[link text](../directory/article-name.md)`

- Ein Artikel in einem untergeordneten Unterverzeichnis verlinkt auf einen Artikel in einem anderen Unterverzeichnis:

   `[link text](../../directory/article-name.md)`

## Link zu Ankern

Sie müssen keine Anker erstellen. Sie werden automatisch zum Veröffentlichungszeitpunkt aller H2-Überschriften generiert. Sie müssen nur Links zu den H2-Abschnitten (##) erstellen.

- So verlinken Sie auf eine Überschrift im selben Artikel:

   `[link](#the-text-of-the-level2-section-separated-by-hyphens)`

   `[Link to anchors](#links-to-anchors)`

- So verlinken Sie einen Anker in einem anderen Artikel im selben Unterverzeichnis:

   `[link text](article-name.md#anchor-name)`

   `[Configure your profile](overview.md#getting-started)`

- So verlinken Sie einen Anker in einem anderen Dienstunterverzeichnis:

   `[link text](../directory/article-name.md#anchor-name)`

   `[Configure your profile](../overview.md#configure-your-profile)`

## Link zu Bildern

Es empfiehlt sich, Bilder und Dateien in einem `assets`-Verzeichnis auf derselben Ebene wie die Markdown-Datei zu speichern, die darauf verlinkt.

- Ein Artikel verlinkt zu einem Bild im `assets`-Unterverzeichnis:

   `![alt text](assets/image-name.png)`

- Ein Artikel verlinkt zu einem Bild im `assets/no-localize`-Unterverzeichnis:

   `![alt text](assets/no-localize/image-name.png)`
