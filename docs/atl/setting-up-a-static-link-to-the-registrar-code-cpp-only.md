---
title: "Setting Up a Static Link to the Registrar Code (C++ Only) | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
helpviewer_keywords: ["statically linking to ATL Registrar code", "linking [C++], to ATL Registrar code"]
ms.assetid: 835f5885-87a6-48fa-91e6-60988ee65538
caps.latest.revision: 11
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# Setting Up a Static Link to the Registrar Code (C++ Only)
C++ clients can create a static link to the Registrar's code. Static linking of the Registrar's parser adds approximately 5K to a release build.  
  
 The simplest way to set up static linking assumes you have specified [DECLARE_REGISTRY_RESOURCEID](reference/registry-macros.md#declare_registry_resourceid) in your object's declaration. (This is the default specification used by the ATL.)  
  
### To create a static link using DECLARE_REGISTRY_RESOURCEID  
  
1.  Specify [/D](../build/reference/d-preprocessor-definitions.md)`_ATL_STATIC_REGISTRY` instead of /D**_ATL_DLL**.  
  
2.  Recompile.  
  
## See Also  
 [Registry Component (Registrar)](../atl/atl-registry-component-registrar.md)

