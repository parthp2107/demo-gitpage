# Database

<b id="httpsopen-metadata.orgschemaentitydatadatabase.json">&#36;id: https://open-metadata.org/schema/entity/data/database.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/id">id</b>
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/databaseName](#/definitions/databaseName)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/fullyQualifiedName">fullyQualifiedName</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/owner">owner</b>
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/service">service</b> `required`
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/usageSummary">usageSummary</b>
	 - &#36;ref: [../../type/usageDetails.json](#....typeusagedetails.json)
 - <b id="#https://open-metadata.org/schema/entity/data/database.json/properties/tables">tables</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)


## Type definitions in this schema
**databaseName**

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


