---
title: multiple-h1
description: Docs 組建問題 multiple-h1 的說明和解決方式。
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 12/12/2018
ms.prod: non-product-specific
ms.openlocfilehash: 55ce6260cb4d1e09f63e0540528576ed3fa165f8
ms.sourcegitcommit: 4053577bd0478d711257a283ee661d618b49c2df
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2019
ms.locfileid: "57427238"
---
# <a name="multiple-h1"></a>multiple-h1

## <a name="warning"></a>警告

`Multiple H1s are not allowed. You can only have one top-level heading.`

H1 指的是 Markdown 檔案中的第一個標題。 當發佈到 docs.microsoft.com 時，H1 會以大型字體顯示在頁面頂端。 H1 的建立方式為以單一井字 (#) 開始一行文字，其後跟隨一個空格，接著為標題文字。 您在每個檔案中只能有一個 H1。

## <a name="resolution"></a>解決方式

若要修正此問題，請將後續 H1 的標題層級變更為 H2 (`##`)，或重新組織您的檔案。 請注意，不允許略過標題層級，例如在 H1 後面接著 H3。

```markdown
---
author: meganbradley
ms.author: mbradley
---
# This is an H1

Some content...

## This is an H2
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]