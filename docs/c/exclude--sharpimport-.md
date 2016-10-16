---
title: "exclude (#import)"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "exclude"
dev_langs: 
  - "C++"
  - "C"
helpviewer_keywords: 
  - "exclude attribute"
ms.assetid: 0883248a-d4bf-420e-9848-807b28fa976e
caps.latest.revision: 4
ms.author: "corob"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# exclude (#import)
**C++ Specific**  
  
 Excludes items from the type library header files being generated.  
  
## Syntax  
  
```  
exclude("Name1"[, "Name2",...])  
```  
  
#### Parameters  
 `Name1`  
 First item to be excluded.  
  
 `Name2`  
 Second item to be excluded (if necessary).  
  
## Remarks  
 Type libraries may include definitions of items defined in system headers or other type libraries. This attribute can take any number of arguments, each being a top-level type library item to be excluded.  
  
 **END C++ Specific**  
  
## See Also  
 [#import Attributes](../c/sharpimport-attributes--c---.md)   
 [#import Directive](../c/sharpimport-directive--c---.md)