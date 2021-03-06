﻿# androidWorkProfilePkcsCertificateProfile resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Android Work Profile PKCS certificate profile

Inherits from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidWorkProfilePkcsCertificateProfiles](../api/intune_deviceconfig_androidworkprofilepkcscertificateprofile_list.md)|[androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md) collection|List properties and relationships of the [androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md) objects.|
|[Get androidWorkProfilePkcsCertificateProfile](../api/intune_deviceconfig_androidworkprofilepkcscertificateprofile_get.md)|[androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md)|Read properties and relationships of the [androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md) object.|
|[Create androidWorkProfilePkcsCertificateProfile](../api/intune_deviceconfig_androidworkprofilepkcscertificateprofile_create.md)|[androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md)|Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md) object.|
|[Delete androidWorkProfilePkcsCertificateProfile](../api/intune_deviceconfig_androidworkprofilepkcscertificateprofile_delete.md)|None|Deletes a [androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md).|
|[Update androidWorkProfilePkcsCertificateProfile](../api/intune_deviceconfig_androidworkprofilepkcscertificateprofile_update.md)|[androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md)|Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune_deviceconfig_subjectnameformat.md)|Certificate Subject Name Format. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune_deviceconfig_subjectalternativenametype.md)|Certificate Subject Alternative Name Type. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune_deviceconfig_certificatevalidityperiodscale.md)|Scale for the Certificate Validity Period. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune_deviceconfig_extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md)|
|certificationAuthority|String|PKCS Certification Authority|
|certificationAuthorityName|String|PKCS Certification Authority Name|
|certificateTemplateName|String|PKCS Certificate Template Name|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|rootCertificate|[androidWorkProfileTrustedRootCertificate](../resources/intune_deviceconfig_androidworkprofiletrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune_deviceconfig_androidworkprofilecertificateprofilebase.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfilePkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String"
}
```



