---
title: "userPFXCertificate resource type"
description: "Entity that encapsulates all information required for a user's PFX certificates."
---

# userPFXCertificate resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Entity that encapsulates all information required for a user's PFX certificates.
## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection|List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.|
|[Get userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.|
|[Create userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.|
|[Delete userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|None|Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Update userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique identifier for the PFX certificate.|
|thumbprint|String|SHA-1 thumbprint of the PFX certificate.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Certificate's intended purpose from the point-of-view of deployment. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|User Principal Name of the PFX certificate.|
|startDateTime|DateTimeOffset|Certificate's validity start date/time.|
|expirationDateTime|DateTimeOffset|Certificate's validity expiration date/time.|
|providerName|String|Crypto provider used to encrypt this blob.|
|keyName|String|Name of the key (within the provider) used to encrypt the blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Padding scheme used by the provider during encryption/decryption. Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binary|Encrypted PFX blob.|
|encryptedPfxPassword|String|Encrypted PFX password.|
|createdDateTime|DateTimeOffset|Date/time when this PFX certificate was imported.|
|lastModifiedDateTime|DateTimeOffset|Date/time when this PFX certificate was last modified.|

## Relationships
None
## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





