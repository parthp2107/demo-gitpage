# Database

<b id="httpsopen-metadata.orgschemaentitydatadatabase.json">&#36;id: https://open-metadata.org/schema/entity/data/database.json</b>

Type: `object`

## Properties
 - **id**
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - &#36;ref: [#/definitions/databaseName](definitionsdatabasename)
 - **fullyQualifiedName**
	 - Type: `string`
 - **description**
	 - Type: `string`
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
 - **owner**
	 - &#36;ref: [../../type/entityReference.json](....typeentityreference.md)
 - **service** `required`
	 - &#36;ref: [../../type/entityReference.json](....typeentityreference.md)
 - **usageSummary**
	 - &#36;ref: [../../type/usageDetails.json](....typeusagedetails.md)
 - **tables**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)


## Type definitions in this schema
### databaseName

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


