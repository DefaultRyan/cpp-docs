---
title: "_get_output_format"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
apiname: 
  - "_get_output_format"
apilocation: 
  - "msvcr110_clr0400.dll"
  - "msvcr100.dll"
  - "msvcr80.dll"
  - "msvcrt.dll"
  - "msvcr90.dll"
  - "msvcr120.dll"
  - "msvcr110.dll"
apitype: "DLLExport"
f1_keywords: 
  - "get_output_format"
  - "_get_output_format"
dev_langs: 
  - "C++"
  - "C"
helpviewer_keywords: 
  - "output formatting"
  - "get_output_format function"
  - "_get_output_format function"
ms.assetid: 0ce42f3b-3479-41c4-bcbf-1d21f7ee37e7
caps.latest.revision: 13
ms.author: "corob"
manager: "ghogen"
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
# _get_output_format
Gets the current value of the output format flag.  
  
> [!IMPORTANT]
>  This function is obsolete. Beginning in Visual Studio 2015, it is not available in the CRT.  
  
## Syntax  
  
```  
unsigned int _get_output_format();  
```  
  
## Return Value  
 The current value of the output format flag.  
  
## Remarks  
 The output format flag controls features of formatted I/O. At present the flag has two possible values: 0 and `_TWO_DIGIT_EXPONENT`. If `_TWO_DIGIT_EXPONENT` is set, the floating point numbers is printed with only two digits in the exponent unless a third digit is required by the size of the exponent. If the flag is zero, the floating point output displays three digits of exponent, using zeroes if necessary to pad the value to three digits.  
  
## Requirements  
  
|Routine|Required header|  
|-------------|---------------------|  
|`_get_output_format`|\<stdio.h>|  
  
 For more compatibility information, see [Compatibility](../crt/compatibility.md) in the Introduction.  
  
## .NET Framework Equivalent  
 Not applicable. To call the standard C function, use `PInvoke`. For more information, see [Platform Invoke Examples](../Topic/Platform%20Invoke%20Examples.md).  
  
## See Also  
 [printf, _printf_l, wprintf, _wprintf_l](../crt/printf--_printf_l--wprintf--_wprintf_l.md)   
 [printf_s, _printf_s_l, wprintf_s, _wprintf_s_l](../crt/printf_s--_printf_s_l--wprintf_s--_wprintf_s_l.md)   
 [printf Type Field Characters](../crt/printf-type-field-characters.md)   
 [_set_output_format](../crt/_set_output_format.md)