---
title: "msfp_satisfactionmetric Entity Reference | MicrosoftDocs"
description: "Includes schema information and supported messages for the msfp_satisfactionmetric entity."
ms.date: 07/29/2020
ms.service: 
  - crm-online
ms.topic: "reference"
author: "sbmjais"
ms.author: "shjais"
manager: "shujoshi"
---

# msfp_satisfactionmetric Entity Reference

Satisfaction metric defined for a project.

**Added by**: Dynamics 365 Customer Voice Solution

## Entity Properties

|Property|Value|
|--------|-----|
|CollectionSchemaName|msfp_satisfactionmetrics|
|DisplayCollectionName|Customer Voice satisfaction metrics|
|DisplayName|Customer Voice satisfaction metric|
|EntitySetName|msfp_satisfactionmetrics|
|IsBPFEntity|False|
|LogicalCollectionName|msfp_satisfactionmetrics|
|LogicalName|msfp_satisfactionmetric|
|OwnershipType|UserOwned|
|PrimaryIdAttribute|msfp_satisfactionmetricid|
|PrimaryNameAttribute|msfp_name|
|SchemaName|msfp_satisfactionmetric|

<a name="writable-attributes"></a>	

## Writable attributes	

These attributes return true for either **IsValidForCreate** or **IsValidForUpdate** (usually both). Listed by **SchemaName**.	

- [ImportSequenceNumber](#BKMK_ImportSequenceNumber)	
- [msfp_description](#BKMK_msfp_description)	
- [msfp_historicalcomputedvalue](#BKMK_msfp_historicalcomputedvalue)	
- [msfp_issystemkpi](#BKMK_msfp_issystemkpi)	
- [msfp_lastcomputedon](#BKMK_msfp_lastcomputedon)	
- [msfp_lastcomputedvalue](#BKMK_msfp_lastcomputedvalue)	
- [msfp_maximumvalue](#BKMK_msfp_maximumvalue)	
- [msfp_minimumvalue](#BKMK_msfp_minimumvalue)	
- [msfp_name](#BKMK_msfp_name)	
- [msfp_project](#BKMK_msfp_project)	
- [msfp_questions](#BKMK_msfp_questions)	
- [msfp_satisfactionmetricId](#BKMK_msfp_satisfactionmetricId)	
- [msfp_status](#BKMK_msfp_status)	
- [msfp_threshold](#BKMK_msfp_threshold)	
- [msfp_type](#BKMK_msfp_type)	
- [msfp_versionnumber](#BKMK_msfp_versionnumber)	
- [OverriddenCreatedOn](#BKMK_OverriddenCreatedOn)	
- [OwnerId](#BKMK_OwnerId)	
- [OwnerIdType](#BKMK_OwnerIdType)	
- [statecode](#BKMK_statecode)	
- [statuscode](#BKMK_statuscode)	
- [TimeZoneRuleVersionNumber](#BKMK_TimeZoneRuleVersionNumber)	
- [UTCConversionTimeZoneCode](#BKMK_UTCConversionTimeZoneCode)

### <a name="BKMK_ImportSequenceNumber"></a> ImportSequenceNumber

|Property|Value|
|--------|-----|
|Description|Sequence number of the import that created this record.|
|DisplayName|Import Sequence Number|
|Format|None|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|importsequencenumber|
|MaxValue|2147483647|
|MinValue|-2147483648|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_msfp_description"></a> msfp_description

|Property|Value|
|--------|-----|
|Description|Description of the satisfaction metric.|
|DisplayName|Description|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_description|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_historicalcomputedvalue"></a> msfp_historicalcomputedvalue

|Property|Value|
|--------|-----|
|Description|Historical computed value of the satisfaction metric.|
|DisplayName|Historical computed value|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_historicalcomputedvalue|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_issystemkpi"></a> msfp_issystemkpi

|Property|Value|
|--------|-----|
|Description|Indicates if the satisfaction metric is system defined or user defined.|
|DisplayName|Is system KPI|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_issystemkpi|
|RequiredLevel|None|
|Type|Boolean|

#### msfp_issystemkpi Options

|Value|Label|
|-----|-----|
|1|True|
|0|False|

**DefaultValue**: False



### <a name="BKMK_msfp_lastcomputedon"></a> msfp_lastcomputedon

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Date and time when the satisfaction metric was last computed.|
|DisplayName|Last computed on|
|Format|DateAndTime|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_lastcomputedon|
|RequiredLevel|None|
|Type|DateTime|


### <a name="BKMK_msfp_lastcomputedvalue"></a> msfp_lastcomputedvalue

|Property|Value|
|--------|-----|
|Description|Last computed value of the satisfaction metric.|
|DisplayName|Last Computed Value|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_lastcomputedvalue|
|MaxLength|4000|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_msfp_maximumvalue"></a> msfp_maximumvalue

|Property|Value|
|--------|-----|
|Description|Maximum value of the satisfaction metric.|
|DisplayName|Maximum value|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_maximumvalue|
|MaxValue|2147483647|
|MinValue|0|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_msfp_minimumvalue"></a> msfp_minimumvalue

|Property|Value|
|--------|-----|
|Description|Minimum value of the satisfaction metric.|
|DisplayName|Minimum value|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_minimumvalue|
|MaxValue|2147483647|
|MinValue|0|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_msfp_name"></a> msfp_name

|Property|Value|
|--------|-----|
|Description|Name of the satisfaction metric.|
|DisplayName|Name|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_name|
|MaxLength|550|
|RequiredLevel|ApplicationRequired|
|Type|String|


### <a name="BKMK_msfp_project"></a> msfp_project

|Property|Value|
|--------|-----|
|Description|Project to which the satisfaction metric belongs.|
|DisplayName|Project|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_project|
|RequiredLevel|ApplicationRequired|
|Targets|msfp_project|
|Type|Lookup|


### <a name="BKMK_msfp_questions"></a> msfp_questions

|Property|Value|
|--------|-----|
|Description|Questions on which the satisfaction metric is calculated.|
|DisplayName|Questions|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_questions|
|MaxLength|50000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_satisfactionmetricId"></a> msfp_satisfactionmetricId

|Property|Value|
|--------|-----|
|Description|Unique identifier for entity instances|
|DisplayName|Customer Voice satisfaction metric|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|msfp_satisfactionmetricid|
|RequiredLevel|SystemRequired|
|Type|Uniqueidentifier|


### <a name="BKMK_msfp_status"></a> msfp_status

|Property|Value|
|--------|-----|
|Description|Status of the satisfaction metric.|
|DisplayName|Status|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_status|
|RequiredLevel|None|
|Type|Picklist|

#### msfp_status Options

|Value|Label|
|-----|-----|
|647390000|Active|
|647390001|InActive|



### <a name="BKMK_msfp_threshold"></a> msfp_threshold

|Property|Value|
|--------|-----|
|Description|Threshold value of the satisfaction metric.|
|DisplayName|Threshold|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_threshold|
|MaxValue|2147483647|
|MinValue|-2147483648|
|RequiredLevel|ApplicationRequired|
|Type|Integer|


### <a name="BKMK_msfp_type"></a> msfp_type

|Property|Value|
|--------|-----|
|Description|Type of the satisfaction metric.|
|DisplayName|Type|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_type|
|MaxLength|200|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_msfp_versionnumber"></a> msfp_versionnumber

|Property|Value|
|--------|-----|
|Description|Version number of the satisfaction metric.|
|DisplayName|Version number|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_versionnumber|
|MaxValue|2147483647|
|MinValue|0|
|RequiredLevel|ApplicationRequired|
|Type|Integer|


### <a name="BKMK_OverriddenCreatedOn"></a> OverriddenCreatedOn

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Date and time that the record was migrated.|
|DisplayName|Record Created On|
|Format|DateOnly|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|overriddencreatedon|
|RequiredLevel|None|
|Type|DateTime|


### <a name="BKMK_OwnerId"></a> OwnerId

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|User who owns the satisfaction metric.|
|DisplayName|Owner|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|ownerid|
|RequiredLevel|SystemRequired|
|Targets|systemuser,team|
|Type|Owner|


### <a name="BKMK_OwnerIdType"></a> OwnerIdType

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Owner Id Type|
|DisplayName||
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridtype|
|RequiredLevel|SystemRequired|
|Type|EntityName|


### <a name="BKMK_statecode"></a> statecode

|Property|Value|
|--------|-----|
|Description|Status of the Satisfaction metric|
|DisplayName|Status|
|IsValidForCreate|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|statecode|
|RequiredLevel|SystemRequired|
|Type|State|

#### statecode Options

|Value|Label|DefaultStatus|InvariantName|
|-----|-----|-------------|-------------|
|0|Active|1|Active|
|1|Inactive|2|Inactive|



### <a name="BKMK_statuscode"></a> statuscode

|Property|Value|
|--------|-----|
|Description|Reason for the status of the Satisfaction metric|
|DisplayName|Status Reason|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|statuscode|
|RequiredLevel|None|
|Type|Status|

#### statuscode Options

|Value|Label|State|
|-----|-----|-----|
|1|Active|0|
|2|Inactive|1|



### <a name="BKMK_TimeZoneRuleVersionNumber"></a> TimeZoneRuleVersionNumber

|Property|Value|
|--------|-----|
|Description|For internal use only.|
|DisplayName|Time Zone Rule Version Number|
|Format|None|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|timezoneruleversionnumber|
|MaxValue|2147483647|
|MinValue|-1|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_UTCConversionTimeZoneCode"></a> UTCConversionTimeZoneCode

|Property|Value|
|--------|-----|
|Description|Time zone code that was in use when the record was created.|
|DisplayName|UTC Conversion Time Zone Code|
|Format|None|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|utcconversiontimezonecode|
|MaxValue|2147483647|
|MinValue|-1|
|RequiredLevel|None|
|Type|Integer|

<a name="read-only-attributes"></a>

## Read-only attributes

These attributes return false for both **IsValidForCreate** or **IsValidForUpdate**. Listed by **SchemaName**.

- [CreatedBy](#BKMK_CreatedBy)
- [CreatedByName](#BKMK_CreatedByName)
- [CreatedByYomiName](#BKMK_CreatedByYomiName)
- [CreatedOn](#BKMK_CreatedOn)
- [CreatedOnBehalfBy](#BKMK_CreatedOnBehalfBy)
- [CreatedOnBehalfByName](#BKMK_CreatedOnBehalfByName)
- [CreatedOnBehalfByYomiName](#BKMK_CreatedOnBehalfByYomiName)
- [ModifiedBy](#BKMK_ModifiedBy)
- [ModifiedByName](#BKMK_ModifiedByName)
- [ModifiedByYomiName](#BKMK_ModifiedByYomiName)
- [ModifiedOn](#BKMK_ModifiedOn)
- [ModifiedOnBehalfBy](#BKMK_ModifiedOnBehalfBy)
- [ModifiedOnBehalfByName](#BKMK_ModifiedOnBehalfByName)
- [ModifiedOnBehalfByYomiName](#BKMK_ModifiedOnBehalfByYomiName)
- [msfp_projectName](#BKMK_msfp_projectName)
- [OwnerIdName](#BKMK_OwnerIdName)
- [OwnerIdYomiName](#BKMK_OwnerIdYomiName)
- [OwningBusinessUnit](#BKMK_OwningBusinessUnit)
- [OwningTeam](#BKMK_OwningTeam)
- [OwningUser](#BKMK_OwningUser)
- [VersionNumber](#BKMK_VersionNumber)


### <a name="BKMK_CreatedBy"></a> CreatedBy

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier of the user who created the record.|
|DisplayName|Created By|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|createdby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_CreatedByName"></a> CreatedByName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_CreatedByYomiName"></a> CreatedByYomiName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdbyyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_CreatedOn"></a> CreatedOn

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Date and time when the record was created.|
|DisplayName|Created On|
|Format|DateAndTime|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|createdon|
|RequiredLevel|None|
|Type|DateTime|


### <a name="BKMK_CreatedOnBehalfBy"></a> CreatedOnBehalfBy

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier of the delegate user who created the record.|
|DisplayName|Created By (Delegate)|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|createdonbehalfby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_CreatedOnBehalfByName"></a> CreatedOnBehalfByName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdonbehalfbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_CreatedOnBehalfByYomiName"></a> CreatedOnBehalfByYomiName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdonbehalfbyyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_ModifiedBy"></a> ModifiedBy

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier of the user who modified the record.|
|DisplayName|Modified By|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|modifiedby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_ModifiedByName"></a> ModifiedByName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ModifiedByYomiName"></a> ModifiedByYomiName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedbyyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_ModifiedOn"></a> ModifiedOn

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Date and time when the record was modified.|
|DisplayName|Modified On|
|Format|DateAndTime|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|modifiedon|
|RequiredLevel|None|
|Type|DateTime|


### <a name="BKMK_ModifiedOnBehalfBy"></a> ModifiedOnBehalfBy

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier of the delegate user who modified the record.|
|DisplayName|Modified By (Delegate)|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_ModifiedOnBehalfByName"></a> ModifiedOnBehalfByName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ModifiedOnBehalfByYomiName"></a> ModifiedOnBehalfByYomiName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfbyyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_msfp_projectName"></a> msfp_projectName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|msfp_projectname|
|MaxLength|450|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_OwnerIdName"></a> OwnerIdName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Name of the owner|
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridname|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_OwnerIdYomiName"></a> OwnerIdYomiName

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Yomi name of the owner|
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_OwningBusinessUnit"></a> OwningBusinessUnit

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier for the business unit that owns the record|
|DisplayName|Owning Business Unit|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owningbusinessunit|
|RequiredLevel|None|
|Targets|businessunit|
|Type|Lookup|


### <a name="BKMK_OwningTeam"></a> OwningTeam

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier for the team that owns the record.|
|DisplayName|Owning Team|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owningteam|
|RequiredLevel|None|
|Targets|team|
|Type|Lookup|


### <a name="BKMK_OwningUser"></a> OwningUser

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Unique identifier for the user that owns the record.|
|DisplayName|Owning User|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owninguser|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_VersionNumber"></a> VersionNumber

**Added by**: Active Solution Solution

|Property|Value|
|--------|-----|
|Description|Version Number|
|DisplayName|Version Number|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|versionnumber|
|MaxValue|9223372036854775807|
|MinValue|-9223372036854775808|
|RequiredLevel|None|
|Type|BigInt|

<a name="manytoone"></a>

## Many-To-One Relationships

Each Many-To-One relationship is defined by a corresponding One-To-Many relationship with the related entity. Listed by **SchemaName**.


### <a name="BKMK_msfp_msfp_project_msfp_satisfactionmetric_project"></a> msfp_msfp_project_msfp_satisfactionmetric_project

See msfp_project Entity [msfp_msfp_project_msfp_satisfactionmetric_project](msfp_project.md#BKMK_msfp_msfp_project_msfp_satisfactionmetric_project) One-To-Many relationship.

### See also

[About the Entity Reference](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/about-entity-reference)<br />
[Programming reference for Dynamics 365 Customer Engagement (on-premises)](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/programming-reference)<br />
[Web API reference](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/about)<br />
