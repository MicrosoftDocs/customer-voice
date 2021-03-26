---
title: "msfp_question Entity Reference | MicrosoftDocs"
description: "Includes schema information and supported messages for the msfp_question entity."
ms.date: 07/29/2020
ms.service: 
  - crm-online
ms.topic: "reference"
author: "sbmjais"
ms.author: "shjais"
manager: "shujoshi"
---
# msfp_question Entity Reference

Question in a survey to collect feedback.

**Added by**: Dynamics 365 Customer Voice Solution

## Entity Properties

|Property|Value|
|--------|-----|
|CollectionSchemaName|msfp_questions|
|DisplayCollectionName|Customer Voice survey  questions|
|DisplayName|Customer Voice survey question|
|EntitySetName|msfp_questions|
|IsBPFEntity|False|
|LogicalCollectionName|msfp_questions|
|LogicalName|msfp_question|
|OwnershipType|UserOwned|
|PrimaryIdAttribute|msfp_questionid|
|PrimaryNameAttribute|msfp_name|
|SchemaName|msfp_question|

<a name="writable-attributes"></a>	

## Writable attributes	

These attributes return true for either **IsValidForCreate** or **IsValidForUpdate** (usually both). Listed by **SchemaName**.	

- [ImportSequenceNumber](#BKMK_ImportSequenceNumber)	
- [msfp_choicetype](#BKMK_msfp_choicetype)	
- [msfp_correctanswer](#BKMK_msfp_correctanswer)	
- [msfp_imageproperties](#BKMK_msfp_imageproperties)	
- [msfp_Maximumrating](#BKMK_msfp_Maximumrating)	
- [msfp_multiline](#BKMK_msfp_multiline)	
- [msfp_name](#BKMK_msfp_name)	
- [msfp_order](#BKMK_msfp_order)	
- [msfp_otherproperties](#BKMK_msfp_otherproperties)	
- [msfp_questionchoices](#BKMK_msfp_questionchoices)	
- [msfp_questionId](#BKMK_msfp_questionId)	
- [msfp_questiontext](#BKMK_msfp_questiontext)	
- [msfp_questiontype](#BKMK_msfp_questiontype)	
- [msfp_responserequired](#BKMK_msfp_responserequired)	
- [msfp_sequence](#BKMK_msfp_sequence)	
- [msfp_sourceparentquestionidentifier](#BKMK_msfp_sourceparentquestionidentifier)	
- [msfp_Sourcequestionidentifier](#BKMK_msfp_Sourcequestionidentifier)	
- [msfp_sourcesurveyidentifier](#BKMK_msfp_sourcesurveyidentifier)	
- [msfp_subtitle](#BKMK_msfp_subtitle)	
- [msfp_Survey](#BKMK_msfp_Survey)	
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


### <a name="BKMK_msfp_choicetype"></a> msfp_choicetype

|Property|Value|
|--------|-----|
|Description|Shows whether the question accepts single line or multiple lines of response.|
|DisplayName|Choice question type|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_choicetype|
|RequiredLevel|None|
|Type|Picklist|

#### msfp_choicetype Options

|Value|Label|
|-----|-----|
|647390000|Single choice|
|647390001|Multi choice|
|647390002|none|



### <a name="BKMK_msfp_correctanswer"></a> msfp_correctanswer

|Property|Value|
|--------|-----|
|Description|Stores the correct answer in case of quizzes.|
|DisplayName|Correct answer|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_correctanswer|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_imageproperties"></a> msfp_imageproperties

|Property|Value|
|--------|-----|
|Description|Question image properties in JSON format.|
|DisplayName|Image Properties|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_imageproperties|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_Maximumrating"></a> msfp_Maximumrating

|Property|Value|
|--------|-----|
|Description|Stores maximum rating of rating question type|
|DisplayName|Maximum rating|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_maximumrating|
|MaxValue|2147483647|
|MinValue|-2147483648|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_msfp_multiline"></a> msfp_multiline

|Property|Value|
|--------|-----|
|Description|Shows if the text question is multiple lines or not|
|DisplayName|Multiple lines|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_multiline|
|RequiredLevel|None|
|Type|Boolean|

#### msfp_multiline Options

|Value|Label|
|-----|-----|
|1|Yes|
|0|No|

**DefaultValue**: False



### <a name="BKMK_msfp_name"></a> msfp_name

|Property|Value|
|--------|-----|
|Description|The name of the custom entity.|
|DisplayName|Name|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_name|
|MaxLength|100|
|RequiredLevel|ApplicationRequired|
|Type|String|


### <a name="BKMK_msfp_order"></a> msfp_order

|Property|Value|
|--------|-----|
|Description|Order of the question in the survey.|
|DisplayName|Order|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_order|
|MaxValue|100000000000|
|MinValue|-100000000000|
|Precision|10|
|RequiredLevel|None|
|Type|Decimal|


### <a name="BKMK_msfp_otherproperties"></a> msfp_otherproperties

|Property|Value|
|--------|-----|
|Description|Stores other question properties in JSON format.|
|DisplayName|Other properties|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_otherproperties|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_questionchoices"></a> msfp_questionchoices

|Property|Value|
|--------|-----|
|Description|Stores the list of answer options|
|DisplayName|Question choices|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_questionchoices|
|MaxLength|1000000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_questionId"></a> msfp_questionId

|Property|Value|
|--------|-----|
|Description|Unique identifier for entity instances|
|DisplayName|Question|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|msfp_questionid|
|RequiredLevel|SystemRequired|
|Type|Uniqueidentifier|


### <a name="BKMK_msfp_questiontext"></a> msfp_questiontext

|Property|Value|
|--------|-----|
|Description|Text of the question in the survey.|
|DisplayName|Question text|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_questiontext|
|MaxLength|100000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_questiontype"></a> msfp_questiontype

|Property|Value|
|--------|-----|
|Description|Stores the type of question to display.|
|DisplayName|Question type|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_questiontype|
|RequiredLevel|None|
|Type|Picklist|

#### msfp_questiontype Options

|Value|Label|
|-----|-----|
|647390000|Choice|
|647390001|Text|
|647390002|Rating|
|647390003|Date|
|647390004|Ranking|
|647390005|MatrixChoiceGroup|
|647390006|MatrixChoice|
|647390007|NPS|
|647390008|File Upload|
|647390009|Number|
|647390010|Date and time|
|647390011|Drop-down|



### <a name="BKMK_msfp_responserequired"></a> msfp_responserequired

|Property|Value|
|--------|-----|
|Description|Shows if the question is mandatory.|
|DisplayName|Response required|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_responserequired|
|RequiredLevel|None|
|Type|Boolean|

#### msfp_responserequired Options

|Value|Label|
|-----|-----|
|1|Yes|
|0|No|

**DefaultValue**: False



### <a name="BKMK_msfp_sequence"></a> msfp_sequence

|Property|Value|
|--------|-----|
|Description|Order of the question in the survey.|
|DisplayName|Sequence|
|Format|None|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_sequence|
|MaxValue|2147483647|
|MinValue|-2147483648|
|RequiredLevel|None|
|Type|Integer|


### <a name="BKMK_msfp_sourceparentquestionidentifier"></a> msfp_sourceparentquestionidentifier

|Property|Value|
|--------|-----|
|Description|Unique identifier for the parent question in the source application.|
|DisplayName|Source parent question identifier|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_sourceparentquestionidentifier|
|MaxLength|250|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_msfp_Sourcequestionidentifier"></a> msfp_Sourcequestionidentifier

|Property|Value|
|--------|-----|
|Description|Unique identifier for the question in the source application.|
|DisplayName|Source question identifier|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_sourcequestionidentifier|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_msfp_sourcesurveyidentifier"></a> msfp_sourcesurveyidentifier

|Property|Value|
|--------|-----|
|Description|Unique identifier for the survey in the source application.|
|DisplayName|Source survey identifier|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_sourcesurveyidentifier|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_msfp_subtitle"></a> msfp_subtitle

|Property|Value|
|--------|-----|
|Description|Stores subtitle of a question.|
|DisplayName|Subtitle|
|Format|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_subtitle|
|MaxLength|50000|
|RequiredLevel|None|
|Type|Memo|


### <a name="BKMK_msfp_Survey"></a> msfp_Survey

|Property|Value|
|--------|-----|
|Description|Unique identifier of the survey to which the question belongs.|
|DisplayName|Survey|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|msfp_survey|
|RequiredLevel|None|
|Targets|msfp_survey|
|Type|Lookup|


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
|Description|Owner Id|
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
|Description|Status of the Question|
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
|Description|Reason for the status of the Question|
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
- [msfp_SurveyName](#BKMK_msfp_SurveyName)
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


### <a name="BKMK_msfp_SurveyName"></a> msfp_SurveyName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|msfp_surveyname|
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

<a name="onetomany"></a>

## One-To-Many Relationships

Listed by **SchemaName**.


### <a name="BKMK_msfp_msfp_question_msfp_questionresponse_questionid"></a> msfp_msfp_question_msfp_questionresponse_questionid

Same as msfp_questionresponse entity [msfp_msfp_question_msfp_questionresponse_questionid](msfp_questionresponse.md#BKMK_msfp_msfp_question_msfp_questionresponse_questionid) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|msfp_questionresponse|
|ReferencingAttribute|msfp_questionid|
|IsHierarchical|False|
|IsCustomizable|True|
|ReferencedEntityNavigationPropertyName|msfp_msfp_question_msfp_questionresponse_questionid|
|AssociatedMenuConfiguration|Behavior: UseCollectionName<br />Group: Details<br />Label: <br />Order: 10000|
|CascadeConfiguration|Assign: NoCascade<br />Delete: RemoveLink<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: Cascade<br />Unshare: Cascade|

<a name="manytoone"></a>

## Many-To-One Relationships

Each Many-To-One relationship is defined by a corresponding One-To-Many relationship with the related entity. Listed by **SchemaName**.


### <a name="BKMK_msfp_msfp_survey_msfp_question_Survey"></a> msfp_msfp_survey_msfp_question_Survey

See msfp_survey Entity [msfp_msfp_survey_msfp_question_Survey](msfp_survey.md#BKMK_msfp_msfp_survey_msfp_question_Survey) One-To-Many relationship.

### See also

[About the Entity Reference](/dynamics365/customerengagement/on-premises/developer/about-entity-reference)<br />
[Programming reference for Dynamics 365 Customer Engagement (on-premises)](/dynamics365/customerengagement/on-premises/developer/programming-reference)<br />
[Web API reference](/dynamics365/customer-engagement/web-api/about)<br />


[!INCLUDE[footer-include](../../includes/footer-banner.md)]