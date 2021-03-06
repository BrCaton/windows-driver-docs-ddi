---
UID: NS:d3dkmddi._DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
title: _DXGKARG_DESTROYPERIODICFRAMENOTIFICATION (d3dkmddi.h)
description: The arguments used to destroy a periodic frame notification.
old-location: display\dxgkarg_destroyperiodicframenotification.htm
ms.date: 05/10/2018
keywords: ["DXGKARG_DESTROYPERIODICFRAMENOTIFICATION structure"]
ms.keywords: DXGKARG_DESTROYPERIODICFRAMENOTIFICATION, DXGKARG_DESTROYPERIODICFRAMENOTIFICATION structure [Display Devices], _DXGKARG_DESTROYPERIODICFRAMENOTIFICATION, d3dkmddi/DXGKARG_DESTROYPERIODICFRAMENOTIFICATION, display.dxgkarg_destroyperiodicframenotification
req.header: d3dkmddi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
tech.root: display
req.typenames: DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
f1_keywords:
 - _DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
 - d3dkmddi/_DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
 - DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
 - d3dkmddi/DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - d3dkmddi.h
api_name:
 - DXGKARG_DESTROYPERIODICFRAMENOTIFICATION
---

# _DXGKARG_DESTROYPERIODICFRAMENOTIFICATION structure


## -description

The arguments used to destroy a periodic frame notification.

## -struct-fields

### -field hNotification

A handle to the notification object created by the KMD.

### -field hAdapter

A handle to the adapter that the notification object was created for.

