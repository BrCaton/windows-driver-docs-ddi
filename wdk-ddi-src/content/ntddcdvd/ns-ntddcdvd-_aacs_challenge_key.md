---
UID: NS:ntddcdvd._AACS_CHALLENGE_KEY
title: _AACS_CHALLENGE_KEY (ntddcdvd.h)
description: The AACS_CHALLENGE_KEY structure contains the challenge key that the device sends to the host.
old-location: storage\aacs_challenge_key.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["AACS_CHALLENGE_KEY structure"]
ms.keywords: "*PAACS_CHALLENGE_KEY, AACS_CHALLENGE_KEY, AACS_CHALLENGE_KEY structure [Storage Devices], PAACS_CHALLENGE_KEY, PAACS_CHALLENGE_KEY structure pointer [Storage Devices], _AACS_CHALLENGE_KEY, ntddcdvd/AACS_CHALLENGE_KEY, ntddcdvd/PAACS_CHALLENGE_KEY, storage.aacs_challenge_key, structs-DVD_7a8e1eeb-73f5-4d10-83c6-13bac3130c91.xml"
req.header: ntddcdvd.h
req.include-header: Ntddcdvd.h
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
req.typenames: AACS_CHALLENGE_KEY, *PAACS_CHALLENGE_KEY
f1_keywords:
 - _AACS_CHALLENGE_KEY
 - ntddcdvd/_AACS_CHALLENGE_KEY
 - PAACS_CHALLENGE_KEY
 - ntddcdvd/PAACS_CHALLENGE_KEY
 - AACS_CHALLENGE_KEY
 - ntddcdvd/AACS_CHALLENGE_KEY
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ntddcdvd.h
api_name:
 - AACS_CHALLENGE_KEY
---

# _AACS_CHALLENGE_KEY structure


## -description

The AACS_CHALLENGE_KEY structure contains the challenge key that the device sends to the host.

## -struct-fields

### -field EllipticCurvePoint

The elliptical curve (ECC) point data.

### -field Signature

The signature that the client uses to verify that the ECC point is valid for the current Advanced Access Content System (AACS) authentication sequence.

## -remarks

Clients retrieve the Advanced Access Content System (AACS) challenge key with an <a href="/windows-hardware/drivers/ddi/ntddcdvd/ni-ntddcdvd-ioctl_aacs_get_challenge_key">IOCTL_AACS_GET_CHALLENGE_KEY</a> request. Clients send an AACS challenge key to the logical unit in an <a href="/windows-hardware/drivers/ddi/ntddcdvd/ns-ntddcdvd-_aacs_send_challenge_key">AACS_SEND_CHALLENGE_KEY</a> structure with an <a href="/windows-hardware/drivers/ddi/ntddcdvd/ni-ntddcdvd-ioctl_aacs_send_challenge_key">IOCTL_AACS_SEND_CHALLENGE_KEY</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/ntddcdvd/ns-ntddcdvd-_aacs_send_challenge_key">AACS_SEND_CHALLENGE_KEY</a>



<a href="/windows-hardware/drivers/ddi/ntddcdvd/ni-ntddcdvd-ioctl_aacs_get_challenge_key">IOCTL_AACS_GET_CHALLENGE_KEY</a>



<a href="/windows-hardware/drivers/ddi/ntddcdvd/ni-ntddcdvd-ioctl_aacs_send_challenge_key">IOCTL_AACS_SEND_CHALLENGE_KEY</a>
