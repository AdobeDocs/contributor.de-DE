---
lastModified: 2018-06-28T00:00:00Z
title: Links in der Dokumentation verwenden
seo-title: Links in der Adobe Git-/Markdown-Dokumentation verwenden
description: Dieser Artikel enthält Anleitungen zum Erstellen von Links zu Inhalten und Bildern.
seo-description: Dieser Artikel enthält Anleitungen zum Erstellen von Links zu Inhalten und Bildern für die Adobe-Dokumentation.
translation-type: tm+mt
source-git-commit: 73ec3b8b63769a192ee16bec2720930ea6a9aaed
workflow-type: tm+mt
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

<!--
## Bob's link test

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> File Type </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>A comma-separated values file (such as one created in Excel). This is the file that contains the customer attribute data. See [Link TEST](/help/setup/full-workflow.md) </p> <p> <b>Naming requirements:</b> Ensure that file name extensions do not contain white spaces. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Required) The <span class="filepath"> .fin </span> file tells the system that you are finished uploading data. The name of the <span class="filepath"> .fin </span> file must match the name of the <span class="filepath"> .csv </span> file. </p> <p>Adobe recommends creating an empty text file with a <span class="filepath"> .fin </span> extension. An empty file saves space and upload time. </p> <p> <p>Note:  Renaming a <span class="filepath"> .fin </span> file is not allowed after it is uploaded. The <span class="filepath"> .fin </span> file must be uploaded separately and cannot be a renamed, previously uploaded file. </p> </p> <p>After you upload the <span class="filepath"> .fin </span> file in the customer attributes FTP, the system retrieves data quickly (within one minute). This differs from other Adobe FTP-based systems, which pick up data less frequently (around once per hour). </p> <p>The <span class="filepath"> .fin </span> file is not required when using the drag-and-drop upload method. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz </span> or <span class="filepath"> .zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz </span> (gzip) or <span class="filepath"> .zip </span> - for compressed files. A <span class="filepath"> .zip </span> file cannot contain more than one file in the archive. </p> <p> <b>Naming requirements:</b> The name of the <span class="filepath"> .zip </span> or <span class="filepath"> .gz </span> should match the name of the <span class="filepath"> .csv </span>. For example, if your <span class="filepath"> .csv </span> file is <span class="filepath"> crm_small.csv </span>, the <span class="filepath"> .zip </span> file should be <span class="filepath"> crm_small.csv.zip </span>. </p> <p>The .fin file must match the .csv. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
