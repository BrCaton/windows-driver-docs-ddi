---
UID: NE:ntddstor._STORAGE_PROTOCOL_NVME_DATA_TYPE
title: STORAGE_PROTOCOL_NVME_DATA_TYPE (ntddstor.h)
description: Describes the type of NVMe protocol-specific data that is to be queried during an IOCTL_STORAGE_QUERY_PROPERTY request.
old-location: storage\storage_protocol_nvme_data_type.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["STORAGE_PROTOCOL_NVME_DATA_TYPE enumeration"]
ms.keywords: "*PSTORAGE_PROTOCOL_NVME_DATA_TYPE, NVMeDataTypeFeature, NVMeDataTypeIdentify, NVMeDataTypeLogPage, NVMeDataTypeUnknown, PSTORAGE_PROTOCOL_NVME_DATA_TYPE, PSTORAGE_PROTOCOL_NVME_DATA_TYPE enumeration pointer [Storage Devices], STORAGE_PROTOCOL_NVME_DATA_TYPE, STORAGE_PROTOCOL_NVME_DATA_TYPE enumeration [Storage Devices], _STORAGE_PROTOCOL_NVME_DATA_TYPE, ntddstor/NVMeDataTypeFeature, ntddstor/NVMeDataTypeIdentify, ntddstor/NVMeDataTypeLogPage, ntddstor/NVMeDataTypeUnknown, ntddstor/PSTORAGE_PROTOCOL_NVME_DATA_TYPE, ntddstor/STORAGE_PROTOCOL_NVME_DATA_TYPE, storage.storage_protocol_nvme_data_type"
req.header: ntddstor.h
req.include-header: Ntddstor.h
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
req.typenames: STORAGE_PROTOCOL_NVME_DATA_TYPE, *PSTORAGE_PROTOCOL_NVME_DATA_TYPE
f1_keywords:
 - _STORAGE_PROTOCOL_NVME_DATA_TYPE
 - ntddstor/_STORAGE_PROTOCOL_NVME_DATA_TYPE
 - PSTORAGE_PROTOCOL_NVME_DATA_TYPE
 - ntddstor/PSTORAGE_PROTOCOL_NVME_DATA_TYPE
 - STORAGE_PROTOCOL_NVME_DATA_TYPE
 - ntddstor/STORAGE_PROTOCOL_NVME_DATA_TYPE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ntddstor.h
api_name:
 - STORAGE_PROTOCOL_NVME_DATA_TYPE
---

# _STORAGE_PROTOCOL_NVME_DATA_TYPE enumeration

## -description

Describes the type of NVMe protocol-specific data that is to be queried during an [**IOCTL_STORAGE_QUERY_PROPERTY**](ni-ntddstor-ioctl_storage_query_property.md) request.

## -enum-fields

### -field NVMeDataTypeUnknown

Unknown data type.

### -field NVMeDataTypeIdentify

Identify data type. This value can be either IDENTIFY CONTROLLER data or IDENTIFY NAMESPACE data.

When this type of data is being queried, the **ProtocolDataRequestValue** field of [**STORAGE_PROTOCOL_SPECIFIC_DATA**](ns-ntddstor-_storage_protocol_specific_data.md) will have a value of **NVME_IDENTIFY_CNS_CONTROLLER** for adapter or **NVME_IDENTIFY_CNS_SPECIFIC_NAMESPACE** for namespace. If the **ProtocolDataRequestValue** is **NVME_IDENTIFY_CNS_SPECIFIC_NAMESPACE**, the **ProtocolDataRequestSubValue** field from the **STORAGE_PROTOCOL_SPECIFIC_DATA** structure will have a value of the namespace ID. (Note that **NVME_IDENTIFY_CNS_ACTIVE_NAMESPACES** is currently not supported.)

### -field NVMeDataTypeLogPage

Log page data type.

### -field NVMeDataTypeFeature

Feature data type.

## -remarks

When using [**IOCTL_STORAGE_QUERY_PROPERTY**](ni-ntddstor-ioctl_storage_query_property.md) to retrieve protocol-specific information in the [**STORAGE_PROTOCOL_DATA_DESCRIPTOR**](ns-ntddstor-_storage_protocol_data_descriptor.md), configure the [**STORAGE_PROPERTY_QUERY**](ns-ntddstor-_storage_property_query.md) structure as follows:

* Allocate a buffer that can contains both a [**STORAGE_PROPERTY_QUERY**](ns-ntddstor-_storage_property_query.md) and a [**STORAGE_PROTOCOL_SPECIFIC_DATA**](ns-ntddstor-_storage_protocol_specific_data.md) structure.

* Set the **PropertyID**  field to **StorageAdapterProtocolSpecificProperty** or **StorageDeviceProtocolSpecificProperty** for a controller or device/namespace request, respectively.

* Set the **QueryType**  field to **PropertyStandardQuery**.

* Fill the [**STORAGE_PROTOCOL_SPECIFIC_DATA**](ns-ntddstor-_storage_protocol_specific_data.md) structure with the desired values. The start of the **STORAGE_PROTOCOL_SPECIFIC_DATA** is the **AdditionalParameters** field of [**STORAGE_PROPERTY_QUERY**](ns-ntddstor-_storage_property_query.md).

To specify a type of NVMe protocol-specific information,  configure the [**STORAGE_PROTOCOL_SPECIFIC_DATA**](ns-ntddstor-_storage_protocol_specific_data.md) structure as follows:

* Set the **ProtocolType**  field to **ProtocolTypeNVMe**.

* Set the **DataType**  field to an enumeration value defined by **STORAGE_PROTOCOL_NVME_DATA_TYPE**:
  * Use **NVMeDataTypeIdentify** to get Identify Controller data or Identify Namespace data.
  * Use **NVMeDataTypeLogPage** to get log pages (including SMART/health data).
  * Use **NVMeDataTypeFeature** to get features of the NVMe drive.

## -see-also

[**IOCTL_STORAGE_QUERY_PROPERTY**](ni-ntddstor-ioctl_storage_query_property.md)

[**STORAGE_PROPERTY_ID**](ne-ntddstor-storage_property_id.md)

[**STORAGE_PROPERTY_QUERY**](ns-ntddstor-_storage_property_query.md)

[**STORAGE_PROTOCOL_SPECIFIC_DATA**](ns-ntddstor-_storage_protocol_specific_data.md)
