---
Description: Filtering File Contents
ms.assetid: 2a4aeff0-9abc-4223-b31c-99ec5b4c044d
title: Filtering File Contents
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Filtering File Contents

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The CiDaemon.exe process of Indexing Service filters a file by successively calling the [IFilter::GetChunk](/windows/desktop/api/Filter/nf-filter-ifilter-getchunk) method to retrieve one of two kinds of content: text-type properties or value-type properties. The [IFilter::GetText](/windows/desktop/api/Filter/nf-filter-ifilter-gettext) method retrieves text from the first category, and the [IFilter::GetValue](/windows/desktop/api/Filter/nf-filter-ifilter-getvalue) method retrieves values from the second category. For more information about retrieving property values, see [Filtering File Properties](filtering-file-properties.md). Text chunks can have a locale attribute that indicates the type of word-breaker to use, based on the language in which the chunk is written. The resulting word list is normalized (converted to uppercase and given other minor conversions for comparison purposes) and then stored in a word list in memory. Word lists eventually merge into the master index.

When filtering a file, you generally want to filter any linked and embedded objects that you want associated with the top-level object. An HTML link, for example, may not reflect the contents of the outer document and so should not be filtered with the parent object. However, it may be quite suitable to include an embedded Microsoft Excel chart when filtering the parent object, a Word document, for example. For filtering purposes, logical containment is more important than physical containment. If you want to be able to search for information, filter it.

Logical containment results when you have either of the following.

-   [Embedded Objects](embedded-objects.md)
-   [Linked Objects](linked-objects.md)

 

 


