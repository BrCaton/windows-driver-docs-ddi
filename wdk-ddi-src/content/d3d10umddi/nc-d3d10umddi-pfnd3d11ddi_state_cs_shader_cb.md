---
UID: NC:d3d10umddi.PFND3D11DDI_STATE_CS_SHADER_CB
title: PFND3D11DDI_STATE_CS_SHADER_CB (d3d10umddi.h)
description: The pfnStateCsShaderCb function causes the Microsoft Direct3D 11 runtime to refresh the compute shader.
old-location: display\pfnstatecsshadercb.htm
ms.date: 05/10/2018
keywords: ["PFND3D11DDI_STATE_CS_SHADER_CB callback function"]
ms.keywords: PFND3D11DDI_STATE_CS_SHADER_CB, PFND3D11DDI_STATE_CS_SHADER_CB callback, d3d10umddi/pfnStateCsShaderCb, d3d11state_functions_8292f8aa-d925-4dc9-9d9c-ccbe10d7e15f.xml, display.pfnstatecsshadercb, pfnStateCsShaderCb, pfnStateCsShaderCb callback function [Display Devices]
req.header: d3d10umddi.h
req.include-header: D3d10umddi.h
req.target-type: Desktop
req.target-min-winverclnt: pfnStateCsShaderCb is supported beginning with the Windows 7 operating system.
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
req.typenames: 
f1_keywords:
 - PFND3D11DDI_STATE_CS_SHADER_CB
 - d3d10umddi/PFND3D11DDI_STATE_CS_SHADER_CB
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - d3d10umddi.h
api_name:
 - pfnStateCsShaderCb
---

# PFND3D11DDI_STATE_CS_SHADER_CB callback function


## -description

The <b>pfnStateCsShaderCb</b> function causes the Microsoft Direct3D 11 runtime to refresh the compute shader.

## -parameters

### -param Arg1

*hRuntimeDevice* [in]

A handle to a context for the core Direct3D runtime. This handle is supplied to the driver in a call to the driver's <a href="/windows-hardware/drivers/ddi/d3d10umddi/nc-d3d10umddi-pfnd3d10ddi_createdevice">CreateDevice(D3D10)</a> function.

## -see-also

<a href="/windows-hardware/drivers/ddi/d3d10umddi/nc-d3d10umddi-pfnd3d10ddi_createdevice">CreateDevice(D3D10)</a>



<a href="/windows-hardware/drivers/ddi/d3d10umddi/ns-d3d10umddi-d3d11ddi_corelayer_devicecallbacks">D3D11DDI_CORELAYER_DEVICECALLBACKS</a>
