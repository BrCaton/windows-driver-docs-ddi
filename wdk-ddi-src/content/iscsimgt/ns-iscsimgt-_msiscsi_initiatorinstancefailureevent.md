---
UID: NS:iscsimgt._MSiSCSI_InitiatorInstanceFailureEvent
title: _MSiSCSI_InitiatorInstanceFailureEvent (iscsimgt.h)
description: The MSiSCSI_InitiatorInstanceFailureEvent structure is used to report an event when an initiator instance failure occurs.
old-location: storage\msiscsi_initiatorinstancefailureevent.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["MSiSCSI_InitiatorInstanceFailureEvent structure"]
ms.keywords: "*PMSiSCSI_InitiatorInstanceFailureEvent, MSiSCSI_InitiatorInstanceFailureEvent, MSiSCSI_InitiatorInstanceFailureEvent structure [Storage Devices], PMSiSCSI_InitiatorInstanceFailureEvent, PMSiSCSI_InitiatorInstanceFailureEvent structure pointer [Storage Devices], _MSiSCSI_InitiatorInstanceFailureEvent, iscsimgt/MSiSCSI_InitiatorInstanceFailureEvent, iscsimgt/PMSiSCSI_InitiatorInstanceFailureEvent, storage.msiscsi_initiatorinstancefailureevent, structs-iSCSI_189ce06c-9fb3-49f5-9921-31c400c4ae23.xml"
req.header: iscsimgt.h
req.include-header: Iscsimgt.h
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
req.typenames: MSiSCSI_InitiatorInstanceFailureEvent, *PMSiSCSI_InitiatorInstanceFailureEvent
f1_keywords:
 - _MSiSCSI_InitiatorInstanceFailureEvent
 - iscsimgt/_MSiSCSI_InitiatorInstanceFailureEvent
 - PMSiSCSI_InitiatorInstanceFailureEvent
 - iscsimgt/PMSiSCSI_InitiatorInstanceFailureEvent
 - MSiSCSI_InitiatorInstanceFailureEvent
 - iscsimgt/MSiSCSI_InitiatorInstanceFailureEvent
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - iscsimgt.h
api_name:
 - MSiSCSI_InitiatorInstanceFailureEvent
---

# _MSiSCSI_InitiatorInstanceFailureEvent structure


## -description

The MSiSCSI_InitiatorInstanceFailureEvent structure is used to report an event when an initiator instance failure occurs.

## -struct-fields

### -field FailureType

A <a href="/windows-hardware/drivers/storage/iscsi-initiator-failure-type-qualifiers">ISCSI_INITIATOR_FAILURE_TYPE_QUALIFIERS</a> value that indicates why the initiator instance failed.

### -field RemoteNodeName

The name of the target that is associated with the initiator instance that is reporting a failure.

## -remarks

We recommend that you implement this class.

## -see-also

<a href="/windows-hardware/drivers/storage/iscsi-initiator-failure-type-qualifiers">ISCSI_INITIATOR_FAILURE_TYPE_QUALIFIERS</a>



<a href="/windows-hardware/drivers/storage/msiscsi-initiatorinstancefailureevent-wmi-class">MSiSCSI_InitiatorInstanceFailureEvent WMI Class</a>
