---
UID: NS:d3d10umddi.D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK
title: D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK (d3d10umddi.h)
description: D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK is used with VideoDecoderSubmitBuffers1 to describe the decoder buffer sub sample mapping block size.
old-location: display\d3dwddm2_0ddi_video_decoder_sub_sample_mapping_block.htm
ms.date: 05/10/2018
keywords: ["D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK structure"]
ms.keywords: D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK, D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK structure [Display Devices], d3d10umddi/D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK, display.d3dwddm2_0ddi_video_decoder_sub_sample_mapping_block
req.header: d3d10umddi.h
req.include-header: D3d10umddi.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10
req.target-min-winversvr: Windows Server 2016
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
req.typenames: D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK
f1_keywords:
 - D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK
 - d3d10umddi/D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - D3d10umddi.h
api_name:
 - D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK
---

# D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK structure


## -description

<b>D3DWDDM2_0DDI_VIDEO_DECODER_SUB_SAMPLE_MAPPING_BLOCK</b> is used with  <a href="/windows-hardware/drivers/ddi/d3d10umddi/nc-d3d10umddi-pfnd3dwddm2_0ddi_videodecodersubmitbuffers1">VideoDecoderSubmitBuffers1</a> to describe the decoder buffer sub sample mapping block size.

## -struct-fields

### -field ClearSize

The number of clear (non-encrypted) bytes at the start of the block.

### -field EncryptedSize

The number of encrypted bytes following the clear bytes.

## -remarks

Values in the sub sample mapping blocks are relative to the start of the decode buffer.

## -see-also

<a href="/windows-hardware/drivers/ddi/d3d10umddi/nc-d3d10umddi-pfnd3dwddm2_0ddi_videodecodersubmitbuffers1">VideoDecoderSubmitBuffers1</a>
