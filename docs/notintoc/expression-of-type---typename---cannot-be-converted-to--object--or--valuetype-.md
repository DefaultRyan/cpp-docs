---
title: "Expression of type &#39;&lt;typename&gt;&#39; cannot be converted to &#39;Object&#39; or &#39;ValueType&#39;"
ms.custom: na
ms.date: "10/13/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "bc31394"
  - "vbc31394"
helpviewer_keywords: 
  - "BC31394"
ms.assetid: e6f76257-65bb-4954-99f9-90f282648354
caps.latest.revision: 7
ms.author: "billchi"
manager: "douge"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# Expression of type &#39;&lt;typename&gt;&#39; cannot be converted to &#39;Object&#39; or &#39;ValueType&#39;
An expression evaluates to a type that cannot be boxed by the common language runtime (CLR).  
  
 *Boxing* refers to the processing necessary to convert a type to `Object` or, on occasion, to \<xref:System.ValueType>. The common language runtime cannot box certain types, for example \<xref:System.ArgIterator> and \<xref:System.TypedReference>.  
  
 If you have not used `CType` or `CObj` in the statement containing this expression, [!INCLUDE[vbprvb](../cli/includes/vbprvb_md.md)] has attempted an implicit conversion that causes this error.  
  
 **Error ID:** BC31394  
  
### To correct this error  
  
1.  Locate the expression that evaluates to the cited type.  
  
2.  Locate the part of your statement that attempts to box the cited type.  
  
3.  Rewrite the statement to avoid the boxing conversion.  
  
## See Also  
 [Implicit and Explicit Conversions](../Topic/Implicit%20and%20Explicit%20Conversions%20\(Visual%20Basic\).md)