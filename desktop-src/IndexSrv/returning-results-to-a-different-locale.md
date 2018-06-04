---
Description: Returning Results to a Different Locale
ms.assetid: c0f861f1-2cf5-43a2-bfdc-c03d090cdc3a
title: Returning Results to a Different Locale
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Returning Results to a Different Locale

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

If you are expecting queries from sites in different locales, you can set [CiCodepage](https://www.bing.com/search?q=CiCodepage) in the .htm file .htx (and .htw) file to make sure results are displayed correctly when returned to the client.

You can set the value of [CiCodepage](https://www.bing.com/search?q=CiCodepage) to CiCodepage=&lt;%CiCodepage%&gt; through the URL. Indexing Service takes the value sent by the browser to parse the query with the proper character set. If the CiCodepage variable is set with the same CiCodepage value that is in the .idq file, the CiCodepage variable can be referenced in the .htx or .htw file to display the result in the proper character set.

 

 


