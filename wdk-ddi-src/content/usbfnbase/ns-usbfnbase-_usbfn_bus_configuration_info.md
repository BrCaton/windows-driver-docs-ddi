---
UID: NS:usbfnbase._USBFN_BUS_CONFIGURATION_INFO
title: _USBFN_BUS_CONFIGURATION_INFO (usbfnbase.h)
description: Configuration packet that stores information about an available USB configuration.
old-location: buses\usbfn_bus_configuration_info.htm
tech.root: usbref
ms.date: 05/07/2018
keywords: ["USBFN_BUS_CONFIGURATION_INFO structure"]
ms.keywords: "*PUSBFN_BUS_CONFIGURATION_INFO, PUSBFN_BUS_CONFIGURATION_INFO, PUSBFN_BUS_CONFIGURATION_INFO structure pointer [Buses], USBFN_BUS_CONFIGURATION_INFO, USBFN_BUS_CONFIGURATION_INFO structure [Buses], _USBFN_BUS_CONFIGURATION_INFO, buses.usbfn_bus_configuration_info, usbfnbase/PUSBFN_BUS_CONFIGURATION_INFO, usbfnbase/USBFN_BUS_CONFIGURATION_INFO"
req.header: usbfnbase.h
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
req.typenames: USBFN_BUS_CONFIGURATION_INFO, *PUSBFN_BUS_CONFIGURATION_INFO
f1_keywords:
 - _USBFN_BUS_CONFIGURATION_INFO
 - usbfnbase/_USBFN_BUS_CONFIGURATION_INFO
 - PUSBFN_BUS_CONFIGURATION_INFO
 - usbfnbase/PUSBFN_BUS_CONFIGURATION_INFO
 - USBFN_BUS_CONFIGURATION_INFO
 - usbfnbase/USBFN_BUS_CONFIGURATION_INFO
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - usbfnbase.h
api_name:
 - USBFN_BUS_CONFIGURATION_INFO
---

# _USBFN_BUS_CONFIGURATION_INFO structure


## -description

Configuration packet that stores information about 
an available USB configuration.

## -struct-fields

### -field ConfigurationName

A NULL-terminated string that indicates the name of a configuration.

### -field IsCurrent

Indicates whether this configuration is the 
    current configuration.

### -field IsActive

    Indicates whether the configuration is active. This is a read-only information that is returned by USB function class extension (UFX) and is ignored in requests sent to UFX.

