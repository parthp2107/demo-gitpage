# Topic

<b id="httpsopen-metadata.orgschemaentitydatatopic.json">&#36;id: https://open-metadata.org/schema/entity/data/topic.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/topicName](#/definitions/topicName)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/fullyQualifiedName">fullyQualifiedName</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/service">service</b> `required`
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/partitions">partitions</b> `required`
	 - Type: `integer`
	 - Range:  &ge; 1
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/schemaText">schemaText</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/schemaType">schemaType</b>
	 - &#36;ref: [#/definitions/schemaType](#/definitions/schemaType)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/cleanupPolicies">cleanupPolicies</b>
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/cleanupPolicy](#/definitions/cleanupPolicy)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/retentionTime">retentionTime</b>
	 - Type: `number`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/maximumMessageSize">maximumMessageSize</b>
	 - Type: `integer`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/minimumInSyncReplicas">minimumInSyncReplicas</b>
	 - Type: `integer`
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/retentionSize">retentionSize</b>
	 - Type: `number`
	 - Default: _"-1"_
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/owner">owner</b>
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/followers">followers</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/tags">tags</b>
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [../../type/tagLabel.json](#....typetaglabel.json)
 - <b id="#https://open-metadata.org/schema/entity/data/topic.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)


## Type definitions in this schema
**topicName**

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


**schemaType**

 - The value is restricted to the following: 
	 1. _"Avro"_
	 2. _"Protobuf"_
	 3. _"JSON"_
	 4. _"Other"_


**cleanupPolicy**

 - The value is restricted to the following: 
	 1. _"delete"_
	 2. _"compact"_


