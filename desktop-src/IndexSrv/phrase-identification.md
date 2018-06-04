---
Description: Phrase Identification
ms.assetid: 3b2f2405-e613-4ab7-b62d-f0dc05c65f50
title: Phrase Identification
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Phrase Identification

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

Phrases are a word or a group of words that are modified by one or more others. Phrases are difficult to identify consistently because the same modifier may be used in more than one phrase with the same noun. For example, "new house," "House of Parliament," "new House of Parliament."

Indexing Services uses phrases most often during query time. Phrases in query text receive higher weight than individual words. From the previous example, a document containing "House of Parliament" is ranked higher than one containing "House" and "Parliament" at different points in the document. It is recommended that word breakers generate a phrase at query time if the phrase is likely to match at least one document.

 

 


